# song_recommender_system 


The purpose of this small academic project is mainly to practice web scraping, working with API´s, and coding logic. The objective is to create a song recommender system that will take the user's imput, a song name, will first check if the song is within the list of Billboard Hot 100 and, if it is, it will recommend another song from the same list. If the imput song is not within the Billboard Hot 100 list, it will then send the song to Spotify´s API to retrieve the audio features of it, it will compare this audio features with the audio features of a collection of songs previously obtained from Spotipy, and also previously clustered accordingly to their audio features, and it will determine in which cluster the imput song would fall, to finally recommend the song with the closest audio features from that same cluster. 

In the repository we can find two folders, one called scripts, and another one called data, as well as the song_recommender_system itself. 

Within the scripts folder we can find:

  - billboard_data_web_scraping file. Python script in which web scraping has been performed to collect the Billboard Hot 100 list of songs and artists of the moment. 
  - spotify_data_collection_and_clustering file. Python script in which the code can be seen to connect to Spotify´s API in order obtain a collection of songs, artists, and the audio features of the songs. In this same file, the clustering of songs in accordance to their audio features using KMeans algorithm can also be found.

Within the data folder we can find:

  - billboard_data file. CSV file in which the list of songs and artists from Billboard Hot 100 has been saved.
  - spotify_data file. CSV file in which the collection of songs and artists from Spotify, with the audio features, has been saved.

Finally we have the song_recommender_system itself, a Python function that follows the logic mentioned at the beginning and that can be seen visually just below.

![song_recommender_flow](https://user-images.githubusercontent.com/111697941/226649052-5515a17a-868a-4703-bf65-dfed5751c0e4.jpg)
