# Skillytixs_internship-tasks

# 🩺 Medical Appointment No-Shows – Data Cleaning & Preprocessing

## 📌 Overview
This project focuses on **cleaning and preparing the Medical Appointment No Shows dataset** for analysis.  
The raw dataset had multiple issues such as inconsistent column names, missing or incorrect values, and unstandardized categorical data.  

Using **Python (Pandas)**, the dataset was preprocessed and transformed into an analysis-ready format.

---

## 📂 Dataset
- **Source**: Kaggle – *Medical Appointment No Shows*  
- **Rows**: 110,527  
- **Columns**: 14  

### 🔑 Key Features:
- `PatientID`, `AppointmentID`  
- `Gender`, `Age`, `Neighbourhood`  
- `ScheduledDay`, `AppointmentDay`  
- `Scholarship`, `Hypertension`, `Diabetes`, `Alcoholism`, `Handicap`, `SMS_received`  
- `No-show`  

---

## 🛠️ Cleaning Steps
1. **Column Standardization**  
   - Converted all column names to lowercase.  
   - Replaced spaces with underscores.  
   - Fixed typos: `hipertension → hypertension`, `handcap → handicap`.  

2. **Date Conversion**  
   - Converted `scheduledday` and `appointmentday` to proper datetime format.  

3. **Age Cleaning**  
   - Removed negative and unrealistic ages.  
   - Verified statistics (`min`, `max`, `mean`).  

4. **Duplicate Removal**  
   - Checked and confirmed **no duplicate rows** exist.  

5. **Gender Standardization**  
   - Replaced `F/M` with `Female/Male`.  

6. **No-show Column Update**  
   - Clarified labels as `Showed Up` and `No Show`.  

7. **Binary Column Verification**  
   - Ensured binary values (`0/1`) for:  
     `Scholarship, Hypertension, Diabetes, Alcoholism, Handicap, SMS_received`.  

8. **Neighbourhood Cleaning**  
   - Converted all values to lowercase.  
   - Removed accents and extra spaces.  

9. **Final Verification**  
   - Checked missing values.  
   - Validated data types.  
   - Reviewed sample data.  

---

## 📦 Deliverables
- `cleaned_medical_appointments.csv` → Cleaned dataset  
- `data_cleaning.ipynb` → Python notebook with preprocessing code  
- `screenshots/` → Optional verification screenshots  

---

## ✅ Outcome
The **cleaned dataset** is now ready for:
- Patient no-show prediction  
- Neighborhood-based attendance analysis  
- Health condition impact analysis (Diabetes, Hypertension, etc.)  
- Visualizations of age, gender, and appointment patterns  

---

## 🧾 Note
All preprocessing steps were carefully **documented and verified** to ensure **reliability and reproducibility**.  
This makes the dataset suitable for **further analysis, machine learning models, and reporting**.  
