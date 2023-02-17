# DataScienceProjects

Created a CSV File that I webscraped off of myanimelist.net of the top 10,000 animes. Took some understanding of time.sleep() in python to make sure the server doesn't block access for too many requests (02/16/2023).

How are MyAnimeList scores calculated?
All scores given in the database are calculated as a weighted score.

Weighted Score = (v / (v + m)) * S + (m / (v + m)) * C
S = Average score for the anime/manga
v = Number users giving a score for the anime/manga †
m = Minimum number of scored users required to get a calculated score
C = The mean score across the entire Anime/Manga database

† Note that v does not correspond to the "number of scored users" as seen on the database page. Scores from users who have not viewed 1/5 of the series upon its completion are not included. Scores given from illegitimate accounts created to sway votes are also not included in the scoring algorithm.

Not Yet Aired entries have no score and will display N/A. Entries that do not meet the minimum number of scored users will also not display a calculated score.

Top Anime/Manga Rankings
The "Top Upcoming" and "Most Popular" rankings are ordered by the number of users who have added the entry to their list. All other Top Anime and Top Manga rankings are ordered by weighted score, as calculated above. Please note that while R18+ entries calculate a weighted score, they are excluded from the rankings.

![59510_8b8e76a4b07ef6ed6bd3340ae40f14c9040246d3_myanimelist_m](https://user-images.githubusercontent.com/28698665/219535929-f3beb799-d250-4367-8661-6d858e69ab38.png)
