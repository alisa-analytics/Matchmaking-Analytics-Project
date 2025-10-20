# Matchmaking Analytics Project

This project explores matchmaking mechanics and the influence of cross-platform play on match outcomes in Predecessor. It was developed in Python using Jupyter Notebook and ChatGPT.

I created this project out of curiosity about how the number of players from different platforms affects matchmaking results. Specifically, I wanted to understand how the difference in the number of PC and console players in a team impacts win rates.

## Dataset and Methodology

1. Collected all players from the leaderboard.
2. Extracted their last 10 ranked matches.
3. Created a table with all matches and players.
4. Assigned each player a platform label:
   - `0` for PC
   - `1` for Console
5. Grouped matches by the number of console players in each team (0 to 5) and calculated win rates.
6. Calculated the difference in the number of console players between teams for each match.
7. Grouped matches by this difference (from -5 to 5) and calculated win rates.

## Project Details

- **Duration:** 4 weeks  
- **Data collected:** February 2025

## Results

The analysis included a total of **23,067 matches**. The results show that the win rate tends to decrease for a team if it has more console players than the opposing team.

### 🎮 Win Rate by Number of Console Players

The table below shows how the average team win rate changes depending on the number of console players in each team.

| Console Players in Team | Win Rate |
|:------------------------:|:--------:|
| 0                        | 0.52     |
| 1                        | 0.51     |
| 2                        | 0.50     |
| 3                        | 0.49     |
| 4                        | 0.47     |
| 5                        | 0.48     |

### ⚖️ Win Rate by Console Player Difference

The table below shows how the average team win rate changes depending on the difference in the number of console players between two teams.  
A negative value means the team had *fewer* console players than the opponent, and a positive value means *more* console players.

| Console Player Difference | Win Rate |
|:--------------------------:|:--------:|
| -5                         | 0.62     |
| -4                         | 0.56     |
| -3                         | 0.56     |
| -2                         | 0.53     |
| -1                         | 0.51     |
| 0                          | 0.50     |
| 1                          | 0.49     |
| 2                          | 0.47     |
| 3                          | 0.44     |
| 4                          | 0.44     |
| 5                          | 0.38     |


Teams with fewer console players generally have higher win rates, indicating that cross-platform differences can impact competitive balance.


