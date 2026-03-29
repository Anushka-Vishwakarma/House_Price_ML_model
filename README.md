# 🏠 House Price Prediction (Preprocessing Pipeline)

## 📌 Project Overview
This project focuses on building a data preprocessing pipeline for a house price prediction model using real-world Indian real estate data.

The dataset contains semi-structured data (text + numeric), requiring extensive cleaning and transformation before model training.

---

## 🎯 Objective
To clean, transform, and prepare raw housing data for machine learning models.

---

## 📊 Dataset Description
The dataset includes features such as:

- Location  
- Carpet Area  
- Floor details  
- Furnishing status  
- Ownership  
- Parking  
- Property views (Park, Road, Pool)  

⚠️ The dataset contains:
- Mixed formats (e.g., "1.42 Cr", "849 sqft")
- Missing values
- Text-based categorical data

---

## 🛠️ Data Preprocessing Steps

### 1. Data Cleaning
- Converted price values:
  - "1.42 Cr" → 14200000
- Extracted numeric values using regex:
  - "849 sqft" → 849

### 2. Feature Engineering
- Extracted:
  - `Floor_No` and `Total_Floors`
  - `Is_Basement`
- Created new features:
  - `Parking_Count`
  - `Park_View`, `Road_View`, `Pool_View`

### 3. Handling Missing Values
- Filled numerical columns using median
- Replaced categorical null values with "Unknown"

### 4. Encoding
- One-hot encoding for:
  - Location
  - Facing
  - Ownership
- Label encoding for:
  - Furnishing

---

## 📂 Project Structure

