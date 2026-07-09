 🤖 Electronic Components Classification Project (Sensors vs. Actuators)

This project aims to build an artificial intelligence model that can automatically classify two main types of electronic components used in robotics and
embedded systems: Sensors and Actuators. 
Sensors are responsible for collecting data from the surrounding environment,
while actuators perform actions or movements based on commands.
The project started by collecting images of different electronic components and using Google Teachable Machine to train a machine learning
model capable of recognizing them. After the training process was completed, the model was exported in Keras format (keras_model.h5) along with the labels.txt file, 
which contains the class labels for use during testing.
The testing phase was implemented in Python using Google Colab. The program uses libraries such as TensorFlow/Keras, NumPy,
and Pillow to preprocess input images before passing them to the trained model. Each image is resized to 224 × 224 pixels and normalized to match the
format used during training, ensuring more accurate predictions.
Once the image has been processed, the model analyzes it and predicts whether the component is a Sensor or an Actuator. The final output displays
the predicted class along with a Confidence Score, which indicates how confident the model is in its prediction. During testing, the model successfully 
identified a sensor with a confidence score of over 90%, demonstrating good classification performance.
