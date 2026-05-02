# SOC-Calculator
LFP battery state of Charge calculator 
# 🔋 LFP Battery SOC Calculator

A professional **LFP (Lithium Iron Phosphate) Battery State of Charge Calculator** with a modern **motorcycle / EV cluster style dashboard** interface.

This project calculates battery **SOC (%)** using battery voltage and number of cells with an accurate **OCV interpolation method**.

---

## 🚀 Features

✅ Accurate LFP SOC calculation using voltage lookup table  
✅ Supports custom battery cell count (Ex: 8S / 16S / 24S)  
✅ Motorcycle / EV digital cluster UI  
✅ Animated analog gauge needle  
✅ Full dark premium theme  
✅ LOW / MEDIUM / FULL battery status  
✅ Voltage live display  
✅ Responsive design (Desktop + Mobile)

---

## 📸 Preview

<img width="1366" height="605" alt="Screenshot from 2026-05-02 14-53-46" src="https://github.com/user-attachments/assets/eff7983c-5aa7-4867-aa48-497825393e42" />


---

## ⚙️ How It Works

The calculator uses **Open Circuit Voltage (OCV)** method.

Voltage is compared with predefined LFP battery voltage table:

| Cell Voltage (mV) | DOD |
|------------|------|
| 3400 | 0 |
| 3350 | 1 |
| 3325 | 10 |
| 3300 | 30 |
| 3275 | 60 |
| 3250 | 70 |
| 3225 | 80 |
| 3200 | 83 |
| 3125 | 86 |
| 3000 | 91 |
| 2600 | 100 |

Then:

SOC = 100 - DOD

---

## 🖥️ Usage

1. Enter number of cells  
2. Enter battery pack voltage  
3. Click **CALCULATE**  
4. View SOC on analog gauge + digital display

Example:

```text
Cells: 16
Voltage: 52.80V
Result: SOC = 72%
