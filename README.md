# RESTAURANT-RECOMMENDATION-ML-MODEL

🙋‍♂️ **Author**
Reuben Thomas John

Intern @ Cognifyz Technologies

📅 **Project Duration:** 4 Weeks

---

## 🧠 TASK - 2: Content-Based Restaurant Recommendation System

This project builds a **Content-Based Filtering Recommendation System** that suggests top restaurants to users based on their preferences for **cuisine, price range, and rating**. The system uses restaurant data to match user input with the most similar restaurants using manually defined similarity rules.

---

## 📌 Objective

To recommend the **Top 5 restaurants** based on user preferences using a simple yet effective rule-based similarity system.

### 🎯 User Inputs Considered:

* Preferred **Cuisines**
* Desired **Price Range**
* Minimum **Aggregate Rating**

---

## 🧾 Dataset Overview

* 📂 **Total Records:** 9,551

* 🏷️ **Columns:** 21

* 📊 **Sample Features:**

  * Restaurant Name
  * Cuisines
  * Price Range
  * Aggregate Rating
  * Votes
  * Locality & Address
  * Delivery & Booking Availability

* 🧹 **Preprocessing**:

  * Missing values filled using **mean** (for numbers) and **mode** (for categories).
  * Categorical variables encoded using **LabelEncoder**.

---

## 🛠️ Technologies & Tools Used

* Python
* Google Colab
* Pandas, NumPy
* Scikit-learn
* Seaborn, Matplotlib

---

## 🔄 Recommendation Logic

### ✅ Approach: Manual Content-Based Filtering

The algorithm calculates a **similarity score** for each restaurant by comparing:

* **Cuisines** (exact match = +3 points)
* **Price Range** (closer range = higher score)
* **Aggregate Rating** (closer = better)

### 🏆 Top 5 results are selected based on highest similarity scores.

---

## 🔍 Key Highlights

* Simple, interpretable logic without requiring heavy machine learning models.
* Fast and flexible for small datasets.
* Supports **custom user preferences** directly via a dictionary.

---

## ✨ Sample Output

```text
Top 5 Restaurant Recommendations:

 Restaurant Name     Cuisines  Price range  Avg Cost for two  Aggregate rating  Votes  similarity_score
Izakaya Kikufuji     Japanese          3           1200             4.5           591           8.0
Kuuraku              Japanese          3           1250             3.9           106           7.0
Soho Hibachi         Japanese          1             10             4.3           116           7.0
Tamura               Japanese          3           1500             3.5           163           7.0
3 Wise Monkeys       Japanese          3         450000             4.2           395           7.0
```

---

## 📦 Requirements

Install the required libraries using:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## 🚀 How to Run

1. 📂 Upload the dataset to your Google Drive
2. 🔗 Mount Google Drive in Colab
3. ▶️ Run the cells in order
4. 🧾 Edit `user_preferences` dictionary with your desired inputs
5. 📊 View the top 5 personalized restaurant recommendations!

---

## ✅ Future Improvements

* Use **vectorized** similarity with cosine distance
* Build a **hybrid model** combining user-based & content-based filtering
* Add **user profiles** and **feedback loop**
