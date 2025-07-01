# 📈 Adani Energy Solutions Limited Stock Dataset

![Stock Market](https://img.shields.io/badge/Data-Finance-blue) 
![Pandas](https://img.shields.io/badge/Tool-Pandas-green) 
![Updated](https://img.shields.io/badge/Updated-July_2024-orange)

> "Historical OHLC, Volume, and Market Cap data for Adani Energy Solutions (NSE:ADANIENSOL) - India's power transmission leader."

---

## 🏦 **Dataset Overview**
This dataset tracks **Adani Energy Solutions Ltd** (formerly Adani Transmission), a critical player in India's energy infrastructure. Ideal for:
- **Algorithmic trading** backtesting
- **Technical/fundamental** analysis
- **Energy sector** research

### 🔑 **Key Features**
| Feature          | Detail                          |
|------------------|---------------------------------|
| **Time Period**  | [YYYY] - Present                |
| **Frequency**    | Daily                           |
| **Metrics**      | OHLC, Volume, Market Cap        |
| **Currency**     | INR (₹)                        |

---

## 📊 **Dataset Structure**
### **Columns & Data Types**
| Column            | Type       | Description                | Example        |
|-------------------|------------|----------------------------|----------------|
| 📅 **Date**       | `datetime` | Trading date               | `2024-07-01`   |
| 🟢 **Open**       | `float64`  | Opening price (₹)          | `1025.50`      |
| 🔺 **High**       | `float64`  | Daily high (₹)             | `1050.75`      |
| 🔻 **Low**        | `float64`  | Daily low (₹)              | `1012.30`      |
| 🟣 **Close**      | `float64`  | Closing price (₹)          | `1045.20`      |
| 🔊 **Volume**     | `int64`    | Shares traded              | `1,500,000`    |
| 💰 **Mkt Cap**    | `float64`  | Market Cap (₹ Crores)      | `120,000.50`   |

---

## 🧹 **Data Cleaning Guide**
```python
import pandas as pd

# Load data
df = pd.read_csv("adani_stock_data.csv")

# Fix dates
df['Date'] = pd.to_datetime(df['Date'], format='%d-%m-%Y')

#Replace Commas
for i in ad.iloc[:,2:].select_dtypes(include="object").columns:
  ad[i]=ad[i].apply(lambda x:float(x.replace(",","")))

#💡 Domain Insights
#🚀 Key Stock Drivers
Policy Impact: Renewable energy subsidies & grid reforms
Debt Profile: High capex projects (~70% D/E ratio)
Adani Group Sentiment: Hindenburg report aftermath

#🔗 Resources
Resource Type	Link
Live Data	Yahoo Finance
Company Info	Adani Energy Solutions
Pandas Guide	Official Docs
