📊 Hotel Booking Demand Analysis
This project performs Exploratory Data Analysis (EDA) on the hotel_bookings.csv dataset. The goal is to understand booking patterns, customer behavior, and operational insights such as cancellations, room assignments, and guest demographics.

📁 Dataset Overview
The dataset contains 119,390 rows and 32 columns related to bookings for two types of hotels:

City Hotel

Resort Hotel

Key columns include:

is_canceled

lead_time

arrival_date_year, month, day

adults, children, babies

adr (Average Daily Rate)

country

reserved_room_type, assigned_room_type

market_segment

reservation_status, etc.

✅ Project Highlights
1. 🧼 Data Cleaning
Removed bookings with zero guests (adults + children + babies == 0)

Removed duplicate rows

Handled missing values (children, country, agent, company)

2. 📈 Descriptive Statistics
Summary of lead_time, adr, and total_of_special_requests

Memory usage comparison with memory_usage='deep'

3. 📊 Feature Distribution (Quantiles)
Computed 90th–100th percentile values for key features

Bug Fix: Quantile computation was corrected to i/100 from 1/100

4. 🌍 Where Do the Guests Come From?
Visualized using a Plotly Choropleth Map based on country field

Only included non-canceled bookings

5. 🛏️ Reserved vs Assigned Room Analysis
Cross-tabulation to assess mismatch rate between reserved and assigned room types

6. 📊 Market Segment Analysis
Pie chart showing distribution of market segments

Bar plot comparing ADR across segments and reserved room types

7. 📅 Guest Arrivals Over Time
Combined year, month, and day to create a proper arrival_date

Total guests = adults + children + babies

Line plot showing guest arrival trends

KDE plot of daily total guest arrivals

📦 Libraries Used
pandas

numpy

matplotlib

seaborn

plotly and chart_studio


📬 Contact
For questions or suggestions, feel free to reach out to the project contributor.
