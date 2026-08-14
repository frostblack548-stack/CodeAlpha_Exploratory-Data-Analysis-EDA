# 📚 Books to Scrape — Web Scraping, EDA & Data Visualization

## Internship Project

This project demonstrates an end-to-end data workflow — from **web scraping** to **data cleaning**, **exploratory data analysis (EDA)**, and **data visualization** — using the [Books to Scrape](https://books.toscrape.com/) website as the data source.

---

## 📌 Objective

Scrape book details from the *Books to Scrape* website using Python and BeautifulSoup, clean the collected data, perform exploratory data analysis, and visualize key trends and patterns in the dataset.

---

## 🗂️ Project Structure

```
├── TASK1.ipynb          # Web scraping, data cleaning & initial EDA
├── TASK2_EDA.ipynb       # Detailed exploratory data analysis
├── TASK3_DV.ipynb        # Data visualization
├── books_dataset_cleaned.csv   # Final cleaned dataset (output of Task 1)
└── README.md
```

### Task 1 — Web Scraping (`TASK1.ipynb`)
- Scrapes book data (title, price, availability, rating) from all 50 pages of `books.toscrape.com` using `requests` and `BeautifulSoup`.
- Cleans and preprocesses the raw scraped data (price formatting, rating conversion, etc.).
- Performs an initial round of EDA and visualization.
- Exports the cleaned dataset to `books_dataset_cleaned.csv`.

### Task 2 — Exploratory Data Analysis (`TASK2_EDA.ipynb`)
- Loads the cleaned dataset and explores its structure (`shape`, `info`, `describe`).
- Checks for missing values and duplicate records.
- Analyzes rating distribution and average book price.
- Summarizes key insights (total books, price range, rating counts, etc.).

### Task 3 — Data Visualization (`TASK3_DV.ipynb`)
- Visualizes the dataset using `matplotlib`, including:
  - Book Rating Distribution
  - Book Price Distribution
  - Average Price by Rating
  - Top 10 Most Expensive Books
  - Rating Percentage (Pie Chart)

---

## 📊 Dataset

| Column         | Description                          |
|----------------|---------------------------------------|
| `Title`        | Book title                            |
| `Price`        | Book price (£)                        |
| `Availability` | Stock availability status             |
| `Rating`       | Star rating (One–Five)                |

- **Total records:** 1,000 books
- **Missing values:** None
- **Duplicate records:** None

---

## 🔑 Key Insights

- Average book price: **£35.07**
- Highest price: **£59.99** | Lowest price: **£10.00**
- Rating distribution:
  - One: 226
  - Three: 203
  - Five: 196
  - Two: 196
  - Four: 179

---

## 🛠️ Tech Stack

- **Python 3**
- `requests` — HTTP requests
- `BeautifulSoup` (bs4) — HTML parsing
- `pandas` — data manipulation
- `matplotlib` — data visualization
- Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd <repo-folder>
   ```
2. Install dependencies:
   ```bash
   pip install requests beautifulsoup4 pandas matplotlib
   ```
3. Run the notebooks in order:
   - `TASK1.ipynb` → generates `books_dataset_cleaned.csv`
   - `TASK2_EDA.ipynb` → runs EDA on the cleaned dataset
   - `TASK3_DV.ipynb` → produces visualizations

> **Note:** Update the file path used to read `books_dataset_cleaned.csv` in Tasks 2 & 3 to match your local directory before running.

---

## ✅ Conclusion

This project demonstrates practical, end-to-end data analysis skills — web scraping, data cleaning, exploratory data analysis, and visualization — using real-world data from the Books to Scrape website. The final dataset is clean, well-structured, and ready for further analysis or machine learning applications.
