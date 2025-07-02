# Web Scraping & EDA of Bandung Tourism Data  
### JejakPiknik.com Tourism Extraction and Analysis

This project focuses on **web scraping** and **exploratory data analysis (EDA)** of tourism destinations in Bandung, Indonesia.  
Data was collected from **JejakPiknik.com**, a popular local travel blog that lists and describes various places of interest, including natural sites, cultural areas, entertainment parks, and more.

## Source Website

Data scraped from the following URLs:

- https://jejakpiknik.com/tempat-wisata-di-bandung/
- https://jejakpiknik.com/wisata-alam-bandung/
- https://jejakpiknik.com/destinasi-wisata-bandung/
- https://jejakpiknik.com/tempat-rekreasi-di-bandung/
- https://jejakpiknik.com/tempat-liburan-di-bandung/
- https://jejakpiknik.com/tempat-wisata-di-lembang/
- https://jejakpiknik.com/wisata-lembang/
- https://jejakpiknik.com/wisata-ciwidey/

## Tools & Libraries Used

- `Python`
- `BeautifulSoup`, `requests` – for web scraping
- `pandas`, `re` – for data cleaning and preprocessing
- `matplotlib`, `seaborn` – for data visualization
- `scikit-learn` – for TF-IDF & KMeans clustering
- `nltk` – for stopwords and sentiment classification

## Data Collected

For each destination, the following fields were extracted (when available):
- Name of the Place
- Address
- Ticket Price
- Phone Number
- Operating Hours
- Description

## Exploratory Data Analysis (EDA)

After scraping, the data underwent cleaning, structuring, and several exploratory visualizations:

### Price Categorization
- Grouped into: `Gratis`, `Murah`, `Menengah`, `Mahal`
- Most attractions are in the **Murah (<15K IDR)** category.

### Location Analysis
- Extracted sub-districts and regions (e.g., Lembang, Ciwidey).
- Lembang is the **most tourism-dense** area.

### Operational Schedule
- Parsed mixed formats of opening hours into **daily columns** (Mon–Sun).
- Created **heatmaps** and **bar plots** to compare opening durations.

### Type Classification (Manual Rules)
- Each place was classified as:  
  `Alam`, `Seni`, `Hiburan`, `Edukasi`, `Lainnya`

### Activity Clustering (TF-IDF + KMeans)
- Clustered descriptions into 6 activity types:
  - Hiking / Trekking
  - Camping / Alam
  - Hiburan Anak
  - Hiburan / Kuliner
  - Aktivitas Air
  - Alam Pegunungan

### Crowd Level Estimation
- Descriptions also clustered into **3 crowd levels**:
  - Tinggi
  - Sedang
  - Rendah

### Sentiment Analysis
- Used rule-based method to detect **positive**, **neutral**, or **negative** tone in the place descriptions.
  
## Key Insights

- **Lembang** has the highest tourism density.
- **Nature tourism (Alam)** dominates the region, followed by **entertainment**.
- A number of attractions operate **24 hours**, while most close by **17.00 WIB**.
- **Discounted attractions** can be grouped by price category and location.
- Clustering reveals underlying **tourist activity patterns** and **crowd levels**.

## Project Goals

- Automatically collect and structure unstructured tourism data from local websites.
- Enrich scraped data with additional metadata through EDA and unsupervised learning.
- Enable deeper analysis for tourism planning, business development, or travel recommendations.

## 🙋 Contact

If you'd like to collaborate, give suggestions, or use this project for academic or development purposes:

📧 Email: nadila4295@gmail.com  
🔗 LinkedIn: [(https://www.linkedin.com/in/nadila-gusriyani-8a5877242/)]

---

**#WebScraping #EDA #Python #BeautifulSoup #Bandung #JejakPiknik #DataScience #Clustering #SentimentAnalysis**
