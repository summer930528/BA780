# Do Higher Hospitality Wages Lead to Better Hotel Ratings?

This is the final project for **BA780: Introduction to Data Analytics**. Team B07 examines whether U.S. states with higher hospitality wages also have better hotel ratings, and what guests mention in lower-rated reviews.

## Research question

Are higher hospitality wages associated with higher hotel ratings? We also compare ratings with room-condition complaints, such as cleanliness, pests, odors, smoke, and broken or outdated rooms.

## Project files

- `B07-Do-Higher-Hospitality-Wages-Lead-to-Better-Hotel-Ratings (1).ipynb` — data cleaning, analysis, charts, findings, and conclusions.
- `BA780 - Higher Hospitality Wages, Better Hotel Guest Satisfaction_ (1).pptx` — presentation of the project and its main findings.

## Data sources

The notebook uses three hotel-review CSV files and one wage workbook:

| File | Contents |
| --- | --- |
| `Datafiniti_Hotel_Reviews.csv` | 10,000 hotel review records |
| `Datafiniti_Hotel_Reviews_Jun19.csv` | 10,000 hotel review records |
| `7282_1.csv` | 35,912 hotel review records; the exact source and rating scale need confirmation |
| `780_data_wages_01.xlsx` | 434,473 occupational wage records |

The project identifies the Datafiniti hotel-review dataset on [Kaggle](https://www.kaggle.com/datasets/datafiniti/hotel-reviews) and the wage data as May 2013 [U.S. Bureau of Labor Statistics Occupational Employment and Wage Statistics](https://www.bls.gov/oes/tables.htm). The original data files are not included in this repository. Check the dataset documentation and terms before reusing the files, especially the legacy `7282_1.csv` file.

## Main findings

- The main state-level comparison includes 42 states with at least 100 reviews. Average hospitality wages had almost no correlation with average hotel ratings (**r = -0.03**).
- Room-condition complaints had a stronger negative correlation with state ratings (**r = -0.89**). Cleanliness was among the most common complaints in low-rated reviews.
- Average ratings in the yearly analysis stayed between **3.68 and 3.82** from 2011 to 2016.

These are associations in the available data. They do not show that wages or complaints caused a change in ratings. The review files cover a sample of hotels, wage data is from 2013, and keyword matching may miss complaints or classify a mention without understanding its context.

## How to run the notebook

1. Open the notebook in Google Colab or Jupyter.
2. Place the four source data files in the notebook's working folder. In Colab, upload them using the Files panel or the notebook's upload cell.
3. Run the cells from top to bottom. The notebook creates cleaned data and analysis outputs in `hotel_cleaning_outputs` and `Hotel_Reviews_Cleaned_Results.zip`.

The notebook uses Python with pandas, NumPy, Matplotlib, Seaborn, and openpyxl. It notes pandas 2.0 or later as a requirement. Exact download links and access dates for the supplied source files should be recorded by the team when available.

## Team B07

Anna Zvanskaya, Paula Vasques, Pushan Parihr, Summer Kao, and Sharanya Srinivas.
