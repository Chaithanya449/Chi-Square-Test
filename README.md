# 📊 Chi-Square Test of Independence: Smart Device vs User Satisfaction

## 🧠 Project Objective

To determine whether there's a **significant relationship** between the **type of smart device used** (Smart Thermostat or Smartlight) and the **user's satisfaction level** using the **Chi-Square Test of Independence**.

---

## 📂 Dataset Description

The data contains:
- Two **categorical variables**:
  - **Device Type**: Smart Thermostat, Smartlight
  - **Satisfaction Level**: Very Satisfied, Satisfied, Neutral, Unsatisfied, Very Unsatisfied

It represents a contingency table with the frequency of user responses.

---

## ✅ Problem Statement

**Does the type of smart device impact user satisfaction?**

To answer this, we perform a **Chi-Square Test** to assess whether the distribution of satisfaction levels **differs** significantly across the two device types.

---

## 🧪 Statistical Approach

### ➤ Hypotheses:

- **Null Hypothesis (H₀):**  
  Satisfaction level is **independent** of device type.

- **Alternative Hypothesis (H₁):**  
  Satisfaction level is **dependent** on device type.

### ➤ Test Used:
- **Chi-Square Test of Independence** (`scipy.stats.chi2_contingency`)
- Evaluates whether the observed frequencies differ significantly from the expected frequencies.

---

## 📌 Key Steps in Code

1. **Data Setup**: Create a contingency table using pandas.
2. **Chi-Square Test**: Use `chi2_contingency` to get chi-square statistic, p-value, degrees of freedom, and expected frequencies.
3. **Decision Making**:
   - If **p-value > 0.05**: Fail to reject H₀ → No significant relationship.
   - If **p-value ≤ 0.05**: Reject H₀ → Significant relationship exists.

---

## 📈 Output 

- **Chi-square statistic**: *(e.g., 3.21)*  
- **p-value**: *(e.g., 0.52)*  
- **Conclusion**:  
  Since the p-value is greater than 0.05, we **fail to reject the null hypothesis**, indicating that **there is no significant relationship** between device type and user satisfaction level.

---

## 🛠️ Technologies Used

- Python 🐍
- Pandas 📊
- SciPy 🔬


---



