# Playlistour

Playlistour is an AI-assisted concert discovery app that helps users find live music events based on their Spotify taste profile.

## Why I built it

I built Playlistour to explore how AI can make music discovery more contextual and action-oriented. Instead of only recommending songs or artists, the product connects listening history and taste signals to real-world concerts a user can actually attend.

## What it does

- Connects to a user's Spotify profile
- Uses music taste signals to identify relevant artists and genres
- Searches for upcoming concerts using Ticketmaster and SeatGeek APIs
- Helps users discover live events that match their music preferences
- Experiments with AI-assisted ranking and explanation of why an event may be relevant

## Product focus

The core product question was:

> How can we turn passive music taste into timely, relevant, real-world concert discovery?

Key product areas included:

- User onboarding and Spotify OAuth flow
- Event discovery and ranking
- API integrations across Spotify, Ticketmaster, and SeatGeek
- Relevance and explanation quality
- Trust, privacy, and handling missing or noisy data

## Why this matters

Music discovery often stops at playlists. Playlistour explores a more action-oriented experience: helping users move from "I like this music" to "there is a show near me that I might actually want to attend."

## Tech / implementation notes

The private working repo includes the actual implementation. This public repo is a sanitized portfolio version without secrets, API keys, tokens, user data, or private development notes.

Core components:

- Spotify OAuth integration
- Concert/event search via Ticketmaster and SeatGeek
- AI-assisted product logic for ranking and explanations
- Lightweight frontend for discovery and exploration

## What I learned

This project helped me think more deeply about:

- AI-assisted consumer discovery
- Cross-API product experiences
- Ranking and explanation UX
- User trust in recommendations
- Fast prototyping with AI coding tools

- ## Screenshots

![Playlistour home](screenshots/playlistour-home.png)

![Playlistour results](screenshots/playlistour-results.png)
