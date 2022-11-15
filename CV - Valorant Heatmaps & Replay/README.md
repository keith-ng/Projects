### Project X - Valorant Match Analyses (VCT Champions 2022 - Istanbul)

Hosted on Streamlit: [Check it out here](https://keith-ng-vct-analysis-overview-gm5wxq.streamlit.app/replay_system)

### TLDR:

- Extracted positional data of over 10 object classes from videos using YOLOv7
- Obtained information from over 20 data points using optical character recognition and computer vision
- Combined and cleaned both datasets before generating movement heatmaps using a density plot
- Created a replay system with features that address current pain points verified by KOLs

![Alt text](assets/example.PNG?raw=true "Optional Title")

### Description:

- As a veteran FPS gamer who currently plays Valorant, I find the current features offered by existing analytics & insights platforms lacking.
- This project seeks to bridge this gap and hopefully move this market segment towards a more exhaustive product offering by such platforms.

- It uses video analysis to gain insights into the strategies and playstyles of professional Valorant teams. 
    - The scope of games will tentatively be limited to the Valorant Tournament: VCT Champions 2022 - Istanbul.
- These insights can be interpreted through the display of movements, heatmaps, and a pseudo-replay system provided by this project.
    - The pseudo-replay system also provides an ability tracker that includes the abilities that were casted at the specified second including the past two seconds for reference.

### Challenges:

- Image Annotation
    - Objects of interest are not generic and had to be annotated from scratch.
    - Images are small, requiring the annotations to be precise which is time-consuming.
    - Due to nature of the images, there are many occluded images.

- Data Cleaning
    - Each data point is not 'independent' meaning some null values cannot be dropped without harming the integrity of the dataset.
        - This results in the necessity of extremely intensive data cleaning.
    - Images cleaning require various image preprocessing techniques in order to obtain a respectable accuracy.

### Limitations:

- Occluded Images
    - Input data have no means of identifying object that are significantly occluded
        - This occurrence however, is expected given the nature of the game Valorant.
            1. Grouping up as a team
            2. Maps with 'floors' (multiple spots from a vertical perspective)

### Future Improvements

1. Include Agent 'Astra' Abilities
2. More Matches
3. Introduce new relevant objects
    1. Abilities' Locations
    2. Ultimate Ability Tracker
    3. Through Offical API
        - Kill Feed
        - Round Economy
4. Larger Training Dataset of Images
    - inc. Parameter Tuning if necessary
 
### Files used:

- liq_lev_m1_md_final.csv -- Cleaned match data from Liquid vs Leviathan map 1.
- liq_lev_m1_pl_final.csv -- Cleaned location data from Liquid vs Leviathan map 1.
- liq_lev_m2_md_final.csv -- Cleaned match data from Liquid vs Leviathan map 2.
- liq_lev_m2_pl_final.csv -- Cleaned location data from Liquid vs Leviathan map 2.

### License:

- GNU General Public License v3.0

### Project Status:
- On Hiatus.
