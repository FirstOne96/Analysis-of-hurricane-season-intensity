# 🌩️ StormIndex Regression Analysis

## Overview

This project explores the dependence of **StormIndex** — a variable reflecting storm activity — on various climatic and environmental factors using **linear regression modeling**. The goal was to identify which variables significantly influence storm severity, with a special focus on the interaction between **El Niño phases** and the number of **hurricanes**.

The analysis is part of a university project for the course on **Applied Statistics**.

---

## 📊 Dataset

The dataset `ex1028` contains annual climate records with the following key variables:

- `StormIndex`: Target variable indicating the intensity of storm activity.
- `ElNino`: Categorical variable with levels: *cold*, *neutral*, *warm*.
- `Hurricanes`: Number of hurricanes in the year.
- `WestAfrica`: Index of West African climate activity.
- `Storms`: Number of storms.
- `Temperature`: Global average temperature.
- `Year`: Observation year.

---

## 🔍 Objectives

- Build a linear regression model to explain StormIndex using climatic variables.
- Analyze the interaction between El Niño phases and hurricane counts.
- Evaluate model assumptions and assess predictor significance.

---

## ✅ Key Findings

- **Hurricanes** significantly increase the StormIndex.
- **ElNino** modifies the effect of hurricanes:
  - In *neutral* and *warm* years, hurricanes have a **weaker effect**.
- **WestAfrica** index is a significant positive predictor.
- The **Temperature** variable was excluded due to multicollinearity.
- Assumptions of linear regression (normality, homoscedasticity, independence) were all **satisfied**.

---

## 📈 Statistical Tests

- **Shapiro-Wilk** test: Residuals are normally distributed (p = 0.8611).
- **Breusch-Pagan** test: No heteroscedasticity detected (p = 0.187).
- **Durbin-Watson** test: No autocorrelation (p = 0.461).
- **Multicollinearity**: Detected for `Temperature` and interaction terms; variable removed.

---

## 📦 Requirements

- R version ≥ 4.1
- R packages:
  - `Sleuth2`
  - `ggplot2`
  - `car`
  - `lmtest`
  - `performance`
  - `dplyr`
