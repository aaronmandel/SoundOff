# SoundOff

SoundOff is a Discord bot that integrates with Spotify to show your top songs, artists, genres, and currently playing tracks.

## Features
- Login with Spotify
- Show what’s currently playing
- Display your top tracks & artists
- Retrieve recently played songs
- Discover your top genre of all time or for the month

## Installation

### 1 Clone the repository
```bash
git clone https://github.com/aaronmandel/SoundOff.git
cd SoundOff
```

### 2 Install dependencies
```bash
pip install -r requirements.txt
```

### 3 Set up environment variables
- Create a `.env` file (or rename `.env.example`).
- Add the following variables:

```
DISCORD_TOKEN=your_discord_bot_token
DISCORD_CHANNEL_ID=your_channel_id
SPOTIPY_CLIENT_ID=your_spotify_client_id
SPOTIPY_CLIENT_SECRET=your_spotify_client_secret
SPOTIPY_REDIRECT_URI=http://localhost:8888/callback
SPOTIPY_SCOPE=user-read-playback-state user-top-read user-read-recently-played
```

### 4 Run the bot
```bash
python bot.py
```

## Commands
| Command         | Description |
|----------------|-------------|
| `!login`       | Log in to Spotify |
| `!callback <code>` | Complete Spotify authentication |
| `!list`        | Check if you're logged in |
| `!now_playing` | Show currently playing track |
| `!top_track`   | Show your top track of all time |
| `!top_artist`  | Show your top artist of all time |
| `!top_10`      | Show your top 10 tracks |
| `!recent`      | Show your most recently played track |
| `!top_genre`   | Show your all-time top genre |
| `!top_genre_month` | Show your top genre for the month |

## Dependencies
- Python 3.8+
- [discord.py](https://pypi.org/project/discord.py/)
- [spotipy](https://pypi.org/project/spotipy/)
- [python-dotenv](https://pypi.org/project/python-dotenv/)


