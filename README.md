# AI Feelings Log

A daily, collaborative mood tracker for how people feel about AI. Each day since January 1, 2023 is a glowing orb — yellow for good, blue for bad, red for ugly — clustered by how many people logged that day. Visitors can log their own mood with a required reason; past years collapse by default to keep things fast.

Click "make into art" on any year to watch its orbs animate into pixel formations — a heart, a star, a sun — grouped by mood so each shape forms in clean color bands.

## How it's filled

- **Live logging**: anyone can submit a mood + reason for today. First submission wins if two people log at once. Basic profanity filtering is applied.
- **Historical days**: backfilled with real AI-news headlines (via GDELT's free archive) reframed in a personal voice, falling back to a curated pool of lines when no headline is available.
- **Future days**: filled automatically at midnight UTC by a scheduled Cloud Function, using the same headline-then-fallback approach.

## Stack

Single-page HTML app backed by Firebase Realtime Database (free tier). No paid APIs.
