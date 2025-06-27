# Maternal Health Data Analysis Using Excel

## 📊 Dataset Overview
- **Sample size**: 100 maternal health records

### **Key Variables:**
- `Region`, `Age`, `Parity`
- `ANC_Visits` (Antenatal Care)
- `Vaccinated_TT` (Tetanus Toxoid vaccine status)
- `Hb_Level` (Hemoglobin level)
- `Complication`, `Delivery_At_Facility`
- `Birth_Weight_kg`

---

## 🔍 Derived Variables (Created Using Excel Formulas)

| Column         | Logic Description                                                                 |
|----------------|------------------------------------------------------------------------------------|
| **Anemia_Status** | Flagged as “Anemia” if `Hb_Level < 11.0 g/dL` (WHO cutoff), else “Normal”        |
| **High_Risk**      | “Yes” if `Age < 18 or > 35`, or `Parity ≥ 4`, or `ANC_Visits < 4`                 |
| **Low_BW_Flag**    | “Yes” if `Birth_Weight_kg < 2.5 kg`                                               |
| **Critical_Risk**  | “Yes” if High Risk **and** (Not Vaccinated **or** Low Birth Weight baby)        |

💡 These logical features were created using Excel’s `IF`, `AND`, and `OR` functions.

---

## 🛠️ Tools Used
- **Microsoft Excel**: Data cleaning, formula logic, pivot tables, and visualizations  
- **Canva (planned)**: For summary infographic

---

## 📈 Key Findings 
- X% of women were anemic  
- Y% were identified as high-risk pregnancies  
- Z% delivered at health facilities  
- N% flagged as critical risk using custom logic

---

## 🌍 Impact
This type of logical, Excel-based maternal risk flagging could be easily replicated in low-resource settings for early detection and prioritization of high-risk pregnancies.
