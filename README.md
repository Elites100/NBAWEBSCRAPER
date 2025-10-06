# 🏀 NBA Stats Scraper

**Lightweight Python scraper** that fetches NBA stats pages, extracts leaderboard tables, and prints them nicely.  
Parsed tables can be saved to **CSV** and **pretty TXT** files.

The script uses **pandas** (preferred) and falls back to **BeautifulSoup** for static HTML tables.  
It prompts before writing files, so you always control what gets saved.

---

## ✨ Features

- Parses HTML tables using `pandas.read_html()` for clean DataFrame output.  
- Falls back to a **BeautifulSoup-based** table formatter when pandas finds no tables.  
- **Pretty console output** with aligned and truncated columns for readability.  
- **Interactive saving:** save per table, save all, or skip saving entirely.  
- Writes both **CSV** and **TXT** previews for each saved table.  
- Output files are saved to an `output/` folder with safe filenames and timestamps.

---

## 🎬 Short Demo

1. Run the script to parse and preview tables in the console.  
2. When prompted, choose:  
   a → save all tables  
   n / y → save this table  
   s → skip all remaining saves  
4. Saved files appear in the `output/` directory (next to the script).

---

## 🧩 Requirements

- **Python 3.8+**
- Install dependencies via `requirements.txt`:  
requests  
beautifulsoup4  
pandas  
lxml  
html5lib

You can install them all at once with:

pip install -r requirements.txt

## 🚀 Usage
python nba_stats_scraper.py

## 📁 Output
output/
├── table_1_Leaders_20251006_120314.csv
└── table_1_Leaders_20251006_120314.txt
