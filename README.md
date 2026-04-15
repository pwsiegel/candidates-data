# Opening Distribution in the FIDE Candidates Tournament

Analysis of opening choices across recent FIDE Candidates Tournaments, using game data from [Lichess broadcasts](https://lichess.org/broadcast).

Games are grouped into "opening families" by taking the name before the first colon in the Lichess opening annotation (e.g. "Ruy Lopez: Berlin Defense, Anti-Berlin Variation" becomes "Ruy Lopez").

## Open Section (2022, 2024, 2026)

168 games across three tournaments. Each tournament is an 8-player double round-robin (14 rounds, 4 games per round).

![Open section openings](images/open.png)

The Ruy Lopez dominated in 2022 and 2024 but disappeared entirely in 2026, replaced by a surge in Queen's Gambit Declined. The Sicilian has been on a steady decline. Petrov's Defense remains a consistent choice across all three years.

| Opening Family | 2022 | 2024 | 2026 | Total |
| :--- | :---: | :---: | :---: | :---: |
| Ruy Lopez | 13 | 14 | 0 | 27 |
| Queen's Gambit Declined | 1 | 5 | 20 | 26 |
| Sicilian Defense | 11 | 9 | 4 | 24 |
| Petrov's Defense | 6 | 7 | 6 | 19 |
| English Opening | 4 | 0 | 8 | 12 |
| Italian Game | 5 | 5 | 1 | 11 |
| Catalan Opening | 5 | 1 | 3 | 9 |
| Nimzo-Indian Defense | 3 | 2 | 2 | 7 |
| Four Knights Game | 3 | 1 | 1 | 5 |
| French Defense | 0 | 3 | 2 | 5 |

## Women's Section (2024, 2026)

112 games across two tournaments. The 2022 Women's Candidates used a knockout format rather than a round-robin, so it is not included.

![Women's section openings](images/women.png)

| Opening Family | 2024 | 2026 | Total |
| :--- | :---: | :---: | :---: |
| Sicilian Defense | 6 | 13 | 19 |
| Italian Game | 6 | 11 | 17 |
| Ruy Lopez | 10 | 5 | 15 |
| Queen's Gambit Declined | 7 | 5 | 12 |
| Petrov's Defense | 2 | 2 | 4 |
| Catalan Opening | 4 | 0 | 4 |
| Scotch Game | 1 | 3 | 4 |
| French Defense | 2 | 1 | 3 |
| Caro-Kann Defense | 1 | 2 | 3 |
| Grunfeld Defense | 2 | 1 | 3 |

## Combined (Open + Women, 2024 & 2026)

224 games. Only 2024 and 2026 are included since those are the years where both sections used the same round-robin format.

![Combined openings](images/combined.png)

| Opening Family | 2024 | 2026 | Total |
| :--- | :---: | :---: | :---: |
| Queen's Gambit Declined | 12 | 25 | 37 |
| Sicilian Defense | 15 | 17 | 32 |
| Ruy Lopez | 24 | 5 | 29 |
| Italian Game | 11 | 12 | 23 |
| Petrov's Defense | 9 | 8 | 17 |
| English Opening | 0 | 10 | 10 |
| Catalan Opening | 5 | 3 | 8 |
| French Defense | 5 | 3 | 8 |
| Nimzo-Indian Defense | 3 | 3 | 6 |
| Tarrasch Defense | 3 | 1 | 4 |

## Data Source

All game data is fetched live from the [Lichess Broadcast API](https://lichess.org/api#tag/Broadcasts). The Jupyter notebook `candidates_openings.ipynb` contains the full data pipeline and interactive Plotly charts.

## Running

```
uv run jupyter lab
```
