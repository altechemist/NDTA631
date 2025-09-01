
# Mobile Money in Motion: Sending vs Withdrawing Patterns in South Africa and Beyond

## Assessment Information

- **Assessment:** Group Assignment (NDTA 631)
- **Programme:** Diploma in ICT
- **Module Code:** NDTA 631
- **Module Description:** Data Analysis and Visualization
- **Examiner(s):** Melvin Kisten
- **Group Size:** 6–7 students

## Project Overview

This project explores financial inclusion through the lens of mobile money. Using World Bank Findex datasets, we compare sending money and withdrawing money from mobile money accounts, focusing on South Africa and placing findings in a global context.

**Central Research Question:**
> Do South Africans and global populations use mobile money primarily to send funds, withdraw funds, or both—and how does this vary by gender, region, and over time?

## Datasets Used

- `WB_FINDEX_FIN13BM.csv`: Sent money from a mobile money account, monthly
- `WB_FINDEX_FIN13CM.csv`: Took out money from a mobile money account, monthly
	- Source: World Bank Open Data

## Folder Structure

```
NDTA631/
├── README.md                # Project documentation
├── requirements.txt         # Python dependencies
├── data/
│   ├── raw/                 # Raw World Bank Findex CSVs
│   │   ├── WB_FINDEX_FIN13BM.csv
│   │   └── WB_FINDEX_FIN13CM.csv
│   └── proccessed/          # Cleaned/processed data
├── notebooks/
│   ├── 01_data_preparation.ipynb
│   ├── 02_numerical_analysis.ipynb
│   ├── 03_visualization.ipynb
│   ├── 04_database_integration.ipynb
│   └── 05_data_analysis.ipynb
├── reports/                 # Final report and outputs
```

## Project Workflow

### Data Loading & Cleaning
- Import datasets using Pandas
- Merge on country, year, and demographic fields
- Handle missing values, renaming, filtering for South Africa

### Data Preparation
- Create combined features (send vs withdraw ratios)
- Segment data by gender and region

### Exploratory Data Analysis (EDA)
- Summary statistics
- Correlations between send/withdraw

### Database Integration
- Store cleaned data in SQLite
- Perform queries for regional comparisons

### Visualization & Insights
- Bar charts: South Africa vs Africa vs Global
- Scatter plot: Sending vs Withdrawing (by country)
- Heatmaps: Regional mobile money intensity
- Gender gap plots

### Report Writing (7–9 pages)
- Introduction & objectives
- Methodology
- Key findings with charts
- Recommendations for financial inclusion policies

## Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Database:** SQLite
- **Version Control:** Git & GitHub


## Execution Instructions

1. **Clone this repository:**
	```sh
	git clone https://github.com/<your-group>/mobile-money-analysis.git
	cd mobile-money-analysis
	```
2. **Create a virtual environment & install dependencies:**
	```sh
	python -m venv venv
	# On Mac/Linux
	source venv/bin/activate
	# On Windows
	venv\Scripts\activate
	pip install -r requirements.txt
	```
3. **Run the Jupyter Notebook or Python script:**
	```sh
	jupyter notebook analysis.ipynb
	# OR
	python analysis.py
	```

## Optional Deliverable

- Video Demo: Walkthrough of analysis and visualizations

## Contributors

Full Names & Student Numbers of Group Members (6–7 students)
Keabetswe	 Moloi	202112865
Thakasa 	Gumede	202204383
Akanyang	 Maine	202213306
Princess 	Tau	202109551
Karabelo 	Nthoroane	202328762
Tshepang	Matamela	202325467
Amukelani	Rikhotso	202212514
