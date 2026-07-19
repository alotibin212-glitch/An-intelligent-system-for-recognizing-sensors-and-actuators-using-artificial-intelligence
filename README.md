 # 🤖 Electronic Components Classification (Sensors vs. Actuators)

An AI-powered vision model that looks at an electronic component and instantly tells you: does this part **sense** the world, or does it **act** on it?

---

## 🎯 The Idea

Every electronic circuit has two kinds of "senses": components that **perceive** the environment, and components that **respond** to it. This project builds a machine learning model that automatically classifies a component image into one of two categories:

| Type | Role | Examples |
|------|------|----------|
| 🌡️ **Sensors** | The eyes and ears of the circuit — collect data from the environment (temperature, light, motion, etc.) | Thermistors, photoresistors, PIR sensors |
| ⚙️ **Actuators** | The muscles of the circuit — turn signals into real physical action | Motors, servos, solenoids, relays |

---

## 🧠 How the Model Was Trained

The model was trained using **Google Teachable Machine**, by uploading a diverse set of images for each component category. Once training was complete, the model was exported as:

- `keras_model.h5` — the trained Keras model
- `labels.txt` — the list of classification labels

This lets the model "recognize" components visually, the same way it was taught during training.

---

## 🚀 How Testing Works

Testing was implemented in **Python**, using **Google Colab** as the environment. The pipeline works like this:

1. **Load & preprocess the image** — resized and normalized using **Pillow**
2. **Run inference** — the image is passed through the trained **TensorFlow** model
3. **Handle data** — **NumPy** organizes the numerical arrays behind the scenes
4. **Get the result** — the model outputs the predicted class (*Sensor* or *Actuator*) along with a **Confidence Score**

---

## 🛠️ Tech Stack

- 🧩 Google Teachable Machine — model training
- 🐍 Python — scripting and inference
- 📓 Google Colab — testing environment
- 🔶 TensorFlow / Keras — model framework
- 🔢 NumPy — numerical processing
- 🖼️ Pillow (PIL) — image preprocessing

---

## 📂 Project Files

```
├── keras_model.h5      # Trained classification model
├── labels.txt           # Class labels (Sensor / Actuator)
└── test_script.ipynb    # Colab notebook for testing predictions
```

---

## ✨ Why This Matters

This project shows how a machine can learn to "see" from just a handful of examples, and turn that learning into confident, measurable decisions. It's a small but real step toward machines that understand and interact with their environment intelligently.
