# Spotify Track Insights — Power BI Dashboard

> Interactive Power BI dashboard exploring popularity, energy, tempo, and genre trends across 62,000+ Spotify tracks — built with Power Query transformations and custom DAX measures.

---

## 🛠️ Tools & Technologies

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoftexcel&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=flat&logo=microsoft&logoColor=white)
![Power Query](https://img.shields.io/badge/Power_Query-0078D4?style=flat&logo=microsoft&logoColor=white)

---

## 📌 Business Problem

What actually makes a track popular on Spotify? This dashboard enables **self-service exploration** of track-level audio features and popularity metrics — answering questions a music label, streaming analyst, or playlist curator might ask:

- Which genres consistently produce high-popularity tracks?
- How do energy and tempo correlate with listener engagement?
- Which artists dominate specific audio feature profiles?

---

## 📊 Data

| Attribute | Detail |
|---|---|
| Tracks analyzed | 62,000+ |
| Source | Spotify track dataset |
| Key fields | Track name, artist, genre, popularity score, energy, tempo, danceability, loudness, acousticness, release year |

---

## ⚙️ Methodology

1. **Data Ingestion & Cleaning** — Imported raw data into Power Query; handled nulls, standardized genre labels, removed duplicate track entries
2. **Transformation** — Created calculated columns for energy tiers, tempo buckets, and popularity bands to enable intuitive filtering
3. **Data Modeling** — Structured relationships between track, artist, and genre tables for efficient DAX calculation
4. **DAX Measures** — Built custom measures for average popularity by genre, artist-level track counts, energy/tempo distributions, and YoY trend calculations
5. **Dashboard Design** — Designed multi-page layout with drill-through filters, KPI cards, and cross-filtering for self-service exploration

---

## 📈 Key Results

| Feature | Detail |
|---|---|
| Pages | Multi-page dashboard with genre, artist, and audio feature views |
| KPI cards | Popularity, energy, tempo, danceability — all sliceable |
| Interactivity | Drill-through filters, cross-report filtering, dynamic titles |
| Insight | Genre and energy tier are the strongest predictors of track popularity in this dataset |

---

## 🖼️ Screenshots / Visuals

<img width="1280" height="720" alt="Slide1" src="https://github.com/user-attachments/assets/54ed2f50-631b-4306-9f83-41179c52398a" />
<img width="1280" height="720" alt="Slide2" src="https://github.com/user-attachments/assets/0ff38103-4063-4e8b-aba0-829563ca7856" />



---

## ▶️ How to Run

1. Download the `.pbix` file from this repo
2. Open in **Power BI Desktop** (free download from Microsoft)
3. If prompted, refresh the data source and point to the `/data` folder
4. All visuals and measures will load automatically

---

## 💡 Learnings

- DAX context transition (row context vs. filter context) is unintuitive at first — understanding it unlocked more sophisticated measures and fixed several calculation errors
- Dashboard design is an analytical skill: arranging visuals so a viewer reaches the key insight in under 30 seconds requires deliberate layout choices, not just accurate charts
- Power Query's M language handles transformation logic that would otherwise require multiple pre-processing scripts — keeping the pipeline in one tool reduces maintenance overhead

---
