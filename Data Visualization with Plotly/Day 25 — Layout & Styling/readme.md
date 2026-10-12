# 📅 Day 25 — Layout & Styling

---

# 🎯 Objective

* আজকে শিখার লক্ষ্য হলো Plotly charts-এর **professional layout design & styling control**
* কীভাবে dashboard-like visualization তৈরি করা যায় তা শেখা
* problem solve করা হচ্ছে: **default chart UI simple → সেটাকে professional dashboard look বানানো**

---

# 📚 Topics Covered

* update_layout() usage
* Titles customization
* Axis styling
* Fonts & typography
* Themes (templates)
* Background styling
* Margins & spacing control

---

# 📁 Project Structure

```text id="p25s1"
Day 25 — Layout & Styling/
│── main.py
│── analysis.py
│── utils.py
│── data.csv
│── README.md
```

---

# 📊 Dataset

* File Name: `sales_data.csv`
* Description: Monthly sales and profit dataset for visualization

### Columns:

* month → Month name
* sales → Total sales
* profit → Total profit

---

# 💻 Code Breakdown (File by File)

---

## 📄 1. main.py

### 🔹 Purpose

* Basic sales line chart তৈরি করা
* layout update করা

### 🧾 Code

```python id="g9d1k1"
import pandas as pd
import plotly.express as px

df = pd.read_csv("sales_data.csv")

fig = px.line(df, x="month", y="sales", title="Sales Chart")

fig.update_layout(
    title="Updated Sales Layout"
)

fig.show()
```

### 🧠 Explanation

* Line 1 → pandas import করা হয়েছে data handling-এর জন্য
* Line 2 → Plotly Express import করা হয়েছে visualization-এর জন্য
* Line 4 → CSV data load করা হয়েছে
* Line 6 → line chart তৈরি করা হয়েছে
* Line 9 → layout modify করা হয়েছে
* Overall → basic dashboard-style chart তৈরি হচ্ছে

---

## 📄 2. analysis.py

### 🔹 Purpose

* axis, font, title customize করা
* chart readability improve করা

### 🧾 Code

```python id="g9d1k2"
fig = px.line(df, x="month", y="sales")

fig.update_layout(
    title={
        "text": "📊 Monthly Sales Report",
        "x": 0.5
    },
    xaxis_title="Months",
    yaxis_title="Sales",
    font=dict(size=14, color="black")
)

fig.show()
```

### 🧠 Explanation

* title center করা হয়েছে
* axis label add করা হয়েছে
* font styling দেওয়া হয়েছে
* overall → readable dashboard UI তৈরি হয়েছে

---

## 📄 3. utils.py (if any)

### 🔹 Purpose

* styling helper logic (optional reuse idea)

### 🧾 Code

```python id="g9d1k3"
def get_default_font():
    return dict(family="Arial", size=14, color="black")
```

### 🧠 Explanation

* reusable font configuration তৈরি করা হয়েছে
* multiple charts-এ same style ব্যবহার করা যাবে

---

# ⚙️ Implementation Flow

* Data load করা হয়েছে
* Basic chart তৈরি করা হয়েছে
* Layout customization করা হয়েছে
* Theme & font styling apply করা হয়েছে
* Final dashboard-style visualization তৈরি হয়েছে

---

# 📈 Output / Result

### Key findings:

* sales trend clearly visualized হয়েছে
* professional dashboard look পাওয়া গেছে
* chart readability significantly improved হয়েছে

---

# 🚀 What I Learned

* update_layout() এর power
* dashboard-level styling control
* fonts, titles, themes ব্যবহার করা

---

# 🧠 Key Concepts (Quick Revision)

* update_layout() → full chart styling control
* title customization → centered & formatted text
* template → ready-made themes
* font → typography control
* margin → spacing fix

---

# 📝 Notes

* good design = clean + readable + balanced
* too many colors/style করলে chart messy হয়
* dashboard UI should always be simple but informative

---

# 📌 Next Day Preview

* আগামী দিনে শিখবো:

  * Subplots & multi-chart dashboards
  * Advanced layout grid system
  * Multiple visualization in one figure

---

# ⭐ Bonus (Optional)

## 🔥 Improvements Ideas

* KPI dashboard design
* sales vs profit comparison layout
* dark mode dashboard UI

## 🧪 Practice Ideas

* finance dashboard design করা
* monthly report UI তৈরি করা
* company performance dashboard বানানো

---




# Author

## **Engr. Md Monjur Bakth Mazumder**

🎓 **Secondary School Certificate (SSC) from [Shah Helal High School](https://www.shahhelalhs.edu.bd/)**

🎓 **Diploma in Computer Science and Technology from [Moulvibazar Polytechnic Institute (MPI)](https://mpi.moulvibazar.gov.bd/)**

🎓 **BSc in Computer Science & Engineering (CSE)** _(Ongoing)_ **at [Sylhet International University (SIU)](https://siu.edu.bd/)**

---

## Support the Project

If you found this repository helpful, please consider giving it a **⭐ Star**. It helps others discover the project and motivates future development.

---


## Connect with Me

### Professional Profiles

| Platform | Link |
|:---|:---|
| Portfolio | [monjurmbm404.github.io](https://monjurmbm404.github.io) |
| GitHub | [monjurmbm404](https://github.com/monjurmbm404) |
| LinkedIn | [monjurmbm404](https://www.linkedin.com/in/monjurmbm404) |
| Medium | [@monjurmbm404](https://medium.com/@monjurmbm404) |

### Competitive Programming

| Platform | Link |
|:---|:---|
| Codeforces | [monjurmbm404](https://codeforces.com/profile/monjurmbm404) |
| CodeChef | [monjurmbm404](https://www.codechef.com/users/monjurmbm404) |
| LeetCode | [monjurmbm404](https://leetcode.com/u/monjurmbm404) |
| VJudge | [monjurmbm404](https://vjudge.net/user/monjurmbm404) |

### Social Media

| Platform | Link |
|:---|:---|
| Facebook | [monjurmbm404](https://www.facebook.com/monjurmbm404) |
| X (Twitter) | [@monjurmbm404](https://x.com/monjurmbm404) |
| YouTube | [@monjurmbm404](https://youtube.com/@monjurmbm404) |

### Contact Information

| Type | Email |
|:---|:---|
| Professional | [monjurmbm404@gmail.com](mailto:monjurmbm404@gmail.com) |

