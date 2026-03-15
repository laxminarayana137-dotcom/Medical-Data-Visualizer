# Medical Data Visualizer

This project analyzes medical examination data and visualizes the relationships between different health indicators and cardiovascular disease using Python.

The project uses **Pandas, Matplotlib, and Seaborn** to process and visualize the data.

## Project Objective

The goal of this project is to explore how lifestyle factors and medical indicators relate to cardiovascular disease.

The dataset includes information such as:

* Age
* Height
* Weight
* Blood pressure
* Cholesterol level
* Glucose level
* Smoking habits
* Alcohol intake
* Physical activity
* Presence of cardiovascular disease

Using this data, we generate visualizations that help understand patterns and correlations.

---

## Technologies Used

* Python
* Pandas
* Matplotlib
* Seaborn
* NumPy

---

## Dataset

The dataset used in this project is:

`medical_examination.csv`

Each row represents a patient, and each column contains medical or lifestyle information.

---

## Features Implemented

### 1. BMI Calculation

A new column called **overweight** is added using BMI.

BMI formula:

BMI = weight (kg) / height² (m)

If BMI > 25 → overweight = 1
Otherwise → overweight = 0

---

### 2. Data Normalization

The following variables were normalized:

* cholesterol
* glucose

Values were converted to:

* 0 → normal
* 1 → above normal

---

### 3. Categorical Plot

A categorical plot is created showing the distribution of the following variables:

* cholesterol
* glucose
* smoking
* alcohol intake
* physical activity
* overweight

The chart compares patients **with and without cardiovascular disease**.

---

### 4. Heatmap

A heatmap is generated to visualize correlations between all health variables.

Before creating the heatmap, incorrect data was removed:

* Diastolic pressure greater than systolic pressure
* Extreme height values
* Extreme weight values

---

## Output Visualizations

The project produces:

1. **Categorical Plot**
2. **Correlation Heatmap**

These plots help understand which health factors may influence cardiovascular disease.

---

## How to Run

1. Install dependencies

```
pip install pandas matplotlib seaborn numpy
```

2. Run the project

```
python main.py
```

---

## Project Structure

```
├── medical_examination.csv
├── medical_data_visualizer.py
├── main.py
├── test_module.py
└── README.md
```

---

## Learning Outcome

This project demonstrates:

* Data cleaning
* Data transformation
* Feature engineering
* Data visualization
* Correlation analysis

It is part of the **FreeCodeCamp Data Analysis with Python Certification**.
