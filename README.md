##resonate — music recommendation & data analysis
  
---

## what it is  
a personalized recommendation system built on spotify data 
exploring patterns in sound, popularity, and genre.  
songs suggested by similarity, not just surface.  
music, made measurable.

---

## what it does  
- pulls audio features using Spotify’s Web API  
- builds feature vectors for user-input songs  
- recommends songs via cosine similarity  
- analyzes popularity, genres, mood clusters, and composition shifts  
- visualizes listening trends from 1992 to now

---

## visual insights 

### Top 10 Most Popular Songs  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/cd81f3f5-facb-4d0e-b1da-b60789442352" alt="Top 10 Most Popular Songs" width="100%"/>

### Correlation Heatmap  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/667f1f6e-dc5b-4206-ac4e-ec2cdf705e50" alt="Correlation Heatmap" width="100%"/>

### Loudness vs Energy  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/f4e596f7-f9fc-4fc4-b237-ae227c5027e6" alt="Loudness vs Energy" width="100%"/>

### Popularity vs Acousticness  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/e9d61bb0-b002-4e61-81bf-33096d02fb9c" alt="Popularity vs Acousticness" width="100%"/>

### Songs Released Since 1992  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/39c4e1df-26fb-48a4-b6c3-339b2f6aa6e0" alt="Songs Released Since 1992" width="100%"/>

### Change in Song Duration Over Time  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/e92c1eb1-9368-464f-b5d2-9b877d32e369" alt="Change in Duration Over Time" width="100%"/>

### Duration by Genre  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/0fae7e69-6577-4696-ab18-96ffbf1a4777" alt="Duration by Genre" width="100%"/>

### Top 5 Genres by Popularity  
<img src="https://github.com/Gokul-Raja84/Spotify-Data-Analysis/assets/106546785/7ec5edd7-a45e-425a-9795-d5d5352947e1" alt="Top 5 Genres by Popularity" width="100%"/>


## how it works  
```python
from spotipy.oauth2 import SpotifyClientCredentials
sp = spotipy.Spotify(auth_manager=SpotifyClientCredentials(
  client_id=os.environ["SPOTIFY_CLIENT_ID"],
  client_secret=os.environ["SPOTIFY_CLIENT_SECRET"]))
