# 📊 n8n Workflow – TikTok Competitor Data Scraper

## 📝 Description
This workflow was built in **n8n** to automate the process of **scraping competitor accounts on TikTok**.  
The scraped data (e.g., video stats, captions, engagement metrics) is collected on a daily basis and then stored for further marketing analysis.  
This allows the marketing team to monitor competitor activity and trends without having to manually visit each account.

---

## ⚙️ Workflow Steps
1. **Schedule Trigger**  
   - Runs automatically once a day.  

2. **Apify Actor / HTTP Request Node**  
   - Executes a scraper to fetch competitor TikTok data.  
   - Extracts details such as video title, views, likes, comments, and publish time.  

3. **Transform Data (Function Node)**  
   - Cleans and structures the raw JSON into tabular format.  

4. **Google Sheets / Database Node**  
   - Saves the processed data into Google Sheets (or database if needed).  

5. **Optional: Notification Node (Telegram/Slack)**  
   - Sends a notification when new competitor data has been stored.  

---

## 🖼️ Workflow Example
A simplified view of the workflow:

<img width="1610" height="628" alt="image" src="https://github.com/user-attachments/assets/b6b07694-44f5-49d8-a294-acc3aee63e17" />


---

## 🚀 Implementation Results
- Automated daily competitor data collection from TikTok.  
- Enables the marketing team to perform trend and engagement analysis.  
- Saves hours of manual effort checking competitor accounts.  
- Provides structured data ready for visualization and analysis.  

---

## ⚠️ Notes
- This workflow uses **dummy credentials and API tokens** in the exported JSON for security reasons.  
- The actual implementation connects to Apify or TikTok scraping APIs with real credentials.  

---
