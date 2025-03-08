# Building an Image Classifier Web App with Streamlit

#streamlit #IronHack #deployment 

## What is Streamlit?
Streamlit is a Python library that turns your Python scripts into interactive web applications. It allows you to create a website without knowing HTML, CSS, or JavaScript. You can run it locally or you can publish it on Streamlit platform.
https://streamlit.io/

## Why Streamlit is Great for AI Apps
- You write pure Python code
- Your app updates automatically as users interact with it
- It's free to host basic applications
- You don't need to know web development

## Installing Streamlit
Using Anaconda: https://docs.streamlit.io/get-started/installation/anaconda-distribution
Using pip: `pip install streamlit`

## Writing your first app
### The Main Script
Every Streamlit app starts with a Python file (usually called `app.py` or `streamlit_app.py`). This file contains both your AI logic and your interface code. Here's a simple example:

**Try running it on your computer!**
1. Create new directory `my_cnn_app` (or something like that)
2. Create an `.py` file named `app.py` 
3. Copy into into it the code below
```python
import streamlit as st # importing streamlit library
  
st.title("Image Classifier") # this text will appear big
```

### Running Your First App
4. Open terminal/command prompt
5. Run your app:
```bash
python -m streamlit run app.py
```

### How Streamlit Works
Every time you interact with your Streamlit app (type in a textbox, move a slider, click a button), **Streamlit runs your entire script again from top to bottom. This means any variables you create will be reset!**

Streamlit works in an unusual way for a webapp. Every time you do anything in a Streamlit app - click a button, type text, upload a file - Streamlit runs your entire program again from start to finish. It's like closing and reopening your jupyter notebook. All the variables are forgotten.

*We will learn how to save the variables between re-runs in a few days.*

## Building an Image Classifier App with Streamlit

Now let's build a more advanced app: a CIFAR-10 image classifier that can recognize 10 different types of objects in uploaded images.

### Step 1: Project Setup
1. Create a new directory for your project
2. Create a new file called `app.py`
3. Make sure you have your pre-trained model file (`cifar10_cnn_model.h5`) in the same directory

### Step 2: Import Required Libraries
The first part of our app imports all the necessary libraries:

```python
import streamlit as st
import tensorflow as tf
import numpy as np
from PIL import Image
```

Let's understand what each library does:
- `streamlit`: Creates our web interface
- `tensorflow`: Loads and runs our machine learning model
- `numpy`: Helps us work with arrays (for image processing)
- `PIL`: Python Imaging Library - helps us work with images

### Step 3: Load the Pre-trained Model
This section loads our pre-trained CNN model:

```python
# Load the pre-trained model and cache it (so that we don't have to load it every time)
@st.cache_resource
def load_model():
    return tf.keras.models.load_model('cifar10_cnn_model.h5')

```
- `@` here above the function name signifies something called `decorator`. A decorator in Python is a special kind of function that modifis behavior of a given function without changing function code. Think of decorators like adding a special ability to a function. The decorator intercepts the function call, adds some extra functionality, and then proceeds with the original function.
- `@st.cache_resource`: This is a special decorator that tells Streamlit to save the model in memory after loading it the first time. Remember how Streamlit reruns the entire script for every interaction? Without caching, it would reload the model every time you click anything!
```python
# Define CIFAR-10 class names
class_names = [
    'airplane', 'automobile', 'bird', 'cat', 'deer',
    'dog', 'frog', 'horse', 'ship', 'truck'
]
```
- `class_names`: This list contains the names of the 10 classes our model can predict.

### Step 4: Create the Web Interface
Now we set up the basic elements of our web app:

```python
# Set up the Streamlit app
st.title('CIFAR-10 Image Classifier')
st.write('Upload an image and the model will predict its class')

# File uploader
uploaded_file = st.file_uploader("Choose an image...", type=["jpg", "jpeg", "png"])
```

- `st.title()`: Creates a big heading for our app
- `st.write()`: Adds some text to explain what the app does
- `st.file_uploader()`: Creates a button that lets users upload image files

### Step 5: Image Preprocessing Function
Before feeding an image to our model, we need to prepare it:

```python
def preprocess_image(image):
    image = image.convert('RGB')
    image = image.resize((32, 32)) # has to be the same as your model input!!!
    image_array = np.array(image)
    image_array = image_array.astype('float32') / 255.0
    image_array = np.expand_dims(image_array, axis=0) 
    return image_array
```

This function:
1. Converts the image to RGB format (in case it's in another format)
2. Resizes it to 32x32 pixels (what our CIFAR-10 model expects)
    1. If you are using a different model you have resize it to your model input size
3. Converts the image to a numpy array
4. Scales pixel values to be between 0 and 1
    1. We did this during training because neural networks work better with smaller numbers. Values between 0-1 are less likely to cause computational issues than values between 0-255.
    2. If you didn't do this traing, you definitely should go back and to it.
5. Adds a batch dimension (our model expects a batch of images)

### Step 6: Making Predictions
The final part of our code handles the prediction process:

```python
# If an image is uploaded, we are going to make a prediction and display the results
if uploaded_file is not None:
    # Display the uploaded image
    image = Image.open(uploaded_file)
    st.image(image, caption='Uploaded Image', use_column_width=True)
    
    # Preprocess the image
    image_array = preprocess_image(image)
    
    # Load model and make prediction
    model = load_model()
    predictions = model.predict(image_array)
    predicted_class = class_names[np.argmax(predictions[0])]
    confidence = np.max(predictions[0]) * 100
    
    # Display results
    st.write(f"Prediction: {predicted_class}")
    st.write(f"Confidence: {confidence:.2f}%")
    
    # Display bar chart of all predictions
    st.bar_chart({class_names[i]: float(predictions[0][i]) for i in range(10)})
```

Let's break this down:
1. The `if uploaded_file is not None:` checks if a user has uploaded an image
2. If an image is uploaded:
   - We display the uploaded image with `st.image()`
   - We preprocess the image using our function
   - We load the model and make a prediction
   - We find the class with the highest probability
   - We calculate the confidence (probability * 100)
   - We display the prediction and confidence
   - We create a bar chart showing the probabilities for all classes
