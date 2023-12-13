# What are their Top 10?

## Description
This app allows users to search for artists on Spotify and retrieve their top tracks, by leveraging the Spotify Web API to fetch data based on user input

## Pre-requisites
- Python 3.x
- 'requests' library
- 'python-dotenv' libary
- Spotify API Client ID and Secret

## Installation
Install the requires python libraries : `pip install requests python-dotenv`

### Spotify credentials
You first need to create a Spotify for Developers profile, and register an application in order to get your own `CLIENT_ID` and `CLIENT_SECRET`

Create a .env separate file to store your `CLIENT_ID` and `CLIENT_SECRET` like so : 

`CLIENT_ID = 'your_spotify_client_id'
CLIENT_SECRET = 'your_spotify_client_secret'`

** Important : Do not share these credentials with anyone, make sure you store them in a seprate `.env` file that only you have access to ** 

### Usage
To run the app, simply run `python main.py` (replace `main.py` by your script name) or `python3 main.py`

## Features
** Artist search ** : Search for any artist on spotify 
** Top tracks retrieval ** = Retrieves and displaus the top tracks of any given artist (assuming it exists on Spotify)
** Authorization token handling ** : Automatically handles the generation of auth token needed for API requests

## How it works
** Token generation ** : Retrieves an auth token using your Spotify API credentials
** Artist search ** : Searches for an artist based on the user's input
** Top tracks display ** : If the artist is found, the app lists their top tracks

## Limitations
- The search is limited to Spotify's database and API capabilities (limited amount of requests, etc...)
- The app only displays the top tracks available on the US market
