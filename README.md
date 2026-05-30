# Fashion-MNIST: Shallow vs Deep CNN Comparative Study

## 📌 Objective
This project compares the performance of a **Shallow CNN** and a **Deep CNN** on the Fashion-MNIST dataset.  
The goal is to analyze efficiency, accuracy, and generalization, and to understand the trade-offs between model simplicity and complexity.

---

## 📂 Dataset Overview
- **Dataset**: Fashion-MNIST (60,000 training images, 10,000 test images)
- **Image size**: 28 × 28 grayscale
- **Classes**: 10 categories (T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot)

---

## ⚙️ Experiments
### Part 1: Data Loading & Preprocessing
- Loaded Fashion-MNIST dataset
- Normalized pixel values (0–1)
- Reshaped images to `(28,28,1)` for CNN input

### Part 2: Shallow CNN
- Architecture: Input → Conv2D(32) → MaxPooling2D → Flatten → Dense(64) → Dense(10)
- 1 Conv2D layer + 1 MaxPooling2D
- Flatten → Dense(64) → Output(10)
- Faster training, fewer parameters
- Showed signs of **underfitting**

### Part 3: Deep CNN
- Architecture: Input → Conv2D(32) → MaxPooling2D → Conv2D(64) → MaxPooling2D → Conv2D(128) → Flatten → Dense(128) → Dense(64) → Dense(10)
- 3 Conv2D layers + multiple MaxPooling2D
- Dense(128) → Dense(64) → Output(10)
- More parameters, longer training time
- Achieved **higher accuracy** and better generalization

### Part 4: Comparative Study
| Metric                | Shallow CNN | Deep CNN |
|-----------------------|-------------|----------|
| Conv Layers           | 1           | 3        |
| Total Parameters      | ~X          | ~Y       |
| Training Accuracy     | ~A%         | ~B%      |
| Validation Accuracy   | ~C%         | ~D%      |
| Test Accuracy         | ~E%         | ~F%      |
| Over/Underfitting     | Underfit    | Slight overfit |
| Training Time         | Faster      | Slower   |

*(Replace X, Y, A–F with your actual results from notebook output)*

### Part 5: Prediction & Error Analysis
- Confusion matrices for both models
- 5 correctly classified + 5 misclassified images displayed
- Deep CNN reduced confusion between similar classes (e.g., Shirt vs T-shirt/top)

### Part 6: Final Conclusion
- **Recommended model**: Deep CNN (better accuracy & generalization)
- **More efficient model**: Shallow CNN (faster, fewer parameters)
- **More accurate model**: Deep CNN
- **Key learning**: Trade-off between simplicity and performance — deeper models justify complexity when accuracy is critical.

---

## 📑 Deliverables
- `ShallowCNN-DeepCNN.ipynb` → Jupyter Notebook with all experiments, plots, and outputs
- `report.md` → Short comparative report summarizing objectives, dataset, experiments, and conclusions

---

## 🚀 How to Run
1. Open the notebook in **Google Colab** (recommended for GPU support).
2. Run all cells sequentially.
3. Outputs (plots, confusion matrices, tables) will be generated inline.
4. No external CSVs required — Fashion-MNIST loads directly via Keras.

---

## 👨‍💻 Author
- **Arnab Bera**  
- Senior Full Stack MERN Developer & Technical Architect  
- Contact: seacom.arnab@gmail.com  
- GitHub: [Arnab-Bera](https://github.com/Arnab-Bera)
