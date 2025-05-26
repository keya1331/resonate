<h1 align="center">
  <img src="https://github.com/mrankitgupta/Spotify-Data-Analysis-using-Python/blob/main/images/social-spotify.svg" alt="Spotify" width="55" height="40"/>
  resonate — music recommendation & data analysis
</h1>

---

## what it is  
a personalized recommendation system built on spotify data —  
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

## my part  
i designed the experience —  
from how users feed the system,  
to how the results are returned in rhythm and visuals.  
also worked on EDA, model tuning, and clustering logic.

---

## how it works  
```python
from spotipy.oauth2 import SpotifyClientCredentials
sp = spotipy.Spotify(auth_manager=SpotifyClientCredentials(
  client_id=os.environ["SPOTIFY_CLIENT_ID"],
  client_secret=os.environ["SPOTIFY_CLIENT_SECRET"]))
