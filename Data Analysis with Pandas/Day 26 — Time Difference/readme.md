# 📅 Day 26 — Time Difference

---

## 🎯 Objective

* Pandas এ time difference calculate করা শেখা
* `JoinDate` এবং `LeaveDate` দিয়ে work duration বের করা
* `timedelta` ব্যবহার করে time add/subtract করা
* real-world HR analytics (experience, tenure) তৈরি করা
* date-based business insights generate করা

---

## 📚 Topics Covered

* date subtraction (`-`)
* `timedelta`
* `.dt.days`
* work duration calculation
* time manipulation (add/subtract)
* experience level classification

---

## 📁 Project Structure

```id="d26proj"
day-26/
│── 01_date_subtraction.py
│── 02_days_difference.py
│── 03_timedelta_basic.py
│── 04_custom_timedelta.py
│── 05_real_world_duration.py
│── 06_project_style_analysis.py
│── data.csv
│── README.md
```

---

## 📊 Dataset

### 📄 File Name: data.csv

* **Description:** Employee join and leave date dataset

* **Columns:**

  * Name → employee name
  * JoinDate → joining date
  * LeaveDate → leaving date

👉 এই dataset ব্যবহার করে employee experience / tenure calculate করা হয়

---

# 💻 Code Breakdown (File by File)

---

## 📄 1. main.py (Concept Entry File)

### 🔹 Purpose

* time difference learning module start করা

### 🧾 Code

```python id="t26main"
print("Day 26 - Time Difference Learning")
```

### 🧠 Explanation

* simple starter file
* project initialization indicator

---

## 📄 2. 01_date_subtraction.py

### 🔹 Purpose

* two dates এর মধ্যে difference বের করা

### 🧾 Code

```python id="t26a"
df['Work_Duration'] = df['LeaveDate'] - df['JoinDate']
```

### 🧠 Explanation

* LeaveDate - JoinDate = total working duration
* result = timedelta object

---

## 📄 3. 02_days_difference.py

### 🔹 Purpose

* duration কে days এ convert করা

### 🧾 Code

```python id="t26b"
df['Days_Worked'] = df['Work_Duration'].dt.days
```

### 🧠 Explanation

* `.dt.days` → pure number of days
* HR analysis সহজ হয়

---

## 📄 4. 03_timedelta_basic.py

### 🔹 Purpose

* date add/subtract করা শেখা

### 🧾 Code

```python id="t26c"
df['After_30_Days'] = df['JoinDate'] + timedelta(days=30)
df['Before_10_Days'] = df['JoinDate'] - timedelta(days=10)
```

### 🧠 Explanation

* `timedelta` → time manipulation tool
* future/past date calculate করা যায়

---

## 📄 5. 04_custom_timedelta.py

### 🔹 Purpose

* business-level time estimation

### 🧾 Code

```python id="t26d"
df['After_1_Year'] = df['JoinDate'] + timedelta(days=365)
df['After_6_Months'] = df['JoinDate'] + timedelta(days=180)
```

### 🧠 Explanation

* yearly/monthly projection করা যায়
* planning & forecasting use case

---

## 📄 6. 05_real_world_duration.py

### 🔹 Purpose

* HR analytics style duration analysis

### 🧾 Code

```python id="t26e"
df['Days_Worked'] = (df['LeaveDate'] - df['JoinDate']).dt.days
df['Months_Worked'] = df['Days_Worked'] / 30
```

### 🧠 Explanation

* days → months conversion
* longest working employee identify করা যায়

---

## 📄 7. 06_project_style_analysis.py

### 🔹 Purpose

* real-world HR classification system

### 🧾 Code

```python id="t26f"
df['Experience_Level'] = df['Days_Worked'].apply(
    lambda x: "Senior" if x > 700 else ("Mid" if x > 300 else "Junior")
)
```

### 🧠 Explanation

* experience category তৈরি করা হয়
* business decision making support করে

---

## ⚙️ Implementation Flow

* dataset load করা হয়েছে
* date string → datetime convert করা হয়েছে
* time difference calculate করা হয়েছে
* days & months conversion করা হয়েছে
* timedelta দিয়ে date manipulation করা হয়েছে
* HR insights তৈরি করা হয়েছে

---

## 📈 Output / Result

* employee work duration বের হয়েছে
* experience level classification হয়েছে
* longest serving employee identify হয়েছে
* HR analytics report তৈরি হয়েছে

---

## 🚀 What I Learned

* time difference = core HR analytics concept
* datetime subtraction → timedelta result দেয়
* `.dt.days` → numeric conversion
* timedelta → time add/subtract tool
* real-world experience calculation possible

---

## 🧠 Key Concepts (Quick Revision)

* `date1 - date2` → duration
* `.dt.days` → number of days
* `timedelta(days=n)` → time shift
* experience = business logic based on time
* HR analytics = time-based insights

---

## 📝 Notes

* date format must be datetime before subtraction
* timedelta is very important in forecasting
* experience calculation is rule-based (not fixed)

---

## 📌 Next Day Preview

👉 Day 27 — Time Series Advanced

* rolling mean
* resample
* moving average
* trend analysis
* time-based forecasting basics

---

## ⭐ Bonus

### 🔥 Improvements Ideas

* employee retention analysis system
* attrition prediction dataset

### 🧪 Practice Ideas

* try different experience rules
* calculate tenure in years/months accurately
* build employee lifecycle tracker

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

