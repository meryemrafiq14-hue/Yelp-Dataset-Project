# Yelp Dataset Analysis Project

A comprehensive data analysis project exploring the Yelp Academic Dataset to extract business insights and provide actionable recommendations.

## Overview

This project analyzes the Yelp Academic Dataset, which contains millions of records about businesses, user reviews, customers, and activity on the Yelp platform. The analysis focuses on:

- Business profiles and location data
- User reviews and ratings
- Customer check-ins and engagement patterns
- Market analysis and business recommendations

## Project Structure

- **`yelp_dataset_analysis.ipynb`** - Dataset exploration and analysis of business, review, user, check-in, and tip data
- **`yelp_recommendations.ipynb`** - Business recommendations based on market analysis
- **`yelp_data_import.ipynb`** - Data import and preprocessing pipeline
- **`sql_queries.ipynb`** - SQL queries for database analysis
- **`sql_queries.html`** - Exported HTML report of SQL analysis

## Dataset Description

The Yelp Dataset includes:

- **Business Data**: Details, location, categories, ratings, hours, and attributes
- **Reviews**: Text, stars, date, user/business links, and vote counts
- **Users**: Profiles, review counts, and social data
- **Check-ins**: Visit activity by date
- **Tips**: Brief user suggestions

## Key Findings

The analysis revealed insights about:

- Market gaps and opportunities in specific restaurant categories
- Peak check-in times and customer engagement patterns
- Attributes that correlate with business success
- Geographic opportunities in underserved neighborhoods
- Operational factors that impact business ratings

## Requirements

### Python Libraries
- pandas
- numpy
- pyodbc (for SQL Server connection)
- kagglehub (for dataset download)

### Setup

1. Clone this repository:
```bash
git clone https://github.com/meryemrafiq14-hue/group15-Project1-YelpData.git
cd group15-Project1-YelpData
```

2. Install required packages:
```bash
pip install pandas numpy pyodbc kagglehub
```

3. Set up Kaggle credentials (if downloading data via kagglehub)

4. For SQL queries, configure database connection settings

## Usage

1. Run `yelp_data_import.ipynb` to import and preprocess the Yelp dataset
2. Explore the data using `yelp_dataset_analysis.ipynb`
3. Execute SQL queries in `sql_queries.ipynb` (requires database connection)
4. Review recommendations in `yelp_recommendations.ipynb`

## Database Setup

This project uses Azure SQL Database for relational analysis. Database connection details should be configured using environment variables:

```bash
export DB_SERVER='your-server.database.windows.net'
export DB_NAME='your_database_name'
export DB_USERNAME='your_username'
export DB_PASSWORD='your_password'
```

Alternatively, you can copy `config.example.py` to `config.py` and configure your database credentials there (make sure `config.py` is in `.gitignore`).



## License

This project is for educational purposes. The Yelp Dataset is subject to Yelp's Dataset License Agreement.

## Author

Meryem Rafiq
