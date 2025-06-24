# 🎥 Netflix Horror Genre Analysis Report (Last 12 Months)

## 🔍 Overview
This project investigates how horror content performed on Netflix over the past year. Using the official Netflix viewership dataset, we compare horror to non-horror content in terms of engagement, rank longevity, and viewing trends. We also analyze monthly trends and runtime-to-views correlation.

---

## 📊 Dataset
- **Source:** [Netflix Official Streaming Data - Kaggle](https://www.kaggle.com/datasets/sujaykapadnis/official-netflix-streaming-data)
- **Time Period:** Past 12 months
- **Data Attributes:**
  - `week`, `category`, `show_title`, `weekly_hours_viewed`, `weekly_views`, `runtime`
  - `cumulative_weeks_in_top_10`, `season_title`, `episode_launch_details`

---

## ✅ Key Findings

### 1. 🌟 Horror vs Non-Horror: Engagement Comparison
| Type       | Total Hours Viewed | Avg per Title |
|------------|--------------------|----------------|
| Non-Horror | 32.55B             | 16.91M         |
| Horror     | 3.32B              | **17.02M**     |
> **Insight:** Horror titles attract more views *per title*, despite contributing less overall.

---

### 2. 📆 Top 10 Most Watched Horror Titles
| Rank | Show Title                  | Hours Viewed (Millions) |
|------|-----------------------------|--------------------------|
| 1    | The Witcher                 | 384                      |
| 2    | The Recruit                 | 228                      |
| 3    | XO, Kitty                   | 180                      |
| 4    | My Life With the Walter Boys | 155                    |
| 5    | Destined with You          | 146                      |
| 6    | Obliterated                | 145                      |
| 7    | Painkiller                 | 145                      |
| 8    | The Killer                 | 125                      |
| 9    | Celebrity                  | 113                      |
| 10   | We Have a Ghost            | 106                      |

**Chart:**  
`images/top_horror_bar.png`

> **Graph Insight:** These titles represent peak horror performance; serialized formats like TV shows dominate.

---

### 3. 🏠 Format-Wise Viewership Breakdown
| Category            | Total Weekly Hours Viewed |
|---------------------|----------------------------|
| TV (English)        | 1.69B                      |
| TV (Non-English)    | 681M                       |
| Films (English)     | 759M                       |
| Films (Non-English) | 188M                       |

**Chart:**  
`images/category_pie_chart.png`

> **Graph Insight:** Viewers prefer TV content over films, with English-language content leading across formats.

---

### 4. ⏱️ Rewatchability & Shelf Life
| Type       | Avg Weeks in Top 10 |
|------------|----------------------|
| Non-Horror | 3.07 weeks           |
| Horror     | 2.34 weeks           |

**Chart:**  
`images/rewatchability_bar_chart.png`

> **Graph Insight:** Horror content has a shorter lifecycle in trending charts, emphasizing the need for strong launch promotion.

---

### 5. 🌌 Monthly Trends
| Month      | Horror View Hours (Millions) |
|------------|-------------------------------|
| January    | 345.89M                       |
| February   | 126.13M                       |
| March      | 107.04M                       |
| April      | 66.58M                        |
| May        | 273.77M                       |
| June       | 97.05M                        |
| July       | 603.40M                       |
| August     | 347.10M                       |
| September  | 195.00M                       |
| October    | 288.00M                       |
| November   | 196.90M                       |
| December   | 672.46M                       |

**Chart:**  
`images/monthly_trend_line_chart.png`

> **Graph Insight:** Spikes during July and December suggest seasonal binging beyond Halloween.

---

### 6. ⏲ Runtime vs Views
**Valid records:** 126

**Chart:**  
`images/runtime_scatter.png`

> **Graph Insight:** While there's no strict correlation, most high-performing horror titles are 1–3 hours long.

---

## 🔮 Actionable Marketing Insights
| Strategy                                | Rationale                                 |
|-----------------------------------------|--------------------------------------------|
| Promote horror in July and December     | Viewer demand peaks                        |
| Create more short-form horror content   | Best performance in 1–3 hr range           |
| Prioritize English-language content     | Majority audience prefers English          |
| Focus campaigns around launch week      | Shorter shelf life compared to other genres|
| Leverage Halloween for seasonal titles  | High awareness and increased binge intent  |

---

## 📚 Tools & Technologies
- Python (pandas, matplotlib, seaborn)
- Jupyter Notebook
- KaggleHub for dataset access

---

## 🚀 Author
**Saloni**  
Ops Support Expert, Amazon (Go-AI)  
Kaggle & GitHub Enthusiast

---

## 🔄 Reproduce This Report

```bash
git clone https://github.com/<your-repo>/netflix-horror-trend-analysis.git
cd netflix-horror-trend-analysis
pip install -r requirements.txt
jupyter notebook main.ipynb
