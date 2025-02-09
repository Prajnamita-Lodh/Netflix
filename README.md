# Netflix Content Catalog

## Overview

This project analyzes Netflix movies and TV shows using a dataset containing metadata about titles, including genres, release years, ratings, and production details. The insights are visualized in a Power BI report to provide a comprehensive understanding of Netflix's content catalog.
## Files Included

### Netflix xlsx: 
This Excel file contains metadata about Netflix movies and TV shows, split into two sheets:

#### Credits: Information about people involved in the titles, including directors and actors.

#### Titles: Details about movies and TV shows, including title, type, release year, genres, IMDb scores, and more.

### Netflix.pbix: 
#### A Power BI report file that visualizes trends, statistics, and key insights from the dataset.

## Titles Sheet

#### ID: Unique identifier for each title.

#### Title: Name of the movie/TV show.

#### Type: MOVIE or SHOW.

#### Release_year: Year of release.

#### Age_certification: Age rating.

#### Runtime: Duration in minutes.

#### Genres: Genre classification.

#### Production_countries: Country of production.

#### Seasons: Number of seasons (for TV shows).

#### IMDB_score: IMDb rating.

#### TMDB_score: TMDB rating.

## Credits Sheet

#### Person_id: Unique ID for each person involved.

#### ID: Corresponding title ID.

#### Name: Name of the person.

#### Character: Character played (if applicable).

#### Role: Role in the production (e.g., DIRECTOR, ACTOR).

## Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options."column profiling based on entire dataset".
- Step 3 : It was observed that in none of the columns errors & empty values were present except column named "Age_certification" & "IMDB_score" in Titles Sheet and "Character" in Credits Sheet.
- Step 4 : _Capitalized each word_ of ID from the Title Sheet in the Power query.
- Step 5 : To redirect to the Power BI Desktop, click on "Close & Apply" from the File menu of the Power query 
- Step 6 : In the report view, under the Format pane, select the Black colour for _Canvas Background_.
- Step 7 : Visual filters (Slicers) were added for four fields named "Genres", "Release Year", & "Title".

Snap shot of the Slicers:

![Image](https://github.com/user-attachments/assets/ad90f202-1536-4269-a489-55434fb3fd54)

- Step 8 : Four card visuals were added to the canvas, one representing total run time (in hours), average rating of IMDb, movies and shows.

Snap shot of the Card Visuals:

![Image](https://github.com/user-attachments/assets/4758416e-7404-42b9-ab5b-6e9756ce31e0)


- Step 9 : A bar chart was also added to the report design area representing the Content for Top 5 Genres by Type. While creating this visual, field named "Type" was also added to the Legends bucket.

![Image](https://github.com/user-attachments/assets/d3f9d21d-5cb8-4b78-aa57-30a399863197)


- Step 10 : Add "map" functionality is powered by Bing Maps to represent "Production country by runtime". Here US hold the 1st ranking.

Here is the snippet of Bing Maps:

![Image](https://github.com/user-attachments/assets/e5e73a27-f5a7-4236-b91e-a9507d9b1f20)


- Step 11 : In the Report view, insert the line chart for the representation of "Released Content by Type in Each Year". Here plotted the "Release_year" in the X-axis and "Count of Title" in the Y-axis. While creating this visual, field named "Type" was also added to the Legends bucket.

Snap shot of the Line Chart:

![Image](https://github.com/user-attachments/assets/5634f37e-2e75-4e9d-bcff-9c7a4d2a6820)


- Step 12 : Donut chart is added in the Report view to show the count of Movies and Show. In this representation, "Type" was added as the Legends.

Snippet of the Donut Chart:

![Image](https://github.com/user-attachments/assets/e1fc21e3-6de3-46aa-a0af-1a9ccb828c42)


- Step 13 : In the report view, under the insert tab, one text box were added to the canvas. The introductio of Netflix was written in the text box in White colour.

Please see the snippet here:

![Image](https://github.com/user-attachments/assets/a9210173-a818-4301-a306-9bb8b2f8e749)


- Step 14 : In the report view, under the insert tab, using image option company's logo was added to the report design area. 
Here is the Logo:

![Image](https://github.com/user-attachments/assets/9c61735b-a01a-44e4-b535-e4f97f48856a)

 
 - Step 15 : The report was then published to Power BI Service.
 
 
![Image](https://github.com/user-attachments/assets/0a8a76fc-6e4a-41a4-b948-e900d8f23de9)

 
 # Report Snapshot (Power BI DESKTOP)

 
![Image](https://github.com/user-attachments/assets/d8caf682-f5ef-4e14-b640-4c8c0b31f2d0)

# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.


# Conclusion:
The analysis of Netflix's content library provides valuable insights into trends, genre popularity, and audience preferences. From the data, we can see that Netflix consistently produces content across multiple genres, with certain types like comedy and dramas receiving higher IMDb and TMDB ratings. The country-wise distribution shows that the majority of content originates from the US, followed by other significant contributors. Audience prefer the movies rather than the shows. By leveraging this data, Netflix can optimize its content strategy to focus on high-performing genres and target audience preferences more effectively.

