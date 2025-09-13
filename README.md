# Big Data Platforms and Analytics

This repository contains my analysis and solutions of the *Big Data Platforms and Analytics* course. The work covers two major problem areas: sampling analysis on an urban commute dataset and trip-level aggregation and clustering for a U.S. truck trips dataset.

---

## 📂 Repository Structure

* `notebook.ipynb` – Main Jupyter/Colab notebook with all code and analysis
* `report.pdf` – Detailed written report with explanations, methodology, and findings
* `urban_commute_population.csv` – Dataset of 100,000 urban commuters (used in Problem 1)
* `truck_trips_usa_500k.csv` – Dataset of 500,000 truck trips (used in Problem 2)
* `truck_routes_usa_reference.csv` – Route-level reference information for the truck trips dataset

---

## 📝 Problem 1: Sampling Urban Commute Data

City planners are collecting data to study commuting behavior. Using `urban_commute_population.csv` (100,000 records), I drew **three samples** of size 100:

* **Convenience sample** (first 100 records)
* **Simple random sample** (without replacement)
* **Stratified sample** proportionate to income bracket

### Analyses Performed

For each sample and the full dataset, I compared:

* Commute distance (km)
* Remote work days per week
* Car ownership (0–2 cars)
* Commute method (Walk, Bike, Transit, Car, Other, WFH)
* Commute time (minutes)
* Other relevant variables (parking, children, etc.)

I evaluated which sampling method best estimated the averages for commute distance, commute time, and remote work days, and provided an explanation for the differences.

---

## 🚚 Problem 2: Truck Trips Analysis

Using `truck_trips_usa_500k.csv` (trip-level data) and `truck_routes_usa_reference.csv` (route information), I performed:

### Route-Level Summarization

For each route, I computed:

* Total number of trips
* Average & standard deviation of distance, duration, and load
* Average & variability of cost per kilometer
* Total distance traveled & total cost

### Visualizations

Created charts to compare routes by:

* Cost efficiency
* Distance
* Load characteristics

### Exploratory Data Analysis (EDA)

* Relationship between distance, terrain type, load, duration, and costs
* Seasonal/temporal patterns:

  * Monthly cost variations
  * Peak-hour effects on duration or fuel consumption
* Identification of the most and least efficient routes (cost per km)

### Clustering Analysis

Performed clustering on the aggregated route-level dataset and interpreted clusters in business terms (geographic regions, terrain types, corridor lengths, etc.).

---

## 🛠️ Tools & Technologies

* Python (Pandas, NumPy, Matplotlib/Seaborn)
* Jupyter Notebook / Google Colab
* Excel for quick checks
* GitHub for version control

---

## 📊 Results

* Clear comparison of sampling strategies for urban commute data
* Aggregated route-level truck trip data with visualizations
* Insights into cost efficiency, distance, and load characteristics
* Identified meaningful route clusters for business insights

---

## 📄 Deliverables

* `.ipynb` notebook with code
* `.docx`/`.pdf` report with detailed explanations

---
