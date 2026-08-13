# Playlistour

Find concerts from the music you already listen to.

Connect YouTube Music or Spotify, pick a city and dates, and see upcoming shows that match — with a score and a short explanation of why the night is relevant.

**Web:** [playlistour.com](https://playlistour.com)  
**iOS:** [App Store](https://apps.apple.com/us/app/playlistour/id6759816667)  
**Portfolio:** [kirillpm.com](https://kirillpm.com)

This public repository is a product case study. The production source stays private.

I designed and shipped Playlistour as a consumer product, using Lovable as an AI development collaborator.

---

## The problem

Music apps are good at the next song. They are much worse at the next night out.

Taste already exists in playlists and liked tracks. Concert listings already exist on ticketing sites. The gap is joining those two without making the user search artist by artist, and without pretending an LLM “knows” which show to attend.

---

## What it does

1. **Connect a library** — YouTube Music (primary) or Spotify.
2. **Pick place and time** — a city and a date range.
3. **Choose what to search from** — playlists / liked music, not a blank genre box.
4. **See matches** — list + calendar, match score, and “why this concert.”
5. **Act** — open tickets, save to calendar, optionally subscribe to alerts for artists you care about.

---

## Product decisions

**Start from listening, not from a city homepage.** The interesting object is *your* artists, not a generic “events near you” feed.

**Score the match in product logic.** Relevance is deterministic from listening signals (how central the artist is, playlist presence, penalties for weak matches such as tributes). The model writes the explanation; it does not get to invent the ranking.

**Use several event sources, then tell the truth about missing data.** Search draws on Ticketmaster, Bandsintown, and SeatGeek. Listings are incomplete in the real world — sold-out state, price, and lineups are often wrong or absent. The UI should not fabricate them.

**YouTube Music is the reliable on-ramp.** Spotify is supported, with access currently limited by Spotify’s development-mode cap and a waitlist for everyone else. The public product should not pretend that path is fully open.

**Alerts are the retention loop.** Discovery is a one-shot. “Email me when this artist announces a date in my city” is the reason to come back.

---

## What this is not

Not a new ticketing company. Not a claim that AI trained a music model. Not an open Spotify integration for every user today.

It is a consumer discovery product: turn a library you already have into a show you might actually attend.

---

## How it was built

I designed the wizard, the matching rules, and the honesty constraints around third-party event data, then built and shipped the web and iOS product with Lovable as an AI coding collaborator.

---

## Screenshots

To add after a sanitization pass (no real emails, account names, or personal playlists):

1. Connect music source.
2. City / dates.
3. Results — list or calendar with match score.
4. “Why this concert” explanation.

Existing App Store captures in this repo should be reviewed before they are linked; do not ship broken image paths.

---

## Links

- Web: [playlistour.com](https://playlistour.com)
- App Store: [Playlistour](https://apps.apple.com/us/app/playlistour/id6759816667)
- Portfolio: [kirillpm.com](https://kirillpm.com)
