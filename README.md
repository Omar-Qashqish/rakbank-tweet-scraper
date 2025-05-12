# 🐦 RAKBANK Tweet Scraper

RAKBANK Tweet Scraper is an automated tool built with **Python + Selenium** to collect recent tweets that mention **"rakbank"** or **"#rakbank"** from Twitter (X). It logs in to your account (once), scrolls through the search results, extracts tweet details, and exports them to an Excel file.

---

## 📌 What the Script Does

✅ Opens X (Twitter) using Selenium & Chrome  
✅ Logs in automatically using saved cookies  
✅ Navigates to the search page:
https://x.com/search?q=rakbank&src=typed_query&f=live

✅ Scrolls down the page to load more tweets  
✅ Extracts data from every tweet, including:
- **Username** – who posted the tweet  
- **Date** – when it was posted  
- **Content** – full tweet text  
- **Likes** – number of likes  
- **Retweets** – number of retweets  
- **Link** – direct URL to the tweet

✅ Saves the data into an Excel file:  
📄 `rakbank_tweets_full.xlsx`

---

## 📤 Output Example

| Username | Date | Content | Likes | Retweets | Link |
|----------|------|---------|-------|----------|------|
| @rakbank | 2025-05-10 10:43 | RAKBANK is hosting an event... | 12 | 3 | https://x.com/... |

---
⚠️ Notes
The tool uses Selenium to simulate human behavior. Twitter/X does not allow anonymous access to search pages.

You only log in once — the session is reused using saved cookies.

Make sure you’re using it responsibly and within Twitter’s terms of use.
