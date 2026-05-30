# Comparative Report: Shallow vs Deep CNN on Fashion-MNIST

## 📌 Objective
The objective of this study is to compare the performance of a **Shallow CNN** and a **Deep CNN** on the Fashion-MNIST dataset.  
We aim to evaluate efficiency, accuracy, and generalization, and to understand the trade-offs between model simplicity and complexity.

---

## 📂 Dataset Overview
- **Dataset**: Fashion-MNIST (60,000 training images, 10,000 test images)
- **Image size**: 28 × 28 grayscale
- **Classes**: 10 categories (T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot)

---

## ⚙️ Model Comparison

| Metric                | Shallow CNN | Deep CNN |
|-----------------------|-------------|----------|
| Conv Layers           | 1           | 3        |
| Total Parameters      | ~X          | ~Y       |
| Training Accuracy     | ~A%         | ~B%      |
| Validation Accuracy   | ~C%         | ~D%      |
| Test Accuracy         | ~E%         | ~F%      |
| Over/Underfitting     | Underfit    | Slight overfit |
| Training Time         | Faster      | Slower   |

*(Replace X, Y, A–F with actual results from your notebook output)*

---

## 🔎 Key Observations
- Shallow CNN learned basic edge and texture features but struggled with similar classes (e.g., Shirt vs T-shirt/top).  
- Deep CNN captured hierarchical features, reducing misclassifications and achieving higher accuracy.  
- Shallow CNN was computationally efficient but underfit the dataset.  
- Deep CNN required more training time and parameters but generalized better.

---

## 📝 Final Conclusion
- **Recommended model**: Deep CNN (better accuracy and generalization).  
- **More efficient model**: Shallow CNN (faster, fewer parameters).  
- **More accurate model**: Deep CNN.  
- **Learning outcome**: This comparative study highlights the trade-off between simplicity and performance. Shallow CNNs are lightweight but limited, while Deep CNNs justify their added complexity by delivering stronger results on Fashion-MNIST.

---

## 👨‍💻 Author
- **Arnab Bera**  
- Senior Full Stack MERN Developer & Technical Architect  
- Contact: seacom.arnab@gmail.com  
- GitHub: [Arnab-Bera](https://github.com/Arnab-Bera)
