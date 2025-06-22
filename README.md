🔍 Law Firm SEO Ranking Analysis

This project analyzes key on-page SEO factors that influence search engine ranking for law firm websites. By crawling real-world sites and extracting structured signals, we compare the top 3 results against ranks 4–10 to understand what differentiates higher-performing pages.

⸻

📁 Project Structure

.
├── sftop10_crawler.ipynb         # Web scraping for top 10 ranked law firm pages
├── SEO_data_cleaning.ipynb       # Data preprocessing and cleaning
├── SEO_expanding.ipynb           # Feature engineering and signal enrichment
├── sf_top3_seo_signals_results.csv   # Cleaned SEO signal data for top 3 pages
├── sf_top10_seo_signals_results.csv  # Cleaned SEO signal data for top 4–10 pages
├── visuals/
│   ├── Alt Text Coverage.png
│   ├── Content Length Comparison.png
│   ├── Internal Linking.png
│   └── Page Load Performance.png
└── README.md

⸻

📊 Key Findings

1. Alt Text & External Links

Top 3 pages show slightly more consistent usage of image alt attributes, but pages ranked 4–10 tend to have significantly more external links — which may not translate directly to better rankings.


⸻

2. Content Length

Word count is slightly higher on pages ranked 4–10, but the difference is not statistically significant. High-ranking content tends to be more concise and focused.


⸻

3. Internal Linking

Top 3 pages show stronger internal linking strategies, which likely help with crawlability and topical authority.


⸻

4. Page Load Speed

Top-ranking pages load faster, both in overall load time and first paint — a critical factor for user experience and SEO.


⸻

⚙️ Tech Stack
	•	Python / Jupyter Notebooks
	•	requests, BeautifulSoup, tqdm – web scraping
	•	pandas, numpy – data processing
	•	matplotlib, seaborn – data visualization
	•	lighthouse / Pagespeed API – performance metrics (optional)

⸻

✅ How to Use
	1.	Clone the repo
	2.	Run sftop10_crawler.ipynb to scrape legal websites and extract signals
	3.	Clean the data using SEO_data_cleaning.ipynb
	4.	Enrich the features and generate visuals from SEO_expanding.ipynb

⸻

📌 Future Work
	•	Add semantic analysis of headings and content topics
	•	Include backlink profile via Moz/Majestic API
	•	Run statistical tests to validate feature importance
