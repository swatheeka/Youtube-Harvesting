**Title:** YouTube Data Harvesting and Warehousing with SQL and Streamlit

**Description:**

This project empowers users to harvest valuable data from YouTube channels, store it persistently in a SQL database, and leverage Streamlit for interactive analysis and visualization. It addresses the need for efficient data collection, warehousing, and exploration of YouTube channel information, video details, and limited comment data.

**Key Skills:**

- Python scripting
- Data Collection using YouTube API
- Streamlit for User Interface Development
- API Integration
- Data Management with SQL

**Domain:**

- Social Media Analytics
- YouTube Channel Insights

**Problem Statement:**

This project tackles the challenge of creating a user-friendly Streamlit application that fulfills the following criteria:

- **Data Retrieval:** Users can effortlessly input a YouTube channel ID and harvest comprehensive data encompassing channel name, subscriber count, total video count, playlist ID, video IDs, likes, dislikes, and limited comments for each video. Google API integration facilitates seamless data acquisition.
- **Data Collection:** Up to 10 distinct YouTube channels can be targeted for data collection, with the harvested data stored in a designated data lake for interim processing.
- **Data Storage Flexibility:** The application offers the option to store the collected data in either a MySQL or PostgreSQL database, catering to user preferences and existing database infrastructure.
- **SQL-Powered Search and Retrieval:** Users can leverage the power of SQL queries to search and retrieve data from the established SQL warehouse. This empowers users to conduct customized data exploration, including joining tables for insightful analyses of combined channel and video details.

**Approach:**

1. **Streamlit App Setup:** Streamlit serves as the foundation for building a user-friendly interface. It facilitates the creation of a simple UI where users can input YouTube channel IDs, view channel details, and choose channels for migration to the SQL data warehouse.
2. **YouTube API Connection:** The Google API client library in Python provides a robust mechanism for connecting to the YouTube Data API. This connection enables the application to retrieve channel and video data effortlessly.
3. **Data Storage and Cleaning:** Once retrieved, the YouTube API data is stored in an appropriate format (e.g., pandas DataFrames) for temporary storage before migrating to the SQL data warehouse. Data cleaning steps might be necessary to ensure data consistency and quality.
4. **Data Migration to SQL Warehouse:** After collecting data for multiple channels, the application seamlessly migrates it to a chosen SQL data warehouse (MySQL or PostgreSQL). This structured storage format facilitates efficient data management and querying.
5. **SQL Data Warehouse Queries:** SQL queries empower users to extract insights from the data warehouse. Users can join tables to retrieve data for specific channels based on their input. Python SQL libraries like SQLAlchemy can aid in interacting with the SQL database.
6. **Data Visualization in Streamlit:** The harvested data, retrieved through SQL queries, is presented back to the user within the Streamlit application. Streamlit's data visualization features enable users to create charts and graphs, fostering interactive data exploration and analysis.

**Overall, this project adheres to a well-defined approach that integrates Streamlit for a user-friendly interface, utilizes the YouTube Data API for data acquisition, leverages a SQL data warehouse for structured storage, empowers users with SQL queries for data exploration, and finally presents the results back within the Streamlit application.**
