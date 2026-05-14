# 🌌 Cosmological Data Analysis – Hubble's Constant Estimation

## 📌 Project Overview

This project focuses on estimating **Hubble’s Constant (H₀)** using observational cosmological data through **Linear Regression**.

Hubble’s Constant represents the rate at which the universe is expanding. It is calculated using the relationship between:

* **Galaxy distance**
* **Recessional velocity**

We perform analysis in two scenarios:

1. **With Outliers**
2. **Without Outliers**

Additionally, statistical measures such as **Mean** and **Variance** are computed for both cases.

---

## 🎯 Objectives

* Apply **Linear Regression** to cosmological data
* Compute:

  * Mean
  * Variance
  * Hubble’s Constant (slope of regression line)
* Compare results:

  * With outliers
  * Without outliers
* Visualize and interpret results

---

## 📂 Project Structure

```
📦 Cosmological-Data-Analysis
│
├── 📁 data
│   ├── Datasheet 1.csv
│   ├── Datasheet 2.csv
    ├── Datasheet 3.csv
│
├── 📁 Notebooks
│   ├── A7P1.ipynb
│   ├── A7P2.ipynb
│   ├── A7P3.ipynb
│
├── README.md
└── requirements.txt
```
> *Run command [pip install -r requirements.txt] before executing any notebook*
---

## 📊 Notebooks

### 🔹 1. Data Analysis

This notebook focuses on understanding and preparing the dataset before applying any models.

Detailed tasks performed:

* Loading CSV files from the `/Data` directory
* Inspecting dataset structure (rows, columns, datatypes)
* Handling missing values (if any)
* Identifying inconsistencies in data
* Visualizing distributions using plots
* Understanding relationship trends between **distance** and **velocity**
* Detecting potential outliers through scatter plots and statistical checks

👉 **Open Notebook:**
[Click here to view](./Notebooks/A7P1.ipynb)

---

### 🔹 2. Linear Regression Model

This notebook implements the core machine learning logic used to estimate Hubble’s Constant.

Detailed tasks performed:

* Separating independent (distance) and dependent (velocity) variables
* Applying Linear Regression using libraries like **Scikit-learn** or manual implementation
* Fitting the regression model to the dataset
* Plotting the regression line over actual data points
* Evaluating model behavior with and without outliers
* Understanding slope interpretation as Hubble’s Constant
* Comparing regression performance visually

👉 **Open Notebook:**
[Click here to view](./Notebooks/A7P2.ipynb)

---

### 🔹 3. Hubble’s Constant Calculation

This notebook contains the final computation and comparison of statistical and regression results.

Detailed tasks performed:

* Calculating **Mean** of distance and velocity values
* Calculating **Variance** to understand data spread
* Extracting slope from regression model as **Hubble’s Constant (H₀)**
* Performing calculations for:

  * Dataset with outliers
  * Dataset without outliers
* Comparing both cases numerically and graphically
* Interpreting how outliers affect final cosmological conclusions

👉 **Open Notebook:**
[Click here to view](./Notebooks/A7P3.ipynb)

---

## 📈 Methodology

### 1. Data Collection

* Data is stored in the `/Data` folder as CSV files.
* Contains:

  * Distance (Mpc)
  * Velocity (km/s)

---

### 2. Statistical Analysis

For both datasets:

* Mean:

  μ = (1/n) Σ xi

* Variance:

  σ² = (1/n) Σ (xi - μ)²

---

### 3. Linear Regression

We use the equation:

v = H₀ · d

Where:

* v = velocity
* d = distance
* H₀ = Hubble’s Constant (slope)

---

### 4. Outlier Handling

* Results are computed:

  * Including outliers
  * After removing outliers
* Helps improve model accuracy and reliability

---

## 📌 Results

| Case             | Mean | Variance | Hubble Constant (H₀) |
| ---------------- | ---- | -------- | -------------------- |
| With Outliers    | ✔️   | ✔️       | ✔️                  |
| Without Outliers | ✔️   | ✔️       | ✔️                  |

*(Values are computed inside notebooks)*

---

## 🧠 Key Insights

* Outliers significantly impact regression results
* Removing outliers leads to:

  * More stable slope
  * Better estimation of H₀
* Linear relationship validates **Hubble’s Law**

---

## ⚙️ Technologies Used

* Python 🐍
* NumPy
* Pandas
* Matplotlib / Seaborn
* Scikit-learn

---

## 🚀 How to Run

1. Clone the repository:

```
git clone https://github.com/TanveeSP/Cosmological-Data-Analysis.git
```

2. Navigate to project:

```
cd Cosmological-Data-Analysis
```

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Run notebooks:

```
jupyter notebook
```

---

## 📎 Notes

* Each subsection is implemented in a **separate notebook** for clarity
* Data is organized in the `/Data` folder
* Code is modular and easy to understand

---

## 👤 Author

* **Name:** Tanvee Sushama Paresh
* **GitHub:** [TanveeSP](https://github.com/TanveeSP)

---

## 💡 Conclusion

This project demonstrates how statistical methods and machine learning techniques can be applied to real-world astrophysical data to estimate fundamental constants of the universe.
