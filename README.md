 🤖 Electronic Components Classification Project (Sensors vs. Actuators)

This project aims to build an artificial intelligence model that automatically classifies electronic components into two main types:
Sensors (which collect environment data) and Actuators (which perform actions or movements).


The model was trained using Google Teachable Machine by uploading various images of these components. Once the
training was complete, the model was exported in Keras format (⁠keras_model.h5⁠) alongside a ⁠labels.txt⁠ file 
containing the classification categories.


The testing phase was implemented in Python using Google Colab. The script uses libraries like ⁠TensorFlow⁠,
⁠NumPy⁠, and ⁠Pillow⁠ to resize and normalize the input image, then passes it to the model to predict the component type with a specific Confidence Score.
