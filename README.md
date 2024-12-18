<h1>1. Initialization and Setup</h1>
Library Installation and Imports:
Installs pyspark, indicating the use of Apache Spark for distributed data processing.
Imports essential libraries such as pandas, matplotlib, numpy, and collections.Counter.
<h1>2. Data Loading</h1>
Spark DataFrame:
A Spark session is initialized using SparkSession.builder.
Loads the Netflix dataset into a Spark DataFrame, with schema inferred automatically.
Displays the schema and the first five rows of the dataset.
Counts the total rows in the dataset.
<h1>3. Handling Missing Data</h1>
Null Values:
Calculates the number of null values in each column using Spark SQL functions.
This helps in understanding the completeness of the dataset.
<h1>4. Descriptive Analysis</h1>
Summary Statistics:
Generates descriptive statistics for numerical columns.
Lists distinct values in categorical columns like type and rating.
<h1>5. Content Distribution Analysis</h1>
Data Aggregation:
Groups data by type (e.g., TV Shows or Movies) to calculate and display the count of each category.
Extracts year_added from date_added and groups data by year to analyze trends over time.
<h1>6. Genre and Rating Analysis</h1>
Genres:
Splits the listed_in column into individual genres using Spark’s explode and split functions.
Aggregates and ranks genres by frequency.
Ratings:
Groups data by rating to calculate and display the count for each rating category.
<h1>7. Analysis of Key Contributors</h1>
Top Directors and Actors:
Lists top directors by frequency of their content.
Splits the cast column into individual actors and ranks them by frequency.
<h1>8. Visualization</h1>
Converts the Spark DataFrame to a Pandas DataFrame for enhanced visualization using matplotlib.
Key Graphs:
Content Distribution by Year:
Bar chart showing the distribution of content by release year.
Content Type Distribution:
Pie chart displaying proportions of TV Shows and Movies.
Rating Distribution:
Bar chart visualizing the count of different content ratings.
Top 10 Genres:
Bar chart highlighting the most frequent genres in Netflix content.
Content Duration:
Histogram showing the distribution of content duration (in minutes for movies and seasons for TV shows).
<h1>9. Data Cleaning and Transformation</h1>
Duration Conversion:
Custom function to convert duration (e.g., "1h 30m", "2 Seasons") into numeric values (minutes or seasons).
Handles various formats and errors gracefully.
Plot Duration Distribution:
Visualizes the distribution of content duration using a histogram.
