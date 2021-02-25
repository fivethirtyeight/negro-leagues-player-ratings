# negro-leagues-player-ratings
This repo contains the data behind the story [The Negro League Stars That MLB Kept Out — And Is Finally Recognizing](https://projects.fivethirtyeight.com/negro-leagues-mlb/). 

`negro-leagues-player-ratings.csv` contains player ratings for players with either 150 games as a batter or 60 (games + starts) as a pitcher in the Negro Leagues, and active or Hall of Fame non-Negro Leagues MLB players with either 300 games as a batter or 350 (games + starts) as a pitcher. To find similar players for batters and pitchers in the Negro Leagues, we converted their rate statistics — courtesy of [Seamheads.com](http://www.seamheads.com/NegroLgs/) — into values relative to the league average for each season, and then aggregated those into career rates weighted roughly by their wins above replacement (WAR) in each season. For each player pool — either players from the Negro Leagues or non-Negro League MLB players — we generated percentile rankings for each aggregated category.


|   Category   |                                     Description                                     |
|--------------|-------------------------------------------------------------------------------------|
| playerID     | Baseball-Reference or Seamheads player ID tag                                       |
| commonName   | Name of player                                                                      |
| league       | League played — Negro Leagues or non-Negro Leagues MLB                              |
| hof          | 1 if the player is in the Hall of Fame; 0 if not                                    |
| startYear    | First year in league                                                                |
| endYear      | Final year in league                                                                |
| totalGames   | Total games played                                                                  |
| positionWar  | Wins above replacement in their category — whether as a position player or pitcher  |
| averageHit   | Batting average percentile                                                          |
| patience     | Isolated patience (OBP - AVG) percentile                                            |
| power        | Isolated power (SLG - AVG) percentile                                               |
| speed        | Speed score percentile                                                              |
| defense      | Defensive WAR percentile                                                            |
| gameCutoff   | Qualifying cutoff for league/position                                               |
| playerLabel  | Category of player                                                                  |
| shortWar     | WAR per 162 games                                                                   |
| positionCat  | Position played within overall category                                             |
| position     | Overall position —  batter or pitcher                                               |
| careerStarts | Starts as a pitcher                                                                 |
| strikeOuts   | Strikeouts per 9 innings percentile                                                 |
| control      | Fewest walks per 9 innings percentile                                               |
| fip          | Fielding independent pitching percentile                                            |
| whip         | (Walks + Hits)/Innings pitched percentile                                           |
| era          | Earned run average percentile                                                       |
| fact         | Selected factoid about player                                                       |




