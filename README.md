#  Spotify & YouTube Music Data Cleaning

##  Project Overview

This project focuses on cleaning and preprocessing a combined **Spotify and YouTube Music dataset** to ensure consistency, accuracy, and usability for further analysis. The data contained missing values, irregular formatting, duplicates, inconsistent data types, and merged columns. Using structured cleaning techniques, the dataset was standardized to make it analysis-ready.

---

##  Objectives

* Identify and handle **missing values** in key columns such as Views and Likes.
* Fix irregularities in **merged columns** (Spotify\_Info & YouTube\_Info).
* Standardize **naming conventions** and correct case sensitivity.
* Remove **irrelevant columns** and random data.
* Convert **inconsistent data types** (text → numeric).
* Replace **invalid data entries** with meaningful placeholders.
* Check and remove **duplicate rows** for uniqueness.
* Reorder and rename columns for better **clarity and readability**.

---

##  Key Data Cleaning Steps

### 1️ Handle Missing Values

* Filled **Views** and **Likes** with `0` (indicating no engagement yet).
* Preserved contextual data by avoiding row deletion.

### 2️ Fix Merged Columns

* **Spotify\_Info** → Split by `|` delimiter to extract clean links.
* **YouTube\_Info** → Split by fixed character lengths for URLs.

### 3️ Standardization

* Converted all column names to **lowercase\_with\_underscores**.
* Applied **Title Case** to Artist and Track names.

### 4️ Remove Irrelevant Data

* Dropped **random\_column\_1** and **random\_column\_2** (no insights).
* Cleaned placeholder values like “N/A”, “nan”, and “UNKNOWN”.

### 5️ Fix Data Types

* Converted numeric features like **danceability, energy, views** to proper numeric format.
* Replaced conversion errors with `0` or `null`.

### 6️ Handle Invalid Entries

* Replaced “invalid\_data” in **Views** with `null`.
* Ensured **Album column** only contained valid labels.

### 7️ Duplicates Check

* Used key columns (ID, Track, Album) to check uniqueness.
* Ensured no duplicate rows remained.

### 8️ Reorder & Rename Columns

* Example order: **ID, Track Name, Album Name, Artist Name, Spotify\_Link, YouTube\_Link, Views, Likes**.
* Renamed columns for clarity (`unnamed:0 → ID`, `spotify_info → spotify_song_link`, etc.).

---

## Outcomes

✅ Cleaned dataset ready for analysis and visualization.
✅ Consistent column naming conventions and standardized formats.
✅ Removed irrelevant and noisy data to improve accuracy.
✅ Ensured **data integrity** for further analytics like trend analysis, popularity comparisons, and recommendation systems.

---

##  Tools & Technologies

* **Power Query / Power BI Editor**
* **Data Cleaning Techniques** (null handling, standardization, deduplication)
* **Data Quality Assurance**
* **dataset** [Spotify & YouTube Music](https://drive.google.com/file/d/1qanyuwEzkwEJ73vDJHk4ZlWE0JUG7udb/view)

---

## 👩‍💻 Author

**Disha Sindhi**

* Email: [dishasindhi7@gmail.com](mailto:dishasindhi7@gmail.com)
* LinkedIn: [Disha Sindhi](https://www.linkedin.com/in/disha-sindhi-b0092732a)
* portfolio: [Disha Sindhi portfolio](https://www.wscubetech.com/portfolio/data/disha-sindhi-rsk7ymi)
