[README.md](https://github.com/user-attachments/files/32160332/README.md)
# fashion_mnist_model.keras--# Fashion MNIST Image Classification using Deep Learning

## 📌 Project Overview
Is project mein **Fashion MNIST** dataset use karke ek Deep Learning model banaya gaya hai jo clothing items (jaise shoes, shirts, bags, etc.) ko unki images se classify kar sake. Yeh approach usi tarah hai jaise MNIST dataset mein handwritten digits (0-9) classify kiye jaate hain.

## 📂 Dataset
**Fashion MNIST** — TensorFlow/Keras ki built-in library se load hota hai.

- Training images: 60,000
- Testing images: 10,000
- Image size: 28x28 pixels (grayscale)

| Label | Class        |
|-------|--------------|
| 0     | T-shirt/top  |
| 1     | Trouser      |
| 2     | Pullover     |
| 3     | Dress        |
| 4     | Coat         |
| 5     | Sandal       |
| 6     | Shirt        |
| 7     | Sneaker      |
| 8     | Bag          |
| 9     | Ankle boot   |

## ⚙️ Requirements
```
tensorflow
numpy
matplotlib
```

Install karne ke liye:
```
pip install tensorflow numpy matplotlib
```

## 🧠 Model Architecture
```
Input (28x28) 
   → Flatten 
   → Dense (128, ReLU) 
   → Dense (64, ReLU) 
   → Dense (10, Softmax)
```

## 🚀 Steps (Project Workflow)

1. **Data Loading** — `tf.keras.datasets.fashion_mnist.load_data()` se dataset load kiya gaya.
2. **Preprocessing** — Pixel values (0–255) ko normalize karke (0–1) range mein convert kiya gaya.
3. **Model Building** — Sequential Neural Network define kiya gaya.
4. **Compilation** — Adam optimizer aur Sparse Categorical Crossentropy loss function use kiya gaya.
5. **Training** — Model ko 10 epochs tak train kiya gaya, validation split ke sath.
6. **Evaluation** — Test dataset par model ki accuracy check ki gayi.
7. **Prediction** — Trained model se test images par predictions li gayin.
8. **Visualization** — Predictions ko actual images ke saath graphically dikhaya gaya.
9. **Graphs** — Training/Validation accuracy aur loss ka graph banaya gaya.
10. **Model Saving** — Trained model `.keras` / `.h5` format mein save kiya gaya.

## ▶️ How to Run
```bash
python fashion_mnist.py
```

## 📊 Results
Model ne test dataset par approximately **87-88% accuracy** achieve ki.

## 💾 Output Files
- `training_graph.png` — Accuracy/Loss graph
- `fashion_mnist_model.keras` — Saved trained model

## 📝 Conclusion
Yeh project dikhata hai ke wahi Deep Learning approach jo digit classification (MNIST) ke liye use hoti hai, usi tarah image-based fashion item classification ke liye bhi apply ki ja sakti hai — sirf dataset aur output classes change hote hain, model ka basic structure same rehta hai.

## 👤 Author
Assignment submitted as part of Deep Learning coursework.
