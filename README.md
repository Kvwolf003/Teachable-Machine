# Teachable-Machine

# 🧠 Image Classification using Keras Model

This project uses a **pre-trained Keras model** to classify images. It loads a custom model and label set to predict the class of a provided image.

---

## 📂 Project Structure

```text
project/
│
├── keras_model[1].h5       # Pre-trained Keras model
├── labels[1].txt           # Class labels file
├── OIP (convert.io).png    # Image to be classified
├── classify.py             # Python script for prediction
└── README.md               # Project documentation
```

---

## 🔧 Requirements

* Python 3.x
* TensorFlow
* Keras
* Pillow
* NumPy

### Install Dependencies:

```bash
pip install tensorflow pillow numpy
```

---

## 🚀 How to Run

1. Ensure the following files are in the project directory:

   * `keras_model[1].h5`
   * `labels[1].txt`
   * The image you want to classify (default is `OIP (convert.io).png`)

2. Run the Python script:

```bash
python classify.py
```

3. The output will display:

```text
Class: [Predicted Class]
Confidence Score: [Confidence Value]
```

---

## 🖼️ Image Requirements

* Input images should be resized to **224x224 pixels**.
* Image is normalized to fit the model’s expected input range.

---

## 🧩 Key Concepts Used

* **Keras Model Loading**
* **Image Preprocessing (Resizing, Normalization)**
* **Numpy Array Handling**
* **Confidence Scoring**

---

## ✅ Notes

* The script currently uses a hardcoded image path:
  `"/OIP (convert.io).png"`
  You can replace this with your own image path.

* The labels file `labels[1].txt` should have each class name on a separate line.

* Make sure your model input size matches the preprocessing size `(224, 224, 3)`.

---

## 🌟 Possible Improvements

* Add command-line arguments to easily input different image paths.
* Build a GUI or web interface for user-friendly image selection.
* Add batch image processing functionality.
* Implement model evaluation on a test dataset.

---

## 📜 License

This project is released under the MIT License.

