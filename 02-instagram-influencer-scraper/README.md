# 📸 **Instagram Hashtag Scraper — Automated Workflow**

### 📘 **Overview**

This n8n workflow automates the process of **scraping Instagram posts by hashtag** and extracting detailed **profile data** for each post owner.
By simply entering a hashtag, it collects recent posts, extracts usernames, and gathers **public profile details** — all saved automatically to **Google Sheets** for analysis or CRM use.

This project demonstrates **data automation**, **social media analysis**, and **API-based data extraction** using n8n’s modular workflow design.

---

## ⚙️ **How It Works**

1. **User Input (Hashtag Entry)**
   The workflow begins with a manual or scheduled trigger where the user inputs a hashtag (e.g., `#fashionblogger`).

2. **Post Fetching**
   The workflow connects to an external Instagram scraper API to collect the latest posts for that hashtag, returning post URLs, captions, and usernames.

3. **Profile Extraction**
   It then loops through each username to gather public profile data such as:

   * Username
   * Followers count
   * Bio
   * Category or niche
   * Contact info (if available)
   * Engagement metrics

4. **Google Sheets Integration**
   Each profile’s data is structured and written into a connected Google Sheet, ready for analysis or influencer selection.

---

## 🧩 **Core Process Overview**

| Stage  | Function        | Output                         |
| ------ | --------------- | ------------------------------ |
| Part 1 | Hashtag Input   | Triggers the workflow          |
| Part 2 | Post Collection | List of users per hashtag      |
| Part 3 | Profile Scraper | User info from public profiles |
| Part 4 | Data Export     | Google Sheets record           |

Each part is modular and can be reused independently or combined for full automation.

---

## 🧭 **Setup Guide**

### 1️⃣ **Preparation**

* Set up your **Google Sheets** integration in n8n.
* Create one Google Sheet for storing collected profile data.
* Obtain access to a **public Instagram scraping API** (such as Apify, RapidAPI, or another endpoint provider).
* Add the API credentials securely in n8n.

### 2️⃣ **Execution**

* Enter a target **hashtag** in the workflow trigger node.
* Run the workflow — it will fetch posts, extract usernames, and retrieve profile details.
* The final dataset will automatically populate your connected Google Sheet.

---

## 🧠 **Tips & Best Practices**

* Limit API calls to avoid **rate limits** or **temporary blocks**.
* Use **n8n’s Wait or SplitInBatches** nodes for controlled requests.
* Run the workflow on a **schedule** (e.g., daily or weekly) to collect ongoing data.
* For better segmentation, use a separate sheet per hashtag or campaign.
* Verify data fields (some profiles may hide certain info).

---

## 🧾 **Example Result**

After the workflow completes:

* The Google Sheet contains influencer profiles extracted by hashtag.
* Each row includes profile details, bio, follower count, and post engagement data.
* Perfect for CRM imports, campaign targeting, or influencer analysis.

---

## 🪪 **Requirements**

* n8n version ≥ 1.50
* Google Sheets account and credentials
* Access to a compatible Instagram scraping API

---

## 🧩 **Tech Stack**

* **Platform:** n8n
* **Integrations:** Google Sheets API, Instagram Scraper API
* **Data Handling:** JSON to Sheet conversion, looping, and structured extraction
* **Automation Type:** API-driven data pipeline

---

## 📸 **Preview**

*(Optional: add a workflow screenshot or diagram here)*
Example:

```
/assets/instagram-hashtag-scraper-diagram.png
```

---

## 📬 **Author**

**Created by:** Sief Shama

**Focus:** Automation Development · Data Engineering · AI Integration

**LinkedIn:** [linkedin.com/in/siefshama](https://www.linkedin.com/in/siefshama/)

