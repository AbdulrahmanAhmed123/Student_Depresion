# Student_Depresion
# 🎓 Student Depression Analysis & Cleaning Project

اهلا بيك في المشروع دا! هنا إحنا بنعمل **Data Preparation & Cleaning** لـ Dataset خاصة باكتئاب الطلاب (`student_depression_dataset.csv`). الهدف الأساسي هو تجهيز البيانات وتنظيفها عشان تكون جاهزة للـ Analysis والـ Machine Learning.

---

## 📌 Project Overview
المشروع عبارة عن **Jupyter Notebook** مبني على خطوات منظمة جداً للتعامل مع البيانات الواقعية (Real-world Data) بكل ما فيها من مشاكل أو Missing values أو قيم غريبة.

### 🛠️ Tech Stack & Libraries Used
إحنا استخدمنا أقوى مكتبات الـ Data Science في Python:
*   **Pandas & NumPy:** عشان الـ Data Manipulation والـ Cleaning.
*   **Matplotlib, Seaborn, & Plotly:** لتجهيز الـ Visualizations والرسومات البيانية.

---

## 📂 Data Structure & Features
الـ Dataset دي فيها **27,901 صف** و **18 عمود**، وبتغطي تفاصيل مهمة جداً عن حياة الطلاب زي:
*   `Age`, `Gender`, `City`, `Degree` (البيانات الديموغرافية).
*   `Academic Pressure`, `CGPA`, `Study Satisfaction` (الجانب الأكاديمي).
*   `Sleep Duration`, `Dietary Habits`, `Work/Study Hours` (أسلوب الحياة).
*   `Financial Stress`, `Family History of Mental Illness`.
*   `Depression` & `Suicidal thoughts` (**Target Columns**).

---

## 🔧 Data Cleaning Steps (ماذا فعلنا في الكود؟)

المشروع ركز بشكل كبير على الـ **Data Cleaning** وحل مشاكل الـ Structural Errors اللي ظهرت بعد الـ Inspection:

1. **Financial Stress Column:** 
   * كان فيه قيم غريبة عبارة عن علامات استفهام `?`.
   * عملنا ليها **Drop** وحولنا العمود بالكامل لـ `int` عشان يبقى قيم رقمية صحيحة ونقدر نستخدمه صح.
2. **Work/Study Hours Column:**
   * حولنا الـ Dtype بتاعه من `float` لـ `int` عشان الساعات تكون أرقام صحيحة منطقية.
3. **City Column:**
   * اكتشفنا قيم عشوائية ومش منطقية في عمود المدن (زي ظهور رقم `3.0` مكان اسم المدينة!).
   * شلنا الصفوف دي تماماً (**Data Filtering**) عشان نحافظ على الـ Data Quality.

---

## 📊 Summary Statistics Quick Look
بعد التنظيف، دي نظرة سريعة على الـ Data Insights:
*   **Age Range:** الطلاب في العينة أعمارهم بتتروح من **18 لـ 59 سنة**، بمتوسط عمر حوالي **25 سنة**.
*   **Financial Stress:** المتوسط العام للضغط المادي واصل لـ **3.1 من 5**، ودا مؤشر مهم جداً.
*   **Depression Rate:** حوالي **58%** من الحالات اللي في الـ Dataset متسجل عندها Depression (مؤشر يحتاج دراسة وتحليل عميق).

---

## 🚀 How to Run
1. اعمل Clone للـ Repository.
2. اتأكد من تحميل الـ Dataset في نفس الفولدر باسم `student_depression_dataset.csv`.
3. افتح الـ Notebook وعيش مع الكود! 

> **Note:** تقدر تفتح المشروع مباشرة على Google Colab من خلال الـ Badge الموجودة فوق خالص في الـ Notebook! 🚀
