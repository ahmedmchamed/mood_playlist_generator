# Final group project - Spicify mood playlist generator

## Web App
![login_screenshot](/public/login_screenshot.png?raw=true "login Screenshot")

The login page

![homepage_screenshot](/public/homepage_screenshot.png?raw=true "homepage Screenshot")

The homepage after generating a playlist

---
## Brief

This is our final group project. We built this app to generate random playlists, using Spotify's API via an OAuth 2.0 authorisation flow, based on a mood selector that can be manually set by a user or detected automatically through the user's facial expression.

The facial expression API is from Microsoft Azure, which returns data ranking a user's expression based on properties such as happiness, neutral, sadness, surprise, etc. The user can manually set the rotational slider around the camera view, or click on the shutter icon to take a selfie, after which an API call is made and the results fetched. 

When clicking on the 'Generate Playlist' button, a list of songs from the user's existing playlists are returned that match as closely as possible the mood result that the user would like to listen to. Using the Spotify Connect SDK, the songs can be played as normal with the usual playback options available, and a progress bar reflecting how far into the song the user is.

The frontend framework for the app is React, using an express server to communicate with the Spotify and Azure APIs.

## Starting the app

`cd` into the `frontend` directory and run: `npm install` followed by `npm start`

`cd` into the `backend_node` directory and run: `npm install` followed by `npm run server:dev`

