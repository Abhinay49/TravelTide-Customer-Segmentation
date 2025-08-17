# TravelTide Customer Segmentation Project

## 📌 Overview
This project was completed as part of the **TravelTide Mastery Project**, following the **CRISP-DM** methodology.  
The objective was to segment customers of **TravelTide**, an online travel startup, to support the design of a **personalized rewards program**.  

By analyzing customer behavior across sessions, flights, and hotels, the project identifies meaningful customer groups and aligns them with reward program perks proposed by **Elena Tarrant, Head of Marketing**.  

---

## 🎯 Business Objective
- Understand customer behavior and preferences.  
- Identify distinct customer segments using data-driven methods.  
- Map each segment to the most relevant **reward program perk**.  
- Provide **actionable recommendations** to improve retention and engagement.  

---

## 📂 Project Structure
```
TravelTide-Customer-Segmentation/
│
├── data/
│   ├── Raw/               # Extracted raw data
│   ├── Processed/         # Cleaned and preprocessed datasets
│
├── notebooks/             # Jupyter/Colab notebooks for analysis
├── output/                # Cluster profiling, visualizations, PCA outputs
├── reports/               # Executive summary, stakeholder slides
│
├── README.md              # Project documentation
└── requirements.txt       # Dependencies (optional)
```

---

## ⚙️ Methodology (CRISP-DM)
1. **Business Understanding** – Align segmentation with TravelTide’s rewards program strategy.  
2. **Data Understanding** – Explore relational database (users, sessions, flights, hotels). Identify anomalies (duplicate sessions, invalid hotel nights).  
3. **Data Preparation** – Clean and filter data, define user cohorts, handle outliers, scale features.  
4. **Feature Engineering** – Derive behavioral metrics (rebooking ratio, co-booking ratio, dollars saved per km, etc.), aggregated at the **user level**.  
5. **Modeling (Customer Segmentation)** – Apply **KMeans clustering** with PCA. Iterated across multiple values of `k`. Evaluated with **silhouette scores** and interpretability.  
6. **Evaluation** – Validate clusters against hypothesized perk behaviors. Ensure alignment with marketing strategy.  
7. **Deployment (Communication)** – Deliver **executive summary** and **stakeholder slide deck** with visuals (heatmaps, radar charts).  

---

## 📊 Key Findings
- Identified **7 distinct customer segments** (Iteration 4, k=7).  
- Segments showed clear differences in **spend, booking type, rebooking, discount sensitivity, and engagement**.  
- Each segment was assigned a **personalized perk** (e.g., *Free Checked Bag*, *No Cancellation Fees*, *Exclusive Discounts*).  
- Results validated some of Elena’s hypotheses while also surfacing **new behavioral patterns**.  

---

## 🎁 Perk Mapping (Final Segments)
| Cluster | Segment Name                          | Assigned Perk                          |
|---------|---------------------------------------|-----------------------------------------|
| 0       | Deal-Seeking Co-Bookers               | 💰 Exclusive Discounts                  |
| 1       | Inactive / Idle Users                 | 🥘 Free Hotel Meal                      |
| 2       | Affluent Hotel Travelers              | 🥞 Complimentary Daily Breakfast        |
| 3       | Family Leisure Vacationers (Hotel-Only) | 🧼 Free Mid-Stay Housekeeping          |
| 4       | Rebooking-Prone Solo Fliers           | ❌ No Cancellation Fees                 |
| 5       | Loyal High-Value Travelers            | ✈️ 1 Night Free Hotel + Flight          |
| 6       | Stable Frequent Fliers                | 🧳 Free Checked Bag                     |

---

## 📑 Reports & Deliverables
- [Executive Summary](reports/Executive%20Summary%20for%20TravelTide%20Customer%20Segmentation.docx)  
- [Stakeholder Presentation](reports/TravelTide_Customer_Segmentation_ABHINAY_DORNIPATI_FINAL_Presentation.pptx)  
- [Cluster Profiling Summary](output/cluster_summary_k7_updated.csv)  
- [Full Feature Dataset with Cluster Labels](output/df_true_cluster_k7.csv)  

---

## 🚀 Next Steps
- Track **segment performance** after perks rollout.  
- Re-cluster periodically as new data accumulates.  
- Explore additional **personalization strategies** (dynamic perks, hybrid offers).  

---

## 🛠️ Tools & Technologies
- **SQL (PostgreSQL)** – data extraction & cohorting  
- **Python (pandas, scikit-learn, matplotlib)** – preprocessing, clustering, visualization  
- **Colab/Jupyter** – analysis workflow  
- **PowerPoint / Word** – business communication deliverables  

---

## 📬 Author
**Abhinay Dornipati**  
TravelTide Mastery Project – Customer Segmentation  
