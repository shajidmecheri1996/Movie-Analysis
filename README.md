# Movie-Analysis
🎬 Movie Dataset Analysis & Visualization
📌 Project Overview

This project focuses on cleaning, transforming, and analyzing a movie dataset to uncover trends related to genres, popularity, and release years. After preprocessing, the dataset is visualized to extract meaningful insights.

🧹 Data Cleaning & Preprocessing
Initial Observations

The dataset contains no NaN values.

The following columns were identified as irrelevant to the analysis and removed:

Overview

Original Language

Poster Url

Data Type & Structural Changes

Release Date was converted to datetime, and only the release year was retained.

Genre values were originally comma-separated strings and required restructuring.

The dataset contains no duplicate records.

Feature Engineering

Vote_Average Categorization
The Vote_Average column was categorized into four groups using a custom categorize_col() function:

Popular

average

below_avg

not_popular

Genre Normalization

The Genre column was split into lists.

The dataframe was exploded so that each movie-genre combination occupies a single row.

Final Dataset Shape

Columns: 6

Rows: 25,793

The dataset is now clean, normalized, and analysis-ready.

📊 Data Visualization

Libraries used:

Matplotlib

Seaborn

These were used to generate visual insights into genre frequency, popularity distribution, and yearly movie production.

🔍 Key Questions & Findings
Q1. What is the most frequent genre in the dataset?

Drama is the most frequent genre.

It accounts for over 14% of all movies among 19+ genres.

Q2. Which genre has the highest votes?

25.5% of the dataset falls under the Popular category (6,520 movies).

Drama again leads, holding over 18.5% of popular movies.

Q3. Which movie has the highest popularity? What is its genre?

Spider-Man: No Way Home

Genres:

Action

Adventure

Science Fiction

Q4. Which movie has the lowest popularity? What is its genre?

The United States

Threads

Genres include:

Music

War

Sci-Fi

History

Q5. Which year had the most filmed movies?

2020 recorded the highest number of movies in the dataset.

🧠 Conclusion

Drama dominates both in frequency and popularity, indicating strong audience demand.

Genre normalization was critical—without exploding genres, these insights would be misleading.

The dataset is now structured well enough to support advanced analysis such as trend modeling or recommendation systems.
