# Customer-Shopping-Behavior-Analysis


📌 Project Overview :
This project analyses customer shopping behaviour using transactional data from 3,900 purchases. The goal is to uncover patterns in spending, customer segments, product preferences, and subscription behaviour to drive data‑informed business strategies.

❓ Problem Statement:  
Businesses often lack a clear understanding of ‘who’ their high‑value customers are, ‘what’ drives purchases, and ‘how’ marketing efforts can be optimized. Without structured analysis, opportunities to increase revenue, improve loyalty, and fine‑tune discount strategies are missed.

📊 Dataset Info :
- Rows: 3,900  
- Columns: 18  
- Key fields: Demographics (age, gender, location), purchase details (item, category, amount), behavioural data (subscription status, shipping type, discount usage, review rating)  
- Missing values: 37 in `Review Rating` – imputed with median per category

 🛠️ Tech Stack:
- Python (Pandas, Jupyter Notebook) – Data cleaning, feature engineering, EDA  
- PostgreSQL – Structured querying for business insights  
- Power BI – Interactive dashboard creation
- Gamma AI – Prepare presentation
- GitHub – Version control and project sharing

 🔁 Workflow (Python  → SQL → Power BI → Gamma AI → GitHub)  

1. Python (Jupyter Notebook)  
   - Loaded raw CSV, inspected structure and missing values  
   - Imputed missing review ratings using category median  
   - Standardized column names, created `age_group` and `purchase_frequency_days`  
   - Removed redundant `promo_code_used` (identical to `discount_applied`)  
   - Loaded cleaned data into PostgreSQL  

2. SQL (PostgreSQL)  
   - Ran 10 analytical queries to answer key business questions:  
     - Revenue by gender  
     - High‑spending discount users  
     - Top‑rated products  
     - Shipping type comparison  
     - Subscriber vs. non‑subscriber spend  
     - Products with highest discount dependency  
     - Customer segmentation (New / Returning / Loyal)  
     - Top 3 products per category  
     - Repeat buyers & subscription correlation  
     - Revenue by age group  

3. Power BI  
   - Connected to PostgreSQL (or used exported data)  
   - Built an interactive dashboard with slicers and visualizations  

 ✨ Key Features  
- Data Cleaning & Feature Engineering – Automated handling of missing values, creation of derived columns  
- SQL Analysis – Structured queries answering real‑world business questions  
- Interactive Dashboard – Dynamic filters (subscription, gender, category, shipping type) allow stakeholders to explore data on their own  

 📈 Insights  
- Subscribers spend 68% more per transaction, yet only 27% of customers subscribe → huge opportunity to boost subscriptions  
- Express shipping customers spend 12% more than standard shipping users → consider premium shipping offers  
- 5 products (Hat, Sneakers, Coat, Sweater, Pants) have >47% discount‑dependent purchases → margin risk  
- Middle‑aged and Senior customers contribute the highest revenue → target them with relevant products  
- Top‑rated products (Blouse, Dress, Shirt) should be featured in campaigns  
- Loyal customers (previous purchases >10) are only 15% of customers but likely drive high revenue – retention is key  

 📸 Poster and Screenshot:

![Dashboard Preview](https://github.com/dee8864/Customer-Shopping-Behavior-Analysis/blob/main/CUSTOMER%20BEHAVIOUR%20DASHBOARD%20POSTER.png)
![Dashboard Preview](https://github.com/dee8864/Customer-Shopping-Behavior-Analysis/blob/main/CUSTOMER%20BEHAVIOUR%20DASHBOARD%20PICTURE.png)
