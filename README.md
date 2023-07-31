# Youtube API Project

## Authors

- Github: [@camelliale1912](https://www.github.com/camelliale1912)
- Linkedin: www.linkedin.com/in/tra-le-nguyen-huong

## Summary of Project
This Python script utilizes the Google YouTube API to fetch statistics and details for given channels and videos. It preprocesses the data, converts count columns, and performs data visualization using Seaborn and Matplotlib. The visualizations include top/bottom videos by views, scatter plots, and a word cloud of video titles.

## Technical Implementation: Python Code Summary
**Data Retrieval:**
- Utilizes the Google YouTube API client library to interact with the YouTube API.
- Fetches channel statistics, including channel name, subscribers, views, total videos, and playlist ID of uploads.
- Retrieves video IDs from a specified playlist.

**Data Preprocessing:**

- Converts count columns (viewCount, likeCount, favoriteCount, commentCount) to numeric data types.
- Converts the "publishedAt" column to a datetime format.
- Extracts the day of the week from the published date.

**Data Visualization:**

- Uses Seaborn and Matplotlib libraries for data visualization.
- Creates bar plots to show top and bottom videos by view count.
- Creates scatter plots to visualize the relationships between view count and comment count, and view count and like count.
- Generates a word cloud from video titles, removing stopwords.

**NLP Processing:**
- Uses the NLTK library to process natural language text.
- Downloads stopwords and tokenizes video titles.

**Functionality:**

- **get_channel_stats:** Fetches channel statistics from the YouTube API and returns a Pandas DataFrame.
- **get_video_ids:** Retrieves video IDs from a playlist using the YouTube API and returns them as a list.
- **get_video_details:** Fetches video details from the YouTube API and returns a Pandas DataFrame.

## Licensing, Authors, Acknowledgements
Youtube API. Avaiable at https://developers.google.com/youtube/v3
