# Indian-kids-Screentime-2025-
Analyzing Indian kids' screen time patterns by age, gender, location, device &amp; activity using Python, Seaborn, and Power BI | 9,668 records | 8-week data visualization project
![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C72B0?style=flat)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=flat&logo=powerbi&logoColor=black)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)
![Records](https://img.shields.io/badge/Records-9%2C668-blue?style=flat)

> Analyzing Indian kids' screen time patterns to uncover trends by **age, gender, location type (urban/rural), device type, and activity category** using Python and Power BI. Built to present clear, actionable insights for parents, educators, and policymakers.

---

## 📌 Project Overview

**ScreenSense** is an 8-week end-to-end data visualization project based on the Indian Kids Screentime 2025 dataset from Kaggle. The project covers the full data science pipeline — from raw data ingestion and cleaning, through exploratory analysis and cohort segmentation, to an interactive Power BI dashboard and final presentation.

| | |
|---|---|
| **Dataset** | [Indian Kids Screentime 2025 — Kaggle](https://www.kaggle.com/datasets/ankushpanday2/indian-kids-screentime-2025) |
| **Records** | 9,668 rows × 17 columns |
| **Age Range** | 8–18 years (3 bands: children, young teens, teens) |
| **Location** | Urban (70.4%) and Rural (29.6%) |

---

## 🔑 Key Findings

| Metric | Value | Insight |
|--------|-------|---------|
| Avg daily screen time | **4.37 hr/day** | More than 2× the WHO guideline |
| Exceeded recommended limit | **85.8%** | Nearly every child is overexposed |
| Kids with health issue | **67.1%** | 2 in 3 kids report at least one health impact |
| Avg edu:rec ratio | **0.43** | Less than half of usage is educational |
| Weekend avg screen time | **5.61 hr/day** | 85% higher than weekdays (3.03 hr) |
| Kids exceeding limit on weekends | **100%** | Every single child — zero exceptions |

---

## 📊 Sample Insights by Week

### Week 3 — Univariate & Bivariate Analysis
- Most kids spend **5–6 hours daily** on screens; peak usage is around 5 hours
- **Smartphone** is the most commonly used device (47%), followed by TV (25.6%)
- Median screen time is similar for both males and females (~4 hours) — **screen time is gender-neutral**
- Kids **with health issues** have higher median screen time than those without

### Week 4 — Devices & Weekday/Weekend
- Smartphones dominate across all age groups, genders, and locations
- Recreational usage is the **primary activity type** across the entire dataset
- Users spend **significantly more** time on screens during weekends than weekdays
- Urban users show higher device usage overall; rural users have relatively higher TV dependency

### Week 5 — Cohort Analysis (Heatmaps)
- **Age × Device**: Young teens (13–15) on TV show the highest average usage (4.57 hr/day)
- **Gender × Activity**: Both genders show nearly identical recreational patterns
- **Location × Device**: Smartphones dominate urban areas; TV more prevalent in rural
- **Age × Weekday flag**: All age groups spike on weekends; children (8–12) show the steepest jump (+154%)

### Week 6 — Habit Patterns & Segment Insights
- Screen time is higher on weekends — users have more free time for recreational usage
- Young teens (13–15) have relatively higher median screen time
- Children (8–12) show greater variation with several high outliers
- Urban users have more high screen-time values; rural patterns are more consistent
- Older teens (16–18) use laptops more frequently than younger groups

---

## 🩺 Health Impact Analysis

The dataset reveals a clear **dose-response relationship** between screen time and health outcomes:

| Screen Time Category | % with Health Issue |
|----------------------|---------------------|
| 0–2 hr/day (Low) | **0%** — zero health issues |
| 3–8 hr/day (Moderate) | **72.9%** |
| 9–14 hr/day (High) | **82.3%** |

> **Critical finding:** Teens aged 16–18 in the high usage category show an **85.7% health issue rate** — the worst outcome in the dataset.

---

## 🗂️ Project Structure

```
screensense-kids-screentime/
│
├── notebooks/
│   ├── week1_data_setup.ipynb          # Data loading, schema, nulls, cleaning
│   ├── week2_3_preprocessing.ipynb     # Feature engineering, derived columns
│   ├── week3_univariate_bivariate.ipynb # Distributions, boxplots, comparisons
│   ├── week4_devices_weekday.ipynb     # Device mix, activity, weekday/weekend
│   ├── week5_cohort_analysis.ipynb     # Heatmaps, stacked comparisons
│   └── week6_habit_patterns.ipynb      # Segment insights, habit patterns
│
├── data/
│   ├── README.md                       # Dataset source and download instructions
│   └── cleaned_Indian_Kids_Screen_Time.csv
│
├── dashboard/
│   └── Kids_Screen_Time_Analysis_Dashboard.pbix
│
├── report/
│   ├── ScreenSense_Final_Report.pdf
│   └── ScreenSense_Final_Presentation.pptx
│
├── visuals/                            # Dashboard screenshots
│   ├── page1_overview.png
│   ├── page2_demographics.png
│   ├── page3_devices_time.png
│   └── page4_health_cohorts.png
│
├── requirements.txt
└── README.md
```

---

## 📈 Power BI Dashboard

An interactive 4-page Power BI dashboard was built as the final deliverable:

| Page | Title | Key Visuals |
|------|-------|-------------|
| 1 | Overview | 4 KPI cards · Histogram · Donut · Bar charts |
| 2 | Demographics | Grouped bars · Edu:rec ratio · Health by location |
| 3 | Devices & Time | Device donut · Clustered columns · Weekday vs Weekend |
| 4 | Health & Cohorts | Dose-response chart · Matrix heatmap · Top 5 cohorts |

**Features:**
- Custom sidebar navigation with page buttons
- Synced slicers: Gender · Urban/Rural · Age Group · Screen Time Category
- Conditional colour heatmaps (Matrix visual with background gradient)
- Top N visual-level filter for highest-risk cohort ranking

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| **Data Handling** | Python, Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn, Plotly |
| **Dashboard** | Power BI Desktop |
| **Documentation** | Jupyter Notebook, PDF, PowerPoint |

---

## ▶️ How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/screensense-kids-screentime.git
   cd screensense-kids-screentime
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the dataset**
   - Visit [Kaggle — Indian Kids Screentime 2025](https://www.kaggle.com/datasets/ankushpanday2/indian-kids-screentime-2025)
   - Download `Indian_Kids_Screen_Time.csv` and place it in the `data/` folder

4. **Run notebooks in order**
   ```
   week1 → week2_3 → week3 → week4 → week5 → week6
   ```

5. **Open the dashboard**
   - Open `dashboard/Kids_Screen_Time_Analysis_Dashboard.pbix` in Power BI Desktop

---

## 📅 Week-wise Milestone Summary

| Week | Milestone | Deliverable |
|------|-----------|-------------|
| Week 1 | Data Setup | Loaded dataset, explored schema, handled nulls, saved cleaned CSV |
| Week 2–3 | Preprocessing & Feature Engineering | Created 6 derived columns: age_group, health_issue_present, health_issue_count, health_status, screen_time_category, weekday_flag |
| Week 3 | Univariate & Bivariate Analysis | 10+ visuals: histograms, boxplots, countplots, donut charts, scatter plots |
| Week 4 | Device & Weekday/Weekend Analysis | Device × gender/age/location charts, weekday vs weekend comparison |
| Week 5 | Cohort Analysis | 4 heatmaps (age×device, gender×activity, location×device, age×weekday), 4 stacked bar charts |
| Week 6 | Habit Patterns & Segment Insights | Segment-wise insights with possible drivers across location, age, gender |
| Week 7 | Power BI Dashboard | 4-page interactive dashboard, 22 visuals, synced slicers, sidebar navigation |
| Week 8 | Final Report & Presentation | PDF report (6 sections), 10-slide deck, GitHub repository |

---

## 📋 Evaluation Criteria Coverage

| Criterion | Evidence |
|-----------|----------|
| **Milestone Completion** | All 8 weeks completed with documented Jupyter notebooks |
| **Visual Analysis Quality** | 22 Power BI visuals + 30+ Python plots across 6 notebooks |
| **Insight Discovery** | Cohort heatmaps, dose-response health analysis, segment-wise insights with possible drivers |
| **Presentation & Reporting** | Final PDF report + 10-slide PowerPoint deck + interactive .pbix dashboard |

---

## 📁 Feature Dictionary (Derived Columns)

| Column | Description |
|--------|-------------|
| `age_group` | Binned into: 8–12 children, 13–15 young teens, 16–18 teens |
| `health_issue_present` | Whether the child reports any health issue (yes/no) |
| `health_issue_count` | Number of distinct health issues reported |
| `health_status` | Good / Poor based on health_issue_present |
| `screen_time_category` | Low (0–2 hr), Moderate (3–8 hr), High (9+ hr) |
| `weekday_flag` | Weekday / Weekend indicator |
| `device_type` | Portable (Smartphone, Laptop, Tablet) vs Wall-mounted (TV) |
| `educational_to_recreational_ratio` | Ratio of educational to recreational screen usage |

---

## 📌 Conclusions & Recommendations

**For Parents**
- Enforce screen-free weekdays — target under 2 hr/day
- Weekends require the most active supervision (100% of kids exceed limits)
- Children aged 8–12 show the biggest weekend spike (+154%) — prioritise this group

**For Educators**
- Increase educational content ratio — target edu:rec ratio of 0.6+
- After-school digital programmes should replace recreational screen time
- Teens (13–18) need the most intervention — their ratios are the lowest

**For Policymakers**
- Launch national awareness campaigns targeting the 13–18 age group
- Rural and urban programmes can use identical messaging — patterns are the same
- The solution is clear: keeping daily usage below 2 hr eliminates health impacts entirely

---

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

Dataset credit: [Ankush Panday — Kaggle](https://www.kaggle.com/datasets/ankushpanday2/indian-kids-screentime-2025)

---

*ScreenSense — Kids' Screen Time Visualization Project · 8 Weeks · 9,668 Records · Kaggle Indian Kids Screentime 2025*
