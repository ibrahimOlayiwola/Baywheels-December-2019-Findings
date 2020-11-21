# Baywheels-December-2019-Findings

Bay Wheels is a regional public bicycle sharing system in California's San Francisco Bay Area. It is operated by Motivate in a partnership with the Metropolitan Transportation Commission and the Bay Area Air Quality Management District.Bay Wheels is the first regional and large-scale bicycle sharing system deployed in California and on the West Coast of the United States. It was established as Bay Area Bike Share in August 2013. As of January 2018, the Bay Wheels system had over 2,600 bicycles in 262 stations across San Francisco, East Bay and San Jose.
This project analyzes Lyft's bikeshare, bay wheels, in the San Francisco Bay Area for the month of December 2019.

## Files in this repository.
This repository contains 8 files. The contents of the files are explained below.
#### .ipynb_checkpoints
This folder contains two files which are:
1. bay_wheels_exploration-checkpoint.ipynb: The checkpoints of the notebook used for the analysis.
2. bay_wheels_slide_deck-checkpoint.ipynb: The checkpoints of the notebook used to create the slide deck.
#### 201912-baywheels-tripdata.csv
This contains the raw data of the trips taken in the Bay area of California during the month of December 2019.
##### Dataset Summary

> The dataset consist of 150102 rows and 14 columns.
- **duration_sec:** This is the trip duration in seconds.
- **start_time:** This column tells us the start time and date of the trip.
- **end_time:** This is the end time and date of the trip.
- **start_time_day:** The day of the week the trip was started.
- **end_station_id:** The identification number of the station the trip ended.
- **start_station_name:** The name of the station the trip was started.
- **end_station_name:** The name of the station the trip ended.
- **start_station_latitude** and **start_station_longitude:** Address of the start station on a GPS.
- **start_date:**  The date of the month the trip was started/booked.
- **Bike_id:** Identification number of the bike.
- **User_type:** A user's status (Either a subcriber or a customer).
- **duration_min:** The duration of trip in minutes.

#### df_master.csv
The final dataset after the analysis has been done.

#### output_toggle.tpl
This is a file used to convert ipython notebook to html file.

#### bay_wheels_slide_deck.slides.html
A summary of the findings of the analysis in slides.

### bay_wheels_exploration.ipynb
The notebook used for the analysis.
##### Subsections of the Analysis
1. **Preliminary Wrangling:** In this section, the python packages used for the analysis are imported, the dataset is previewed by checking details like the number of rows and columns, names of the colums etc.
2. **Assessing Data:** This aspect is divided into two, the visual assessment using a spreadsheet (Google sheets) and the programmatic assessment in the notebook. In the programmatic assessment, the number of unique users, average time of trip duration, types of users, the datatypes of the columns are noted. Also, some improvements to be made to the dataset were noted.
3. **Cleaning Data:** In cleaning of the dataset, a copy of the original dataset is made and worked upon thereby safeguarding the raw dataset. 
The improvements to be made that were noted in the assessment sections were implemented in this section.
4. **Main Interests:** The main interest of the analysis - the time most trips are taken in referece to the days of the week and how factors like the duration of the trip, user type, affect the the time- was defined.
5. **Univariate Exploration:** Exploration involving one variable. The investigation covered the following
- Average usage of Bay Wheels by Day of week.
- Average Hourly usage of Bay Wheels in a day.
- Count of Trip Duration in minutes.
- Percentage of User Types of Bay Wheels.
- Distrubution of Trips for the Month (each day).
6. **Bivariate Exploration:** Exploration involving two variables. The variables investigated includes
- Average Number of Trips by Days of Week based on User Type.
- Duration of Trips for Each Day of the month.
- Count of Trip Duration (Minutes) based on User Type.
7. **Multivariate Exploration:** Exploration involving more than two variables.
- Average Duration of Trips based on Days of Week and User Type.
- Daily Duration of Trips by User Type.
- Daily Average Duration of Trips by User Type.
8. **Findings on the analysis:** This section reports the observations based on the analysis conducted.
9. Suggestions on further analysis.

After the analysis, the cleaned dataset used for the analysis was saved as a csv file.

