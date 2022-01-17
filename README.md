The purpose of this project was to harness my Spotify data (see `data/inputs`). I did so in the following ways:

#### Data collection

After requesting my personal data from Spotify (see `data/inputs`), I used my streaming history to create a **set** of all songs I listed to this year. I loaded this into a 
dataframe, ranked songs by number of meaningful listens (> 20 seconds), removed songs from my study playlists, gathered audio features (valence, danceability, tempo, etc.) 
and song URIs via Spotify API. I then created a streaming history dataframe containing audio features too.

#### Creating Playlists

Firstly, I used the data to create playlists. This 

#### Tableau Dashboard [view here](https://public.tableau.com/app/profile/robbie6107/viz/HarnessingMySpotifyData/Dashboard1)
