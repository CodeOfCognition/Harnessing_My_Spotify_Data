# About This Project

This project started because my Spotify Wrapped was all full of music I listened to when I studied. The goal of this project was to use my Spotify data to 
create my own Spotify Wrapped playlist (among others) and gather some insights about my listening patterns.

### Data collection

After requesting my personal data from Spotify (see `data/inputs`), I used my streaming history to create a **set** of all songs I listed to this year. I loaded this into a dataframe, ranked songs by number of meaningful listens (> 20 seconds), removed songs from my study playlists, gathered audio features (valence, danceability, tempo, etc.) and song URIs via Spotify API. I then created a streaming history dataframe containing audio features too. Data is stored in csv form in `data/outputs`.

### Playlist Creation

Using the Spotify API, I was able to create multiple playlists for myself using this dataset. I created algorithms that used a combination of audio feature specifications and number of streams to create playlists. I created a top 100 and a top 250 songs of 2021 playlist. I also created both a "hype dance" playlist and a "low key grooves" playlist. They were absolutely awesome :D

### Tableau Dashboard [(click to view)](https://public.tableau.com/app/profile/robbie6107/viz/HarnessingMySpotifyData/Dashboard1)

My tableau dashboard serves two purposes. 

Firstly, it draws insights about my listening habits. It shows my streaming patterns throughout the day. It shows how I listen to more danceable music as the day progresses. It shows that I like to listen to highly instrumental music in the morning (classical music with breakfast during COVID), and around dinnertime (70's rock while I cook). This shows that my data contains valuable user insights that can be used to classify user listening patterns and motivates a more extensive analysis (see Future plans below).

Secondly, the dashboard contains my top artists and songs for 2021. This was very meaningful to me because my Spotify Wrapped only showed me my top 5 songs and artists, most of which were lo-fi study music tracks/artists. This gave me a chance to understand what my year of music was really like.


### Future Plans

Now that I gathered an annotated dataset of my listeneing patterns, I want to create reccommendation algorithms. I have several ideas for this. 

I want to apply my knowledge of computational linguistics to create abstract representations of songs. One way I can do this is by treating songs as words and music listening sessions as sentences. This allows me to use modified n-gram models to characterize songs, allowing me to create song reccommendations. Additionally, I am taking a course called "Natural Language with Deep Learning" right now (Jan 2022) at McGill. I hope to apply the deep learning concepts I learn in this course to create "next song" reccommendations, as well as playlist creation.



