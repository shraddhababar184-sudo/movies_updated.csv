
# Dataset Overview: movies_updated.csv
This dataset contains detailed information about movies, likely sourced from similar database. It includes metadata such as titles, genres, ratings, and financials. Here's a breakdown of its structure and key insights:

## Key EDA Insights
- Missing Values:
- budget, gross, and score have missing values.
- Consider imputing or dropping rows depending on your analysis goals.
- Data Types:
- budget and gross may be stored as strings with symbols (e.g., $, ,) — these need cleaning and conversion to numeric.
- released is a string and should be converted to datetime for temporal analysis.
- Top Genres:
- Common genres include Action, Drama, Comedy, Thriller, and Adventure.
- You can use .str.get_dummies() on genre for multi-label classification or genre-based analysis.
- Rating Distribution:
- IMDb ratings are typically between 1 and 10, with most movies clustering between 6.0 and 8.0.
- Budget vs Gross:
- A scatter plot of budget vs gross can reveal profitability trends.
- Correlation analysis often shows a moderate to strong positive correlation between budget and gross.
- Top Directors and Stars:
- You can group by director or star and aggregate gross or rating to find top performers.
- Temporal Trends:
- Analyzing year or released can show trends in genre popularity, average ratings, or budget inflation over time.

