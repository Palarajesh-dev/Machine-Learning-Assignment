# Heart Disease Prediction Using a Multilayer Perceptron (MLP)

This project implements a **Multilayer Perceptron (MLP)** neural network to predict the likelihood of heart disease based on demographic, lifestyle, and clinical attributes such as cholesterol, blood pressure, chest pain type, smoking habits, and more.

The aim is to demonstrate a complete machine-learning pipeline involving **data preprocessing**, **feature encoding**, **scaling**, **model training**, and **evaluation**.  
This work is based on the analysis presented in the project report.

---

## ❤️ Background

Heart disease remains a leading cause of death worldwide. Machine-learning models can help identify individuals at higher risk by learning patterns within clinical and lifestyle data.

The MLP model used here is well suited for this prediction task because:

- It can model **nonlinear relationships** in patient characteristics.
- It works well with **mixed data types** (numeric + categorical after encoding).
- It performs efficiently on moderately sized datasets.

---

## 📊 Dataset

The dataset includes typical cardiovascular health factors, such as:

- **Age, sex**
- **Resting blood pressure**
- **Cholesterol**
- **Smoking status**
- **Diabetes status**
- **Maximum heart rate**
- **Chest pain type**
- **Exercise-related attributes**

The target variable:  
- `HeartDisease` — 1 = disease present, 0 = no disease.

---

## 🧠 Methodology

### **1. Preprocessing**
- Separate features (`X`) and labels (`y`)
- Identify categorical features automatically
- Apply **One-Hot Encoding**
- Apply **StandardScaler** to numerical features

### **2. Train–Test Split**
- 80% training  
- 20% testing  
- Stratified sampling to preserve class balance

### **3. MLP Architecture**

| Component | Value |
|----------|--------|
| Hidden Layers | (64, 32) |
| Activation | ReLU |
| Optimizer | Adam |
| Regularization | α = 1e-4 |
| Max Iterations | 200 |

### **4. Pipeline**
A Scikit-learn `Pipeline` ensures clean, leak-free preprocessing:

---

## 📈 Results

- **High precision and recall for both classes**
- **Low error rates** in confusion matrix
- Model demonstrates strong predictive power on structured health data


---

## 🧪 Possible Improvements

- Hyperparameter tuning (learning rate, neurons, layers)
- Add class balancing (e.g., SMOTE)
- Try other models (Random Forest, XGBoost)
- Apply feature selection or dimensionality reduction

---

## ⚖️ Ethical Considerations

ML systems used in healthcare must be carefully validated:

- False negatives may delay treatment  
- False positives can create anxiety  
- Models should **support**, not replace, medical professionals  
- Patient privacy and data security are essential  

This project is for **educational purposes only** and not for clinical decision-making.

---

## 📚 References

- Scikit-learn Documentation  
- Bishop, C. (2006). *Pattern Recognition and Machine Learning*  
- UCI Heart Disease Dataset (structural inspiration)  
- Course notes & lectures  

---

## 📎 GitHub Repository
  
 https://github.com/Palarajesh-dev/Machine-Learning-Assignment.git

---

## 📝 License

This project is released under the **MIT License** — see the LICENSE file for details.


