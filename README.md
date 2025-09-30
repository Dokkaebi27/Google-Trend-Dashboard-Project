# 📊 Google Trends Analysis Dashboard

🌐 Languages: [English](#english-version) | [Bahasa Indonesia](#versi-bahasa-indonesia)

---
## English Version

Welcome to the **Google Trends Dashboard** repository 🚀 

This repository showcases an interactive **Google Trends dashboard** built using **Power BI**. The project tracks and visualizes keyword performance across popular social media platforms.

---

## 🔎 Project Overview
- **Data Source**: Google Trends (via SerpAPI / manual export)  
- **Tools Used**: Power BI (Data visualization & dashboarding)  
- **Objective**: To analyze and compare the popularity of keywords related to **YouTube, Facebook, Instagram, TikTok, and Twitter/X** in globally.

---

## 📊 Dashboard Highlights  
🌍 **Overview**  
- Provides a snapshot of recent keyword search trends.  
- Summarizes total social media–related keywords tracked in the dashboard.  
- Offers a country filter to explore Google Trends by region. 

📈 **Keyword by Date**  
- Tracks **keyword search performance over time** (2004-2025).  
- Allows switching between **different time granularities** (Y/Q/M) for flexible analysis.  
- Highlights **search volume fluctuations** and identifies periods with the highest keyword interest.  
- Useful for spotting **seasonal trends and event-driven spikes** in search behavior.    

⭐ **Rising & Top Keywords**  
- Displays the **most popular keywords** along with their trend scores.  
- Highlights **fastest-growing (Rising) keywords** vs. **consistently searched (Top) keywords**.  
- Provides **category classification** (e.g., YouTube channel, Computer program, etc.).  
- Helps identify **emerging topics** and monitor **brand or product visibility** in real time.
  
⏱️ **Real Time**  
- Shows recent keyword search activity across platforms.
- Displays total searches and keyword distribution.

---
## 📂 Repository Structure
``` 
Google-Trend-Social-Media-Dashboard/
│
├── Docs/                          # Project documentation 
│   ├── Google Trends.pdf
│   ├── Keywords by Date.png
│   ├── Overview.png
│   ├── Real Time.png
│   └── Rising & Top Keyword.png       
│
├── PowerBI/  
│   └── Google Trends.pbix        # Main Power BI dashboard file
│
├── SerAPI/
|   └── Readme.md                 # API query scripts
│
├── README.md                     # Main repository documentation
``` 

---
## 🔧 How to Change Parameters in Power BI  

To customize the dashboard with different keywords or settings, you can modify the parameters in **Power Query Editor**.  

### Steps  
1. Open **Power Query Editor**  
   - Go to the **Home** tab in Power BI Desktop.  
   - Click **Transform Data** → **Transform Data** again.  

2. Locate the **Parameters**  
   - On the left Queries panel, expand the **Parameters** folder.  
   - Available parameters include:  
     - `Keywords` (e.g., YouTube, TikTok, Instagram, etc.)  
     - `Related Keyword`  
     - `Key` (API key)  

3. Update the Parameter  
   - Select the parameter you want to change.  
   - Edit the **Current Value** field (e.g., change from `YouTube` → `TikTok`).  
   - Use **Manage Parameter** if you want to set allowed values or defaults.  

4. Apply the Changes  
   - Click **Close & Apply** to refresh the data model.  
   - The dashboard will now update automatically based on your new parameter.
### Example  
To analyze **TikTok** instead of **YouTube**:  
- Go to **Transform Data > Parameters > Keywords**.  
- Change the current value from `YouTube` → `TikTok`.  
- Click **Close & Apply**.  
- The dashboard will refresh and display TikTok trends.

---

## 🔑 Insights
1. **YouTube** consistently leads in search interest (~40% of total share).  
2. **Facebook** remains strong in globally, ahead of TikTok and Twitter.  
3. **Instagram** shows steady growth, but not as high as YouTube or Facebook.  
4. **Rising Keywords** often include YouTube-related products (*YouTube Music, Shorts, Studio*).  
5. Strong weekend spikes suggest user engagement is time-sensitive.  

---


## 🙍 About Me  

Hi, I'm **Ahmad Zaki Amani** 👋  

✨ I'm passionate about **Data Analytics** and **Business Intelligence**, focusing on building dashboards, creating data visualizations, and turning raw data into actionable insights.  

💡 This project is part of my portfolio, where I showcase skills in:  
- Data visualization & storytelling  
- Dashboard design (Power BI, Tableau)  
- Data transformation & analysis  
- Business Intelligence solutions  

📫 Let’s connect and collaborate!  

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ahmadzaki27.az@gmail.com) 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ahmad-zaki-amani-ab091635b/)  

---
## Versi Bahasa indoneasia

