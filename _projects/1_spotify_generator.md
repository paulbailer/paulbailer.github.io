---
layout: page
title: Spotify Playlist Generator
description: AI-powered playlist generation — describe what you want in plain language, get a real Spotify playlist.
importance: 1
category: fun
---

Started as a university assignment for the **Web Technologies** course at HTW Berlin (SS 2023). The original app let users enter numeric criteria — genre, BPM, danceability — to generate a playlist via Spotify's recommendations API, with results saved to an H2 database. The backend was a Spring Boot REST API.

The project was rebuilt from scratch after Spotify deprecated their `/v1/recommendations` endpoint in November 2024. The new version replaces the old seed parameters with plain-language input: describe a mood, a decade, an energy level — and Claude generates a curated list of tracks that fit. Each suggestion is verified against Spotify's catalog via the search API, so only real tracks make it in. The output is either a shareable list with Spotify links or, for connected accounts, a playlist created directly on the user's profile.

**[View on GitHub](https://github.com/paulbailer/playlist-generator)**