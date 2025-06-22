🔍 Law Firm SEO Ranking Analysis

This project analyzes key on-page SEO factors that influence search engine ranking for law firm websites. By crawling real-world sites and extracting structured signals, we compare the top 3 results against ranks 4–10 to understand what differentiates higher-performing pages.

⸻

📁 Project Structure
```
.
├── code/
│   ├── sftop10_crawler.ipynb        # Web scraping: crawl top 10 law firm result pages
│   ├── SEO_data_cleaning.ipynb      # Clean and process raw HTML signal data
│   └── SEO_expanding.ipynb          # Enrich with additional SEO metrics (Moz, Lighthouse, etc.)
│
├── result/
│   ├── part1_Moz_Enriched_Results/  # Intermediate JSON or HTML parsing results
│   ├── Part2_Moz_Enriched_Results/  # Additional or normalized metrics
│   ├── sf_top3_seo_signals_results.csv     # Final feature set for Top 3 ranked pages
│   ├── sf_top10_seo_signals_results.csv    # Final feature set for Top 4–10 ranked pages
│
│   # 📊 Visualization outputs
│   ├── Alt Text Coverage & External Linking: Top 3 vs Top 4–10.png
│   ├── Content Length Comparison: Top 3 vs Top 4–10.png
│   ├── Internal Linking: Top 3 vs Top 4–10.png
│   ├── Page Load Performance: Top 3 vs Top 4–10 (San Francisco).png
│   └── Radar Chart of Key SEO Signals (Normalized).png
│
└── README.md
```
⸻

📊 Key Findings

1. 🖼️ Alt Text Coverage & External Linking

Top 3 pages have slightly more consistent alt text usage. Interestingly, Top 4–10 pages contain more external links, but that doesn’t directly lead to better rankings.

<img src="result/Alt%20Text%20Coverage%20&%20External%20Linking:%20Top%203%20vs%20Top%204–10.png" alt="Alt Text and External Linking" width="700"/>



⸻

2. 📄 Content Length Comparison

Top 4–10 pages tend to have slightly higher word counts, though medians are close. Top-ranked pages may emphasize concise, focused content.

<img src="result/Content%20Length%20Comparison:%20Top%203%20vs%20Top%204–10.png" alt="Content Length" width="600"/>



⸻

3. 🔗 Internal Linking

Top 3 results generally feature more internal links, which may improve crawlability and SEO authority structure.

<img src="result/Internal%20Linking:%20Top%203%20vs%20Top%204–10.png" alt="Internal Linking" width="600"/>



⸻

4. ⚡ Page Load Performance (San Francisco)

Page speed remains critical: Top 3 pages load ~30% faster on average compared to lower-ranking pages.

<img src="result/Page%20Load%20Performance:%20Top%203%20vs%20Top%204–10%20(San%20Francisco).png" alt="Page Load Performance" width="700"/>



⸻

5. 🕸️ Radar of Key SEO Signals

Radar chart summarizing differences in key SEO metrics.

<img src="result/Radar%20Chart%20of%20Key%20SEO%20Signals%20(Normalized).png" alt="Radar Chart" width="600"/>



⸻

⚙️ Tech Stack
* Python / Jupyter Notebooks
* requests, BeautifulSoup, tqdm – web scraping
* pandas, numpy – data processing
* matplotlib, seaborn – data visualization
* lighthouse / Pagespeed API – performance metrics (optional)

⸻

✅ How to Use
1. Clone the repo
2. Run sftop10_crawler.ipynb to scrape legal websites and extract signals
3. Clean the data using SEO_data_cleaning.ipynb
4. Enrich the features and generate visuals from SEO_expanding.ipynb

⸻

📌 Future Work
* Add semantic analysis of headings and content topics
* Include backlink profile via Moz/Majestic API
* Run statistical tests to validate feature importance
