# 🏥 Hospital Demand Forecasting App

## 👨‍💻 Completed By: Rajeev Nair

## 📌 Overview
This Django web application allows hospital administrators to:
- Upload weekly hospital supply demand data (`.xlsx` format)
- Forecast usage using **Random Forest Regressor**
- Compare **Actual vs Predicted** demand (Weeks 149–156)
- Forecast the next **8 future weeks** (Weeks 157–164)
- View **MAPE**, **RMSE**, and **MAE** metrics
- Visualize results with graphs and tables

---

## ✅ Features
- Upload Excel files with multiple features
- Random Forest-based demand prediction
- Future forecasting with simulated input
- Responsive table + chart output
- Clean UI with error handling

---

## 🗂️ Data Format (Excel)
| Column Name        | Description                                |
|--------------------|--------------------------------------------|
| Item_Code          | Unique item code                           |
| Item_Description   | Name of the item                           |
| Patient_Footfall   | Number of patients for the week            |
| Last_Week_Usage    | Previous week's quantity used              |
| Public_Holiday     | Binary (1 = holiday, 0 = no holiday)       |
| Rain_Impact        | Binary (1 = rain affected, 0 = not)        |
| Quantity_Used      | Actual demand used in that week            |

---

## ⚙️ How to Run the Project

```bash
git clone https://github.com/rajeev27-sudo/Odin-Technical-Assessment.git
cd Odin-Technical-Assessment
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
