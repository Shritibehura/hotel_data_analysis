# 🏨 Hotel Booking Demand Analysis

This repository contains exploratory data analysis (EDA) of the [Hotel Booking Demand Dataset](https://www.sciencedirect.com/science/article/pii/S2352340918315191), which includes information on bookings made at a city hotel and a resort hotel.

## 📂 Dataset

The dataset (`hotel_bookings.csv`) includes **119,390 records** and **32 features** such as:

- Booking dates
- Number of adults, children, and babies
- Length of stay
- Room types (reserved vs assigned)
- Market segment
- Booking cancellation status
- Country of origin
- Average daily rate (ADR)

---

## 🔍 Project Goals

- Clean and prepare the data for analysis
- Explore guest demographics and booking patterns
- Identify relationships between booking features and cancellations
- Visualize guest origin with a world map
- Compare reserved vs assigned room types
- Analyze guest arrival trends and market segments

---

## ✅ Key Steps

### Data Cleaning
- Removed bookings with 0 guests (`adults + children + babies == 0`)
- Dropped duplicate rows
- Converted date columns to a proper datetime format
- Mapped months to numerical indices

### Feature Analysis
- Descriptive statistics of `lead_time`, `adr`, `total_of_special_requests`
- Quantile analysis of booking behavior
- Guest arrival trends over time

### Visualizations
- 📌 **Choropleth map**: Guest countries of origin (Plotly)
- 📌 **Cross-tab**: Reserved vs assigned room types
- 📌 **Pie chart**: Market segment share
- 📌 **Bar chart**: ADR per market segment and room type
- 📌 **Line plot + KDE**: Total guest arrivals per day

---

## 📊 Example Visuals

- **Guest Country Map**  
  ![choropleth](https://raw.githubusercontent.com/your-username/hotel-booking-analysis/main/assets/choropleth-example.png)

- **Room Type Comparison**  
  ![room mismatch](https://raw.githubusercontent.com/your-username/hotel-booking-analysis/main/assets/room-mismatch-example.png)

*(Update image paths if you add `assets/` folder with visuals)*

---

## 📦 Technologies

- Python (pandas, numpy)
- Visualization: matplotlib, seaborn, plotly
- Jupyter Notebook

---

## ▶️ Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/hotel-booking-analysis.git
   cd hotel-booking-analysis
