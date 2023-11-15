# Identifying Performance-Impacting Trends in Men's Professional Tennis (1995-2019)
## Introduction
The goal of this project was to identify and visually describe several major biodemographic trends (pertaining to height and age) in top level men’s professional tennis over the past quarter century, and to conduct cursory exploration of correlates of these trends to player performance. This exploratory data analysis project was conducted as a first step in conceiving the framework for a machine learning-based match outcome prediction project, a summary of which can be found [here](https://github.com/ursus-maritimus-714/Mens-Tennis-Prediction#readme).

## Methods
The primary data source was a ~60,000 match subset over a quarter-century (1996-2019) of [Jeff Sackmann's Association of Men's Tennis Professionals (ATP) data archive](https://github.com/JeffSackmann/tennis_atp). This primary source was supplemented with additions and corrections obtained directly from the [ATP data site](https://www.atptour.com/en/scores/results-archive). This large data set was organized by player (2 records per match), and was then filtered down to player records for the top 200 players in the ATP rankings at any given time step (start of week) in the sample (~119.5K records). All main tour matches contested on either hard (~68% of total) or clay courts (~28%) were included in the analysis (grass court, Davis Cup, and Olympics matches were removed). 

For some analyses, players were filtered into 1 of 4 ranking tiers at each time step. Tier 1= 1-25 ('Elite Players'), Tier 2 = 26-50 ('Quasi-Elite Players'; usually obtaining direct entry to all Grand Slams and main tour events), Tier 3 = 51-125 ('Main Tour Regulars'; usually obtaining direct entry into Grand Slams and lower and mid-tier main tour events), Tier 4 = 126-200 ('Minor Leaguers' sometimes obtaining entry into Grand Slams and lower and mid-tier main tour events via upfront qualifying tournaments).    

All data manipulation, processing, and analyses were conducted in the Python/Pandas environment and documented with Jupyter Notebooks (anaconda3).

## Key Results

1) Mean player height across ranking tiers increased steadily over the sample interval (**Figure 1**). This mean increase was accomplished with a loss of players under ~175 cm and the introduction of a number of players above 190 cm (green arrow in Panel B). 
Taller players became overrepresented in Tier 1 ('Elite Players') relative to other rankings tiers (blue arrow in Panel C), though the height curves for each of Tier 1-Tier 3 right-shifted over time (**Figure 2**).

**Figure 1. Height Representation on the ATP Main Tour Over Time**

![image](https://github.com/ursus-maritimus-714/Trends-In-Mens-Tennis/assets/90933302/11acb8ca-6837-4930-acd5-aa10b13486c7)

**Figure 2. Height Representation on the ATP Main Tour Over Time By Ranking Tier**

![image](https://github.com/ursus-maritimus-714/Trends-In-Mens-Tennis/assets/90933302/d0e9aa50-f212-4b8b-ba48-dd214b01ade7)

2) Along with player height, player serve performance (as measured by mean serve points win% per player, per match) also improved over the sample interval across ranking tiers (**Figure 3**). Performance improved on both clay and hard courts, but perhaps moreso on clay courts over the past ~10 years (Panel B). Nonetheless, because ~70% of tour matches are played on hard courts, most of the analysis moving forward will focus on hard court performance over time.

**Figure 3. Serve Performance on the ATP Main Tour Over Time, Overall and by Playing Surface**

![image](https://github.com/ursus-maritimus-714/Trends-In-Mens-Tennis/assets/90933302/ba8c52e2-2aee-474c-b91d-d748c7ed228d)

3) Height and player serve performance are positively correlated across the sample, both overall on each surface (**Figure 4**) and across rankings tiers on both surfaces (**Figure 5**; hard court data shown in Panel B).

**Figure 4. Correlation Between Height and Serve Performance by Playing Surface on the ATP Main Tour**

![image](https://github.com/ursus-maritimus-714/Trends-In-Mens-Tennis/assets/90933302/95046b5a-deaf-404b-9f63-6df4d5f139f5)
*Each data point represents one Top 200 player’s mean performance for a given sample year on hard courts.*

**



