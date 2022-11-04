### CSGO Match Winner Prediction

### Description:

- The aim of this project is create a model to predict the winner of professional matches for the popular first person shooter game Counter-Strike Global Offensive.
- The data set contains all recorded official matches played in the past 13 months.
- Models' accuracy typically range from 0.6 to 0.7.
- Different models performed better for different teams

### Process:

- Data scraped from popular website 'HLTV.org'
    1. Game results by each individual map, not series.
    2. Historic team ranks of teams with points
    3. Events' information
- Data cleaned in a manner deemed appropriate. 
- Feature Engineering
- Filter data points based on specified team of interest
- Test five different classification models with newly curated data set
    1. Logistic Regression
    2. K-Nearest Neighbors
    3. Random Forest Classifier
    4. Ada Boost Classifier
    5. Gradient Boosting Classifier

### Project's Potential Pitfalls

Roster Changes
- Unlike some traditional sports like football or soccer, a change in one player is much more significant as it consist of 20% of the lineup.
- The impact may cause a substantial difference in a team's performance.
- Thus, there may be value in introducing a new feature to quantify such a change.

Team Dissolution
- It is possible in CS:GO to drop teams in their entirety and pick up a new roster.
- This compromises the integrity of the data as the team name would not adequately reflect the players that are playing under that banner.

Available features
- Due to the nature of the game, there isn't much useful features to proxy our estimates on.
- For example, shots (on target) & corners for soccer, throw-ins & free throws in basketball, XPM & GPM & wards in Dota 2

Data Availability
- Unable to scrape rank points for teams with an international core NOT in the top 30.
- Essentially making predictions for teams under this category impossible under the current model.

### Goal:

Create prediction model to predict the winner of a game.
 
### Files used:

- events_info.csv -- Data of completed events scraped from website 'hltv.org.
- rank_info.csv -- Each teams' historical rank and points scraped from website 'hltv.org.
- results_info.csv -- Game scores by map scraped from website 'hltv.org.
