**Feel free to edit anything and add if you'd like.  I plan to touch it up at the end and make the repository public.**
# ISYE-6740 CDA Group Project
Casual Demonstrations of implementing supervised/unsupervised learning techniques on a dataset of the group's choice for Georgia Tech's Computational Data Analytics course.
## Project Description
Artists that sold over 1 Million Certified Albumns, according to [Recording Industry Association of America (*RIAA*)](https://www.riaa.com/), was collected on 10/01/2022.  An Artist's Spotify page, one of the most popular music streaming services, was accessed using [Spotify's API](https://developer.spotify.com/documentation/web-api/reference/#/) to gather information to see how popular artists relate to one another and what makes a song popular. Below are the quick definitions of a dataset's features.
#### Dataset
##### riaa_top_artists
Artist's from RIAA.com.
 * **Artist** - Name of the Artist.
 * **Certified Units** - Number of Units Sold (In Millions).
 * **Gold-Diamond** - Count of albumns in each classification category.

##### spotify_artists
* **artist_name** - Name of the artist.
* **artist_uri** - Spotify's URI.
* **popularity** - The popularity of the artist. The value will be between 0 and 100, with 100 being the most popular. The artist's popularity is calculated from the popularity of all the artist's tracks.
* **followers** - The total number of followers.
* **genres** - A list of the genres the artist is associated with. If not yet classified, the array is empty.

##### spotify_artists_related_artists
All Information is for Edge Artist except node_artist_uri and node_artist_name.

##### spotify_artists_top_tracks
* **artist_name**
* ...
* **danceability** - Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
* **energy** - Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
* **key** - The key the track is in. Integers map to pitches using standard Pitch Class notation. E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on. If no key was detected, the value is -1.
* **loudness** - The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db.
* **mode** - Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.
* **speechiness** - Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
* **acousticness** - A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
* **instrumentalness** - Predicts whether a track contains no vocals. "Ooh" and "aah" sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly "vocal". The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.
* **liveness** - Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
* **valence** - A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
* **tempo** - The overall estimated tempo of a track in beats per minute (BPM). In musical terminology, tempo is the speed or pace of a given piece and derives directly from the average beat duration.
* **time_signature** - An estimated time signature. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure). The time signature ranges from 3 to 7 indicating time signatures of "3/4", to "7/4".
