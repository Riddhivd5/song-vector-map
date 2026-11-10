# song-vector-map
Explore a large collection of songs as an interactive, genre-organised map. Search for tracks, filter the map by genre, and open individual songs to see their details and listen on Spotify.
Features
- Search songs, artists, albums, and genres.
- Filter by genre families or individual genres.
- Adjust the minimum popularity threshold.
- Explore the map by dragging to pan and scrolling to zoom.
- Click a song to view its details and open it on Spotify.
- Press L to toggle song labels.
- Copy Spotify track links or create a private Spotify playlist from a selected song and related tracks.
- Light and dark appearance based on your system preference.
Try it online
When GitHub Pages is enabled, visit:
- https://riddhivd5.github.io/song-vector-map/

Run locally
This is a self-contained HTML application; no build step or package installation is required.
1. Download or clone this repository.
2. Open index.html in a browser for browsing and searching.
3. For Spotify sign-in, serve the page over HTTP rather than opening it as a file:// URL. For example, with Python installed, run this from the project folder:
   python -m http.server 8000
4. Open http://127.0.0.1:8000 in your browser.

Spotify setup
Spotify features require a Spotify Developer application.
1. Create an app in the Spotify Developer Dashboard.
2. Copy its Client ID.
3. Open the app's Spotify setup section in Song Vector Map and enter the Client ID when prompted.
4. Add the exact URL where the app is hosted to the Spotify app's Redirect URIs. For GitHub Pages, use:
   https://riddhivd5.github.io/song-vector-map/
   
Data
The song collection is embedded in the HTML file. The interface credits the Spotify Tracks Dataset (Kaggle) as its data source. Track availability and Spotify API behaviour may change over time.
Technologies
- HTML, CSS, and vanilla JavaScript
- HTML Canvas for the interactive map
- Spotify Web API for Spotify playlist functionality
Notes
- Browsing, searching, filtering, and copying track links do not require Spotify sign-in.
- Creating a playlist requires Spotify authorization and a working redirect URI.
- This project is an independent project and is not affiliated with or endorsed by Spotify.
