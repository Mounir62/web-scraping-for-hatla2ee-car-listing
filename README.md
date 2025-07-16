# 🔍 Hatla2ee Car Listings Scraper & Analysis

This project is a comprehensive end-to-end solution for scraping, analyzing, and modeling data from the **Hatla2ee** Egyptian car listings website. The project includes Python-based web scraping, CSV data export, Power BI visualizations, and machine learning (Linear Regression) for car price prediction.

---

## ✨ Project Highlights

* 🤖 **Web Scraping:** Extracts structured data from Hatla2ee's Mercedes listings
* 📂 **Data Storage:** Stores data into `data.csv` including car title, model, color, mileage, location, price, date, and image URL
* 🌍 **Compliance:** Respects `robots.txt` restrictions and implements retry + backoff for stable crawling
* 📊 **Visualization:** Power BI dashboards analyzing pricing, color trends, popular models, and more
* 🎯 **ML Model:** Linear Regression model to predict car prices based on multiple features

---

## 🔢 Technologies Used

* **Python 3.10+**
* **BeautifulSoup & Requests** – for scraping
* **Pandas & NumPy** – for preprocessing and analysis
* **Scikit-learn** – for machine learning
* **Power BI** – for interactive data visualization

---

## 🔗 Dataset Overview

After scraping, the dataset contains the following columns:

* `title`
* `car_model_name`
* `car_color`
* `car_mileage`
* `location`
* `date`
* `price`
* `image`

Over 1000 rows of car listing data were collected and exported to `data.csv`.

---

## 📈 Power BI Insights

Power BI was used to create dashboards including:

* Count of cars by model and location
* Color popularity and impact on pricing
* Listing trends by month
* Mileage vs. price scatter plots
* Average price per year/model

---

## 🎓 Machine Learning Component

A simple Linear Regression model was trained on the scraped dataset:

* Features: car model, color, mileage, location
* Target: price
* Encoding: One-hot encoding for categorical variables
* Metrics: Mean Squared Error (MSE), R-squared (R²)

The trained model provides price predictions based on input features with basic accuracy.

---

## 🛠️ How to Run

1. **Clone the repository**
2. Run the Jupyter notebook `Hatla2ee_scraping_model.ipynb` to scrape and analyze data
3. Open `data.csv` in Power BI for visualization
4. Modify and retrain the regression model as needed
