# transfer-analysis

This is a project is a narrative story that seeks to asses the dominance of the English Premier League, and to understand the extent or truth of that dominance. The data in this project is almost entirely sourced from transfermarkt.us, and GitHub user ewenme, whose wonderful project allows me to scrape it. The final project, as a story is here: https://ahanpenkar.github.io/transfer-analysis/

## Scraping

Thankfully, much of the scraping has already happened. For transperancy's sake and clearer expertise, I would refer you to the source project. I will update the scraper to account for the winter transfer window:

Here is what i did:
 
tktktktktktkt

## Understanding the Data - ripped from ewenme

Transfers can be found in the `data/` directory, in .csv format. There's a file for each of these leagues:

- English Premier League (`premier-league.csv`)
- English Championship (`championship.csv`)
- French Ligue 1 (`ligue-1.csv`)
- German 1.Bundesliga (`1-bundesliga.csv`)
- Italian Serie A (`serie-a.csv`)
- Spanish La Liga (`primera-division.csv`)
- Portugese Liga NOS (`liga-nos.csv`)
- Dutch Eredivisie (`eredivisie.csv`)
- Russian Premier Liga (`premier-liga.csv`)

Common variables:

| Header | Description | Data Type |
| --- | --- | --- |
| `club_name` | name of club | text |
| `player_name` | name of player | text |
| `position` | position of player | text |
| `club_involved_name` | name of secondary club involved in transfer | text |
| `fee` | raw transfer fee information | text |
| `transfer_movement` | transfer into club or out of club? | text |
| `transfer_period` | transfer window (summer or winter) | text |
| `fee_cleaned` | numeric transformation of `fee`, in EUR millions| numeric |
| `league_name` | name of league `club_name` belongs to | text |
| `year` | year of transfer | text |
| `season` | season of transfer (interpolated from `year`) | text |

## Merging for Country and League of outgoing Club

There was no data available for the outgoing clubs, so I merged the dataset with the information from FBRef.

## Analysis and interpretation

My analysis of this data is available in the `analysis/` directory. The questions and methods I have chosen, as well as graphs (if any) are detailed in the cells. I will put forward the important qustions here:

An important note: I am not a finanical expert nor am i well versed in buisness. I am simply looking at money in terms of transfers in an out for the sake of simplicity in this story. Reporting on that was outside the scope of this story. 

### Who 
