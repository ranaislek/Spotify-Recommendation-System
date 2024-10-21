# Spotify Song &amp; Genre Analysis, Popularity Prediction and Building a Simple Recommendation System
My very first data science project <3
## CS210 - Introduction to Data Science Sabancı University 2020-2021

<div align="center">
    <img src="https://sabanciuniv.edu/themes/custom/su/logo.svg" alt="SU Logo" width="300"/>
</div>

<br>

This project analyzes Spotify data from the years 1921-2020, featuring over 160,000 tracks. The main goal is to explore the dataset, perform data analysis, and build a basic song recommendation system using similarity metrics and nearest neighbors methods.

## Project Overview
The project is divided into multiple stages:
- **Data Loading & Preprocessing**: The dataset is read and processed to ensure there are no missing values.
- **Exploratory Data Analysis (EDA)**:
  - Visualization of descriptive statistics and correlation analysis between song features.
  - Analysis of the most popular artists, songs, and changes in music trends over time.
- **Modeling & Song Recommendation**:
  - Creation of a song recommendation system using features like acousticness, danceability, and energy.
  - Implementation of similarity metrics and Nearest Neighbors to suggest songs based on given input.

## Dataset
The dataset, **Spotify Dataset 1921-2020, 160k+ Tracks**, is available on [Kaggle](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks). It contains a comprehensive sample of songs, along with aggregated data by artists, years, and genres.

## Key Findings from EDA
- **Correlation Analysis**: Identified relationships between features such as energy, danceability, and popularity.
- **Trends Over Time**: Analyzed how musical features evolved over different decades, providing insights into the changing nature of popular music.
- **Popular Artists & Songs**: Highlighted the top artists and tracks based on various metrics like popularity and tempo.

## Song Recommendation System
The recommendation system utilizes the following:
- **Features**: Acousticness, danceability, duration, energy, instrumentalness, key, liveness, mode, speechiness, tempo, valence.
- **Normalization**: Data is normalized before applying similarity metrics.
- **Recommendation Algorithm**: Uses Nearest Neighbors to suggest similar songs based on user input.

## Technical Details
- **Libraries**: Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn.
- **Data Preprocessing**: Includes normalization, handling of missing values, and feature selection.
- **Modeling**: Implemented similarity-based recommendations using `KNeighborsClassifier` from Scikit-learn.

## Setup & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spotify-data-analysis.git
   cd spotify-data-analysis
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook to explore the data and use the recommendation system:
   ```bash
   jupyter notebook Group_Id_73_Rana_Islek_Presentation.ipynb
   ```

## Example Usage
- Visualize the correlation between song features:
  ```python
  # Example code to plot correlation
  sns.heatmap(data.corr(), annot=True, cmap='coolwarm')
  ```
- Get song recommendations based on a selected song:
  ```python
  # Example code for recommendation
  recommended_songs = recommend_song(input_song_features)
  print(recommended_songs)
  ```

## Acknowledgements
Special thanks to the teaching assistant for their guidance throughout the project. Despite some challenges, the project was completed with a focus on detailed analysis and functional implementation.
