# 🎮 Laptop Performance Prediction (FPS)

A Machine Learning project that predicts **gaming performance (Frames Per Second - FPS)** of a laptop based on its hardware specifications.

This project implements **Multiple Linear Regression from scratch using NumPy**, without using any machine learning libraries like Scikit-Learn.

The model is trained using **Gradient Descent optimization**.

---

# 📌 Project Overview

Gaming performance depends heavily on hardware configuration such as:

* RAM
* GPU performance
* CPU speed
* Storage capacity

This project builds a regression model that learns the relationship between these features and the **FPS produced in games**.

The model is implemented **completely from scratch** using mathematical formulas and NumPy operations.

---

# 🧠 Machine Learning Approach

The project implements **Multiple Linear Regression** with the following equation:

```
FPS = w1 × RAM + w2 × GPU + w3 × CPU + w4 × Storage + b
```

Where:

* **w1, w2, w3, w4** → feature weights
* **b** → bias term

The weights are learned using **Gradient Descent**.

---

# ⚙️ Algorithm Implementation

The notebook implements the following core components:

### 1️⃣ Prediction Function

Computes predicted FPS values.

```
y_pred = X·W + b
```

Implemented using:

```
np.dot(x, w)
```

---

### 2️⃣ Cost Function

Mean Squared Error cost function:

```
J(w,b) = (1/2m) Σ (y_pred − y)^2
```

Used to measure model error during training.

---

### 3️⃣ Gradient Computation

Gradients for updating weights:

```
dj_dw = (1/m) * Xᵀ (y_pred − y)
dj_db = (1/m) * Σ(y_pred − y)
```

---

### 4️⃣ Gradient Descent

Parameters are updated iteratively:

```
w = w − α * dj_dw
b = b − α * dj_db
```

Where:

* **α (alpha)** → learning rate
* **iterations** → number of training steps

---

# 📊 Visualizations

The project includes several visualizations:

### Training Cost

Shows how the cost decreases during training.

### Prediction Convergence

Shows how the predicted FPS stabilizes over iterations.

### Feature Importance

Displays the learned weights for:

* RAM
* GPU
* CPU
* Storage

---

# 🛠 Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Jupyter Notebook**

---

# 📂 Project Structure

```
MULTIPLE_LINEAR_REGRESSION_PROJECT
│
├── data.csv
│   Dataset containing laptop hardware specifications and FPS values
│
├── laptop_performance_prediction_multiple_LR.ipynb
│   Implementation of Multiple Linear Regression using Gradient Descent
│
└── README.md
```

---

# 🚀 Example Prediction

Example input:

```
RAM: 12 GB
GPU Score: 4200
CPU Speed: 2.5 GHz
Storage: 320 GB
```

Model output:

```
Predicted FPS ≈ 54.6
```

---

# 🔬 Key Learning Outcomes

This project demonstrates:

* Implementing **linear regression from scratch**
* Understanding **cost functions**
* Computing **gradients manually**
* Implementing **gradient descent optimization**
* Visualizing training behavior

---

# 👨‍💻 Author

**Hemanth M**
Computer Science Engineering Student
India 🇮🇳

Interested in **Machine Learning, AI, and Software Development**.

---

⭐ If you find this project useful, consider giving it a **star**.
