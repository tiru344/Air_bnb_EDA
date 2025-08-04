# Airbnb Listings EDA Project: New York 2024  

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-green)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📊 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on New York Airbnb data to uncover trends and patterns in rental listings. Using Python data science libraries including **Pandas, NumPy, Matplotlib, and Seaborn**, we analyze pricing strategies, neighborhood trends, and host behaviors to provide actionable insights for both guests and hosts.

---

## 🎯 Objectives
- Analyze **room types, prices, and availability** across different NYC neighborhoods
- Understand **host behavior** and listing distribution patterns  
- Identify and handle **price outliers** in the dataset
- Extract **geographic insights** from borough-level data
- Provide data-driven recommendations for guests and hosts

---

## 📋 Dataset Description
**Dataset Size**: 20,765 entries with 22 features

### Key Features:
| Feature | Description |
|---------|-------------|
| `id` | Unique identifier for each listing |
| `name` | Title/name of the Airbnb listing |
| `host_name` | Name of the property host |
| `neighborhood_group` | NYC borough (Manhattan, Brooklyn, Queens, Bronx, Staten Island) |
| `latitude/longitude` | Geographic coordinates of listings |
| `price` | Nightly rental price in USD |
| `room_type` | Accommodation type (Entire home/apt, Private room, Shared room) |
| `reviews_per_month` | Average monthly review count |
| `availability_365` | Available days per year |

---

## 🔄 Project Workflow

### 1. 🧹 Data Cleaning & Preprocessing
- **Missing Value Treatment**: Handled null values in `price`, `neighborhood`, and `beds` columns
- **Data Type Conversion**: Converted `last_review` to datetime format
- **Outlier Management**: Applied price capping at $1,000 to prevent visualization skewing
- **Data Validation**: Ensured data consistency and logical constraints

### 2. 🔍 Exploratory Data Analysis

#### Price Analysis
- **Borough-wise pricing**: Manhattan leads with highest average prices
- **Room type pricing**: Entire homes command premium rates
- **Price distribution**: Most listings fall within $50-$300 range

#### Geographic Insights  
- **Neighborhood clustering**: Identified high-density listing areas
- **Borough comparison**: Analyzed listing distribution across NYC boroughs
- **Location-price correlation**: Mapped geographic factors to pricing trends

#### Host Behavior Analysis
- **Multi-listing hosts**: Identified professional vs. casual hosts
- **Host performance metrics**: Analyzed review patterns and availability management
- **Market concentration**: Examined host market share distribution

### 3. 📈 Data Visualization Techniques
- **Correlation Heatmaps**: Feature relationship analysis
- **Distribution Plots**: Price and availability patterns
- **Categorical Analysis**: Room type and borough comparisons  
- **Outlier Detection**: Box plots for price anomaly identification
- **Pair Plots**: Multi-dimensional relationship exploration

---

## 🔍 Key Findings

### 💰 Pricing Insights
- **Manhattan** commands the highest prices (average: $X)
- **Entire homes/apartments** are 2-3x more expensive than private rooms
- **Price outliers** above $1,000 represent <1% of listings

### 🏠 Room Type Distribution
- **Entire homes/apartments**: 52% of listings
- **Private rooms**: 45% of listings  
- **Shared rooms**: 3% of listings

### 📍 Geographic Patterns
- **Manhattan**: Highest density but most expensive
- **Brooklyn**: Best value proposition for budget travelers
- **Queens**: Emerging market with growth potential

### 📊 Market Dynamics
- **High availability** correlates with competitive pricing
- **Professional hosts** (3+ listings) dominate prime locations
- **Review frequency** positively impacts booking rates

---

## 🚀 Getting Started

### Prerequisites
```bash
Python 3.8+
Jupyter Notebook
```

### Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/[YOUR-USERNAME]/airbnb-nyc-eda-2024.git
   cd airbnb-nyc-eda-2024
   ```

2. **Install required packages**:
   ```bash
   pip install -r requirements.txt
   # OR
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch the analysis**:
   ```bash
   jupyter notebook airbnb_eda_analysis.ipynb
   ```

### 📁 Repository Structure
```
├── data/
│   ├── raw/                 # Original dataset
│   └── processed/           # Cleaned data
├── notebooks/
│   └── airbnb_eda_analysis.ipynb
├── visualizations/          # Generated plots and charts
├── src/                     # Helper functions and utilities
├── requirements.txt
└── README.md
```

---

## 💡 Recommendations

### 🧳 For Guests
- **Budget travelers**: Consider private rooms in Brooklyn or Queens
- **Quality seekers**: Look for listings with 4+ reviews/month and high availability
- **Location matters**: Manhattan premium justified for business/tourism access

### 🏡 For Hosts
- **Pricing strategy**: Research neighborhood benchmarks before setting rates
- **Availability optimization**: Maintain 70%+ availability for better visibility
- **Review management**: Respond to reviews promptly to build credibility
- **Room type consideration**: Entire homes generate higher revenue per booking

---

## 🔮 Future Enhancements
- [ ] **Machine Learning**: Price prediction model using regression algorithms
- [ ] **Sentiment Analysis**: NLP analysis of guest reviews and feedback
- [ ] **Interactive Dashboard**: Real-time data visualization using Plotly Dash
- [ ] **Time Series Analysis**: Seasonal booking pattern analysis
- [ ] **Geospatial Analysis**: Advanced mapping with Folium integration

---

## 📈 Results & Impact
This analysis provides data-driven insights that can help:
- **Guests** make informed booking decisions and find optimal value
- **Hosts** optimize pricing strategies and improve listing performance  
- **Researchers** understand short-term rental market dynamics in NYC

---

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

---

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 📬 Contact & Connect
- **GitHub**: [@your-username](https://github.com/your-username)
- **LinkedIn**: [Your LinkedIn Profile](https://linkedin.com/in/your-profile)
- **Email**: your.email@example.com

---

## 🙏 Acknowledgments
- Dataset source: [Inside Airbnb](http://insideairbnb.com/)
- Inspiration from the data science community
- Special thanks to contributors and reviewers

---

⭐ **If you found this project helpful, please consider giving it a star!** ⭐
