# Steam Statistics from SteamSpy API

Tableau visualisation: https://public.tableau.com/app/profile/ziming.lin/viz/Steam_16616915480210/Revenue-Price

![screenshot](https://raw.githubusercontent.com/Ziming-Lin/steam-stats-steamspy-api/main/steam-viz.gif)


## Disclaimer

The data is highly approximated. At the point of publishing this visualization, Steam's own API does not show details such as game ownership and playtime. Since Steam added account privacy features in 2018 rendering scraping impracticable, pulling data from Steam Spy's API for such information is the only option but it is approximated data based on Steam Spy's algorithm (see https://en.wikipedia.org/wiki/Steam_Spy).

The game prices in the data refer to current undiscounted prices and do not account for any price reductions since the games were released. Hence certain features such as game revenue can be highly inaccurate (e.g. Counter-Strike: Global Offensive, now $0).


## Usage

Tableau's accessible k-means cluster analysis feature makes it easy to group marks into clusters for analysis purposes.

An example of this can be observed in the price vs release date chart which shows that there is a general trend for game prices to increase over the years. However, cluster analysis suggests that prices of cheaper games produced by indie developers are trending lower, which in turn suggests that there is an increasing number of free and almost-free indie games showing up on Steam.

Another useful observation via cluster analysis can be seen in the ratings vs price chart where 3 clusters form:
- Low prices and low ratings
- Low prices and high ratings
- High prices

It is not unreasonable to infer that games priced higher than ~$30 have harsher critics since ratings fall as game prices increase. Whereas while paying under $30, gamers are able to appreciate the better quality of games they get as game prices increase.
