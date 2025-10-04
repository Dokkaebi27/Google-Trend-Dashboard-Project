🌐 Languages: [English](#english-version) | [Bahasa Indonesia](#indonesian-version)

<a name="english-version"></a>
# 📊 Google Trends Analysis Dashboard

Welcome to the **Google Trends Dashboard** repository 🚀 

This repository showcases an interactive **Google Trends dashboard** built using **Power BI**. The project tracks and visualizes keyword performance across popular social media platforms.

**Project Type**: End-to-End Data Analytics & Business Intelligence. 

**Tool Used**: Microsoft Power BI, and Google Trends API.

---

## 🔎 Project Overview

- **Data Source**: Google Trends (via SerpAPI / manual export)  
- **Tools Used**: Power BI (Data visualization & dashboarding)  
- **Objective**: To analyze and compare the popularity of keywords related to **YouTube, Facebook, Instagram, TikTok, and Twitter/X** in globally.

---
## 📌 Problem Statement

Currently, online keyword trend data is fragmented across platforms (YouTube, Facebook, Instagram, TikTok, Twitter), making it difficult for marketing teams, researchers, and analysts to monitor rising trends in one place.

From the dashboard screens, the key problems solved are:

* **No unified keyword monitoring** → Dashboard provides quick summaries such as total searches, keyword distribution per platform, and popularity share.
* **Hard to track rising vs top keywords** → Consolidated view highlights trending (rising) and most searched (top) keywords for better prioritization.
* **Difficulty in analyzing keyword growth over time** → Visualization of keyword performance across years, months, and days makes it easier to spot long-term and short-term trends.
* **Lack of geographic insights** → Integration with world map provides clear visibility into regional keyword popularity and global distribution.
* **Disconnected platform insights** → Dashboard unifies Google Trends data for multiple platforms (YouTube, Facebook, TikTok, Instagram, Twitter) into a single view.
* **Decision-making gaps** → Teams can identify which keywords are gaining traction, allocate marketing resources effectively, and anticipate audience demand.

---
## 🎯 Business Requirement

Marketing teams, trend analysts, and researchers need a **consolidated dashboard** to monitor keyword performance across platforms (YouTube, Facebook, Instagram, TikTok, Twitter) in order to quickly identify rising and popular trends.

Based on the dashboard screens, the business requirements include:

---
🌍 **Overview Page**  
- Provides a snapshot of recent keyword search trends.  
- Summarizes total social media–related keywords tracked in the dashboard.  
- Offers a country filter to explore Google Trends by region.

---
📈 **Keyword by Date Page**  
- Tracks **keyword search performance over time** (2004-2025).  
- Allows switching between **different time granularities** (Y/Q/M) for flexible analysis.  
- Highlights **search volume fluctuations** and identifies periods with the highest keyword interest.  
- Useful for spotting **seasonal trends and event-driven spikes** in search behavior.
   
---
⭐ **Rising & Top Keywords Page**  
- Displays the **most popular keywords** along with their trend scores.  
- Highlights **fastest-growing (Rising) keywords** vs. **consistently searched (Top) keywords**.  
- Provides **category classification** (e.g., YouTube channel, Computer program, etc.).  
- Helps identify **emerging topics** and monitor **brand or product visibility** in real time.

---
⏱️ **Real Time Page**  
- Shows **recent keyword search activity across platforms.**
- Displays **total searches and keyword distribution.**

---
💡 **Decision Support**
* Identify trending keywords for **digital marketing campaigns**.
* Monitor popular and emerging keywords for **content strategy**.
* Allocate resources to platforms with the highest growth.
* Support research into **audience search behavior changes** across regions.

---
## 🔑 Insights
1. **YouTube** consistently leads in search interest (~40% of total share).  
2. **Facebook** remains strong in globally, ahead of TikTok and Twitter.  
3. **Instagram** shows steady growth, but not as high as YouTube or Facebook.  
4. **Rising Keywords** often include YouTube-related products (*YouTube Music, Shorts, Studio*).  
5. Strong weekend spikes suggest user engagement is time-sensitive.  

---
## 📂 Repository Structure
``` 
Google-Trend-Dashboard-Project/
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

## Steps  
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
🌐 Languages: [English](#english-version) | [Bahasa Indonesia](#indonesian-version)

---
<a name="indonesian-version"></a>
# 📊 Dasbor Analisis Google Trends

Repositori ini menampilkan **dashboard interaktif Google Trends** yang dibangun menggunakan **Power BI**. Proyek ini bertujuan untuk melacak dan memvisualisasikan performa kata kunci di berbagai platform media sosial populer.

**Jenis Proyek**: End-to-End Data Analytics & Business Intelligence

**Alat yang Digunakan**: Microsoft Power BI, dan Google Trends API.

---

## 🔎 Gambaran Proyek

* **Sumber Data**: Google Trends (via SerpAPI / ekspor manual)
* **Tools**: Power BI (visualisasi data & pembuatan dashboard)
* **Tujuan**: Menganalisis dan membandingkan popularitas kata kunci terkait **YouTube, Facebook, Instagram, TikTok, dan Twitter/X** secara global.

---

## 📌 Permasalahan

Saat ini, data tren kata kunci online masih terpisah-pisah di berbagai platform (YouTube, Facebook, Instagram, TikTok, Twitter), sehingga menyulitkan tim pemasaran, peneliti, maupun analis dalam memantau tren yang sedang naik secara menyeluruh.

Berdasarkan tampilan dashboard, permasalahan utama yang dapat diselesaikan adalah:

* **Tidak ada pemantauan kata kunci terpadu** → Dashboard memberikan ringkasan cepat seperti total pencarian, distribusi kata kunci per platform, dan pangsa popularitas.
* **Sulit membedakan kata kunci naik vs populer** → Tampilan gabungan menyoroti kata kunci trending (naik) dan kata kunci yang paling sering dicari (populer).
* **Kesulitan menganalisis pertumbuhan kata kunci dari waktu ke waktu** → Visualisasi performa kata kunci per tahun, bulan, hingga hari memudahkan dalam melihat tren jangka panjang maupun pendek.
* **Kurang wawasan geografis** → Integrasi dengan peta dunia memberi visibilitas yang jelas tentang popularitas kata kunci di berbagai wilayah.
* **Informasi platform yang terpisah** → Dashboard menyatukan data Google Trends untuk beberapa platform dalam satu tampilan.
* **Kesenjangan pengambilan keputusan** → Tim dapat mengidentifikasi kata kunci yang sedang naik, mengalokasikan sumber daya pemasaran secara tepat, serta memprediksi kebutuhan audiens.

---

## 🎯 Kebutuhan Bisnis

Tim pemasaran, analis tren, dan peneliti membutuhkan **dashboard terpadu** untuk memantau performa kata kunci di berbagai platform (YouTube, Facebook, Instagram, TikTok, Twitter) agar dapat dengan cepat mengidentifikasi tren populer maupun tren yang sedang naik.

Berdasarkan tampilan dashboard, kebutuhan bisnis mencakup:

---

🌍 **Halaman Overview**

* Menyediakan ringkasan tren pencarian kata kunci terkini.
* Menyajikan total kata kunci terkait media sosial yang dilacak dalam dashboard.
* Menyediakan filter negara untuk mengeksplorasi Google Trends berdasarkan wilayah.

---

📈 **Halaman Keyword by Date**

* Melacak **performa pencarian kata kunci sepanjang waktu** (2004–2025).
* Dapat berganti antar **granularitas waktu** (Y/Q/M) untuk analisis yang fleksibel.
* Menyoroti **fluktuasi volume pencarian** dan periode dengan minat tertinggi.
* Berguna untuk melihat **tren musiman dan lonjakan akibat event tertentu**.

---

⭐ **Halaman Rising & Top Keywords**

* Menampilkan **kata kunci terpopuler** beserta skor trennya.
* Menyoroti **kata kunci dengan pertumbuhan tercepat (Rising)** vs **kata kunci yang konsisten dicari (Top)**.
* Memberikan **klasifikasi kategori** (misalnya YouTube channel, program komputer, dll).
* Membantu mengidentifikasi **topik yang sedang naik** dan memantau **visibilitas brand/produk** secara real time.

---

⏱️ **Halaman Real Time**

* Menampilkan **aktivitas pencarian kata kunci terbaru di berbagai platform**.
* Menyediakan ringkasan **total pencarian dan distribusi kata kunci**.

---

💡 **Dukungan Pengambilan Keputusan**

* Mengidentifikasi kata kunci trending untuk **kampanye digital marketing**.
* Memantau kata kunci populer maupun yang sedang naik untuk **strategi konten**.
* Mengalokasikan sumber daya ke platform dengan pertumbuhan tertinggi.
* Mendukung penelitian tentang **perubahan perilaku pencarian audiens** di berbagai wilayah.

---

## 🔑 Insight

1. **YouTube** konsisten memimpin minat pencarian (\~40% dari total pangsa).
2. **Facebook** tetap kuat secara global, lebih tinggi dibanding TikTok dan Twitter.
3. **Instagram** menunjukkan pertumbuhan stabil, meski tidak setinggi YouTube atau Facebook.
4. **Rising Keywords** sering berhubungan dengan produk YouTube (*YouTube Music, Shorts, Studio*).
5. Lonjakan pencarian di akhir pekan menunjukkan keterlibatan pengguna yang sensitif terhadap waktu.

---

## 📂 Struktur Repositori

```
Google-Trend-Social-Media-Dashboard/
│
├── Docs/                          # Dokumentasi proyek 
│   ├── Google Trends.pdf
│   ├── Keywords by Date.png
│   ├── Overview.png
│   ├── Real Time.png
│   └── Rising & Top Keyword.png       
│
├── PowerBI/  
│   └── Google Trends.pbix        # File utama dashboard Power BI
│
├── SerAPI/
|   └── Readme.md                 # Script query API
│
├── README.md                     # Dokumentasi utama repositori
```

---

## 🔧 Cara Mengubah Parameter di Power BI

Untuk menyesuaikan dashboard dengan kata kunci atau pengaturan lain, Anda dapat mengubah parameter di **Power Query Editor**.

### Langkah-langkah

1. Buka **Power Query Editor**

   * Pergi ke tab **Home** di Power BI Desktop.
   * Klik **Transform Data** → **Transform Data** lagi.

2. Temukan **Parameters**

   * Di panel Queries sebelah kiri, buka folder **Parameters**.
   * Parameter yang tersedia antara lain:

     * `Keywords` (contoh: YouTube, TikTok, Instagram, dll.)
     * `Related Keyword`
     * `Key` (API key)

3. Ubah Parameter

   * Pilih parameter yang ingin diubah.
   * Edit pada kolom **Current Value** (contoh: ubah dari `YouTube` → `TikTok`).
   * Gunakan **Manage Parameter** jika ingin menentukan nilai yang diizinkan atau default.

4. Terapkan Perubahan

   * Klik **Close & Apply** untuk menyegarkan data model.
   * Dashboard akan otomatis diperbarui sesuai parameter baru.

### Contoh

Untuk menganalisis **TikTok** menggantikan **YouTube**:

* Pergi ke **Transform Data > Parameters > Keywords**.
* Ubah nilai saat ini dari `YouTube` → `TikTok`.
* Klik **Close & Apply**.
* Dashboard akan menyegarkan dan menampilkan tren TikTok.

---

## 🙍 Tentang Saya

Halo, saya **Ahmad Zaki Amani** 👋

✨ Saya memiliki ketertarikan besar pada bidang **Data Analytics** dan **Business Intelligence**, khususnya dalam membangun dashboard, membuat visualisasi data, dan mengubah data mentah menjadi insight yang bermanfaat.

💡 Proyek ini merupakan bagian dari portofolio saya, yang menampilkan keterampilan dalam:

* Visualisasi data & storytelling
* Perancangan dashboard (Power BI, Tableau)
* Transformasi & analisis data
* Solusi Business Intelligence

📫 Mari terhubung dan berkolaborasi!

[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge\&logo=gmail\&logoColor=white)](mailto:ahmadzaki27.az@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/ahmad-zaki-amani-ab091635b/)

---
