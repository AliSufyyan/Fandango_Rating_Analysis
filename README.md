# 🎬 Fandango Rating Analysis

An Exploratory Data Analysis (EDA) project investigating whether Fandango inflates its movie ratings — and how it compares to Rotten Tomatoes, Metacritic, and IMDB.

> Inspired by the FiveThirtyEight article: *"Be Suspicious Of Online Movie Ratings, Especially Fandango's"* (2015)

---

## 📌 Project Overview

Fandango is a movie ticketing platform that also displays user ratings. This project analyzes whether the stars shown to users are inflated compared to the actual underlying ratings — and compares Fandango's scoring behavior against other major review platforms.

---

## 📊 Datasets

| File | Description |
|---|---|
| `fandango_scrape.csv` | Scraped Fandango data — film title, displayed stars, actual rating, vote count |
| `fandango_score_comparison.csv` | Multi-platform ratings — Rotten Tomatoes, Metacritic, IMDB, Fandango |

---

## 🔍 Analysis Breakdown

1. **Fandango Rating Bias** — Compared displayed STARS vs actual RATING, quantified the inflation per film
2. **Rotten Tomatoes: Critics vs Users** — Measured disagreement between critic and audience scores
3. **Metacritic & IMDB Engagement** — Compared user vote counts across platforms
4. **Cross-Platform Normalization** — Normalized all scores to 0–5 scale and compared distributions side by side

---

## 📈 Key Findings

- Fandango consistently **rounds up** displayed star ratings (most common: +0.5 stars)
- After normalization, **Fandango's score distribution sits higher** than every other platform
- Rotten Tomatoes shows the **largest gap** between critic and audience scores
- IMDB has significantly **more user votes** than Metacritic

---

## 🛠️ Tech Stack

- Python 3.x
- NumPy
- Pandas
- Seaborn
- Matplotlib

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/fandango-rating-analysis.git
   cd fandango-rating-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install numpy pandas seaborn matplotlib jupyter
   ```

3. **Run the notebook**
   ```bash
   jupyter notebook Project.ipynb
   ```

---

## 📁 Project Structure

```
fandango-rating-analysis/
├── Project.ipynb                    # Main analysis notebook
├── fandango_scrape.csv              # Fandango scraped data
├── fandango_score_comparison.csv    # Multi-platform comparison data
└── README.md                        # You are here
```

---

## ⚠️ Limitations

- Data is from 2015 — Fandango may have updated its rating system since then
- Analysis is visual/exploratory — no formal statistical significance testing applied

---

## 🧠 What I Learned

- Performing EDA on real-world datasets with Pandas
- Visualizing distributions with Seaborn KDE plots and histograms
- Normalizing scores across different scales for fair comparison
- Merging datasets and extracting meaningful insights through visualization

---

## 📚 Reference

- Original FiveThirtyEight article by Walt Hickey (2015)
- Datasets sourced from the [FiveThirtyEight GitHub repository](https://github.com/fivethirtyeight/data/tree/master/fandango)
