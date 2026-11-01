# Changelog

Everything that changed in Streample, newest first. Each published version is also on the
[releases page](https://github.com/yergerb/streample-releases/releases), where Streample's in-app
updater gets it from.

## 0.6.0 (2026-11-01)

### Endless browsing
- **Endless categories** on Home, Movies and Series: below the usual rows, new categories keep coming as you scroll, from three sources:
  - TMDB combinations: genre × decade ("'90s Comedies"), country × genre ("Korean Crime Series", "Hong Kong Thrillers"), studios (A24, Pixar, Studio Ghibli…), networks (HBO, FX, Apple TV+…), "Critically Acclaimed …", "Hidden Gem …", "… Under 90 Minutes".
  - Trakt public lists people made and voted on ("Rotten Tomatoes: Best Heist Movies of All Time", "Attenborough Documentaries").
  - Rows from what you watch: "More Like [title]", "Starring [actor]", "Directed by [director]".
- The feed **learns what you like**: kinds of categories you open titles from show up more often; ones you scroll past show up less. Your favourite genres get a boost.
- **At least 10 titles per row** everywhere (thin rows are left out), and no category appears twice in one visit. A title can appear in several categories.
- **Rows loop**: after the last title comes the first again, so sideways scrolling never ends (Top 10 doesn't loop).
- The curated theme rows (Heists & Cons, Time Travel…) are now part of the endless mix on Movies and Series.

### Home and Movies
- Home order: Continue Watching, New Episodes, **Top 10 Today**, My List, Top Picks, Trending Movies, Trending Series, **Just Hit Digital**, Coming Soon, Because You Watched…, then endless categories.
- **Just Hit Digital**: movies released digitally in the last two months (Home, and near the top of Movies).
- A small **✓ on posters** you've watched (bottom-right corner).

### Navigation
- **Three very fast Left presses open the menu** from anywhere; holding Left only scrolls (it never opens the menu, even at the start of a row).
- **Back once opens the menu**, anywhere outside the player; **Back twice quickly** goes back for real (to Home, out of the app from Home, or to the previous page from a title).
- The menu's "Back to Movies / Series …" item goes straight back.

### Search
- **Category search**: typing "heist", "zombie", "80s", "korean", "a24"… also shows matching category rows.

### Fixes
- Fixed playback going black and jumping back a few seconds about 20 seconds into an episode: the video player now belongs to the episode, so nothing happening on screen can restart it.

## 0.5.3 (2026-10-31)
- Player: press Down twice quickly to hide the controls.
- **Skip Intro is one press**: when an intro starts, the controls tuck away and the Skip button is already selected, so OK skips. If the controls are up, their Skip button has focus first.

## 0.5.2 (2026-10-31)
- The **Update available** card is a proper dialog: the remote stays on it until you choose Update now or Later (Home behind it no longer scrolls), and its notes show as plain text.
- **Skip Intro**: press Right to select the button (it turns white), then OK to skip.

## 0.5.1 (2026-10-31)

The big settings, browsing and player update (it includes everything from the unreleased 0.4.1 and 0.5.0 test builds).

### Settings
- Settings split into five categories: **Playback**, **Accounts**, **Library**, **About** and **Advanced**. Everyday choices stay short; technical ones live under Advanced.
- **Accounts** shows whether Real-Debrid and Trakt are connected, and holds every key the app uses (Real-Debrid token, Trakt Client ID, TMDB, OMDb), with where to get each one.
- **Hide sources** (Playback): tick Cam / telesync (ticked by default), SD, 720p, 1080p or 4K, and those sources never show up or get picked.
- **Surprise me card** can be switched off (Playback).
- Language and subtitle choices wrap onto a few lines instead of scrolling sideways.
- Advanced → **Player**: video player, match frame rate, surround passthrough, skip intros automatically, player stats, subtitle color / background / position, trailer app.
- Advanced → **Browsing**: spoiler-free episodes.
- Advanced → **Sources**: torrent streaming, largest torrent, torrent data used this month, add-ons.
- Advanced → **Tests & diagnostics**:
  - **Connection check**: internet, Real-Debrid, Trakt, TMDB and OMDb keys, every add-on, plus a speed test that suggests a quality.
  - **Picture test**: HDR10, HDR10+, Dolby Vision and HLG support, and which video formats decode in hardware. AV1 sources move to the bottom of the list on devices that can't decode AV1 in hardware.
  - **Surround sound test**: which formats your TV, soundbar or receiver accepts untouched, and a speaker-by-speaker voice test for 5.1 and 7.1.
  - **Lip-sync**: line up a flash and a beep; the correction applies when VLC plays.
  - Crash reports.
- Library → **Your stats**: hours watched this month, this year and in total, top genres, most-watched titles, biggest day.

### Home and browsing
- **Top 10 Today** row with big rank numbers on Home (movies and series), on Movies (movies only) and on Series (series only).
- On Home, titles in Top 10 don't appear again in Trending Movies / Trending Series.
- **Coming Soon** row: upcoming episodes of shows you watch or have in My List, with air dates.
- **Surprise me** card at the start of Top Picks opens a random pick.
- Movies and Series: the core rows (new releases, highly rated, hidden gems, main genres) stay in order; the themed rows below them (Westerns, Heists, Time Travel and so on) are reshuffled each time you open the tab.
- Continue Watching cards say how much is left ("S2:E5 · 23 min left").
- Spotlight shows three lines of synopsis, with less empty space above the rows.
- The background art fills the whole screen width (no black band on the left), and rows start close to the screen edge.
- Title and actor pages: pressing Left at the edge brings up the menu, with **Back to Movies / Series / …** at the top.
- Coming back from a title always puts focus on the card you opened.

### Title pages
- Age rating badge (PG-13, TV-MA…).
- "Ends at 10:42 PM" for movies.
- A progress bar under each season you've started; the episode row opens on your next episode.

### Player
- A **Skip Intro / Skip Recap** button bottom right while the intro plays: a rounded, see-through pill (OK skips it) that fills to show how much intro is left. Works for episodes IntroDB knows (most popular shows) or files with intro chapters.
- Your audio and subtitle choice for a show is remembered for its other episodes.
- **Sleep timer** in Options: end of this episode, 30 minutes, 1 hour or 1½ hours.
- **Are you still watching?** after three episodes in a row with no button pressed.
- **Player stats** overlay (Options or Advanced): resolution, codec, HDR type, frame rate, bitrate, buffer, dropped frames, sound output, torrent peers.
- Options shows what the sound is sent as (e.g. "Dolby Atmos → sound system (passthrough ✓)").
- Optional automatic Skip Intro / Skip Recap.
- Subtitle color, background box and position (Advanced).

### Search and Android TV
- Redesigned Search: a wide search bar with the mic beside it, the focused title's artwork in the background, and results as **People**, **Movies** and **Series** rows.
- Before you type: your recent searches, and a **Trending now** row you can move into and open.
- A **Streample · Top Picks** row on the Android TV home screen.
- The TV's own search (and Google Assistant, where the launcher supports it) can find Streample titles.

### Fixes
- Settings: the remote can move into a category's settings and scroll through them; Left returns to the category you're in.
- Fixed crashes when moving around Search results (e.g. after searching "lord of the rings" or "star wars") and between the menu and Settings: updated the UI toolkit (Compose 1.8), whose older focus handling caused them.
- The Top 10 trending row retries once if Trakt doesn't answer.

## 0.4.0 (2026-10-31)
- **Match frame rate**: the TV switches to the film's own refresh rate (e.g. 24 Hz) while it plays.
- **Surround passthrough**: Dolby Digital, Atmos and DTS go straight to your soundbar or receiver (VLC too).
- **Play Next** on the Android TV home screen mirrors Continue Watching.
- **Resume or start over** when you press Play on something half-watched.
- Title pages: quality badges (4K, Dolby Vision, Atmos, ⚡ Instant), Rotten Tomatoes and Metacritic scores (with a free OMDb key), and film collections in order.
- **New Episodes** row on Home.
- Hold OK on a Continue Watching card to remove it.
- My List syncs both ways with your Trakt watchlist.
- Thumbs up / down at the end of a movie or series, sent to Trakt; thumbs-down titles stop appearing in Top Picks.
- **Skip Intro / Skip Recap** for episodes (IntroDB community times, or the file's chapters); credits detection uses them too.
- Pause screen with title, synopsis and end time.
- Torrent size limit and a free-space check before a torrent starts.
- Crash reports saved on the device.
- New app icon and banner.

## 0.3.1 (2026-10-31)
- Setup → Languages uses the full screen, with every language on wrapping lines.
- Settings → Run setup again stays on after restarting the app.

## 0.3.0 (2026-10-31)
- **Scrubbable progress bar**: press up to select it, hold left/right; steps speed up from 10 s to 5 min.
- **Smart source fallback**: if a source fails, keeps buffering for 25 s, or a torrent can't connect, Streample switches to the next-best source at the same spot (up to 3 tries).

## 0.2.0 (2026-10-31): first public build
- First-launch setup for Real-Debrid (optional), Torrentio, Trakt, TMDB and languages, with a phone page (QR code) to paste keys.
- Backup and restore of settings, keys, history and My List.
- Keys are entered on the device; release builds contain none.
- In-app updates from GitHub releases.
- Built-in torrent streaming when you don't use Real-Debrid.
- Voice search (mic button and the remote's search key) and people search.
- Cast & crew with character names and actor pages.
- Mark as watched (synced to Trakt), Next Episode button at the credits, next-episode autoplay.
- OpenSubtitles, Trakt scrobbling, player options (speed, zoom, subtitle size, sync).
- Curated Movies and Series categories, TMDB theme rows, endless rows.
- Instant Home on launch; Top Picks reshuffled each launch; Home order Continue Watching, My List, Top Picks, Trending, Because You Watched.

## Before 0.2.0 (personal builds)
- Netflix-style Home, Movies, Series and My List built on Cinemeta and Stremio add-ons.
- Source ranking and one-press Play; ExoPlayer with VLC fallback.
- Trakt history import and recommendations.
- Language preferences that reorder sources without hiding any.
