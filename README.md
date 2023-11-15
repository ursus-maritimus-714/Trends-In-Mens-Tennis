# Identifying Performance-Impacting Trends in Men's Professional Tennis (1995-2019)
## Introduction
The goal of this project was to identify and visually describe several major biodemographic trends (pertaining to height and age) in top level men’s professional tennis over the past quarter century, and to conduct cursory exploration of correlates of these trends to player performance. This exploratory data analysis project was conducted as a first step in conceiving the framework for a machine learning-based match outcome prediction project, a summary of which can be found [here](https://github.com/ursus-maritimus-714/Mens-Tennis-Prediction#readme).

## Methods
The primary data source was a ~100,000 match subset over a quarter-century (1996-2019) of [Jeff Sackmann's Association of Men's Tennis Professionals (ATP) data archive](https://github.com/JeffSackmann/tennis_atp). This primary source was supplemented with additions and corrections obtained directly from the [ATP data site](https://www.atptour.com/en/scores/results-archive). This large set of match records was filtered down to those contested between the top 200 players in the ATP rankings at any given time step (start of week) in the sample. All main tour matches played on either hard (~68% of total) or clay courts (~28%) were included in the exploratory data analysis (grass court, Davis Cup, and Olympics matches were removed). 

For some analyses, players were filtered into 1 of 4 'Rankings Tiers' at each time step. Tier 1= 1-25 ('Elite Players'), Tier 2 = 26-50 ('Quasi-Elite Players'; usually obtaining direct entry to all Grand Slams and main tour events), Tier 3= 51-125 ('Main Tour Regulars'; usually obtaining direct entry into Grand Slams and lower and mid-tier main tour events), Tier 4 = 126-200 ('Minor Leaguers' sometimes obtaining entry into Grand Slams and lower and mid-tier main tour events via upfront qualifying tournaments).    

All data manipulation, processing, and analyses were conducted in the Python/Pandas environment and documented with Jupyter Notebooks (anaconda3).

## Key Results

1) Mean player height steadily increased over the sample interval (**Figure 1**). Taller players became overrepresented in Tier 1 ('Elite Players') relative to other ranking tiers, though the entire height curves for each of Tier 1-Tier 3 have shifted to the right over time (**Figure 2**).

Figure 1. 


