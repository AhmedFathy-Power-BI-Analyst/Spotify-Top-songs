# Spotify-Top-songs
# Music Dataset Analysis with DAX Measures

## Overview

This project involves the analysis of a music dataset using Data Analysis Expressions (DAX) measures in Power BI. The dataset contains information about various attributes of songs such as BPM, energy level, danceability, and more. This README provides a summary of the key insights derived from the dataset along with corresponding DAX measures.

## Key Insights and DAX Measures

1. **Total Number of Songs:**
   - DAX Measure: `Total Songs = COUNTROWS('Case Study Table')`
   - Description: Provides the total count of songs in the dataset.

2. **Average Beats per Minute (BPM):**
   - DAX Measure: `Average BPM = AVERAGE('Case Study Table'[bpm])`
   - Description: Calculates the average BPM (beats per minute) of songs in the dataset.

3. **Average Energy Level:**
   - DAX Measure: `Average Energy = AVERAGE('Case Study Table'[nrgy])`
   - Description: Calculates the average energy level of songs in the dataset.

4. **Average Danceability:**
   - DAX Measure: `Average Danceability = AVERAGE('Case Study Table'[dnce])`
   - Description: Calculates the average danceability score of songs in the dataset.

5. **Average Decibels (dB):**
   - DAX Measure: `Average Decibels = AVERAGE('Case Study Table'[dB])`
   - Description: Calculates the average decibel level of songs in the dataset.

6. **Average Live Performance Score:**
   - DAX Measure: `Average Live Performance = AVERAGE('Case Study Table'[live])`
   - Description: Calculates the average live performance score of songs in the dataset.

7. **Average Valence (Positivity):**
   - DAX Measure: `Average Valence = AVERAGE('Case Study Table'[val])`
   - Description: Calculates the average valence (positivity) score of songs in the dataset.

8. **Average Duration of Songs:**
   - DAX Measure: `Average Duration = AVERAGE('Case Study Table'[dur])`
   - Description: Calculates the average duration of songs in the dataset.

9. **Average Acousticness:**
   - DAX Measure: `Average Acousticness = AVERAGE('Case Study Table'[acous])`
   - Description: Calculates the average acousticness score of songs in the dataset.

10. **Average Speechiness:**
    - DAX Measure: `Average Speechiness = AVERAGE('Case Study Table'[spch])`
    - Description: Calculates the average speechiness score of songs in the dataset.

11. **Total Number of Pop Songs:**
    - DAX Measure: `Total Pop Songs = CALCULATE(COUNTROWS('Case Study Table'), 'Case Study Table'[top genre] = "pop")`
    - Description: Provides the total count of songs categorized as pop genre.

12. **Total Number of Songs by Artist:**
    - DAX Measure (replace "Artist Name" with the actual name of the artist): 
      ```
      Total Songs by Artist = CALCULATE(COUNTROWS('Case Study Table'), 'Case Study Table'[artist] = "Artist Name")
      ```
    - Description: Provides the total count of songs by a specific artist.

## Usage

To use these DAX measures:
1. Import the music dataset into Power BI.
2. Create a new DAX measure for each insight using the provided expressions.
3. Utilize these measures in Power BI visuals and reports to gain insights into the music dataset.

