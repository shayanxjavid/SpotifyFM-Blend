# Spotify Blend Viewer

A web app that connects to Spotify, takes **two usernames**, and displays their **Blend playlist** with tracks, artists, and who added each song.

## Features

- Login with Spotify (OAuth)
- Enter two users → fetch Blend playlist
- Show:
  - Track name + artists
  - Added by which user
  - Playlist image
  - Play/preview buttons (if available)
- Simple EJS interface

## Setup

### Install

```bash
git clone https://github.com/yourname/spotifyfm-blend.git
cd spotify-blend
npm install
```

### Create `.env`

```
LASTFM_API_KEY =
SPOTIFY_CLIENT_ID=
SPOTIFY_CLIENT_SECRET=
SPOTIFY_REDIRECT_URI=http://localhost:3000/callback
SESSION_SECRET=anything
PORT=3000
```

Add to `.gitignore`:

```
.env
```

### Run

```bash
npm start
```

Open in browser:

```
http://localhost:3000
```

## How It Works

```
Login → Spotify OAuth → Fetch Blend Playlist → Render in playlist.ejs
```

## Tech Stack

- Node.js + Express
- Spotify Web API
- EJS templates
- OAuth 2.0

## License

MIT — use freely.
