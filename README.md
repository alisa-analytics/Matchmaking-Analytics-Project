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

## Results

The analysis included a total of **23,067 matches**. The results show that the win rate tends to decrease for a team if it has more console players than the opposing team.
