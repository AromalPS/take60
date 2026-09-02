# Take 60

A single-page practice tool for talking off the cuff: hit spin, get a random topic, and talk about it for a set amount of time without stopping. Built for creators who want to drill short-form video content (Reels/Shorts-style takes) across business niches.

## How it works

1. **Spin** — draws a random topic from the selected niches (a topic never repeats until the log is reset or you free it up).
2. **Start take** — a countdown begins; the topic card shrinks and the timer ring/clock take over as the main focus. Once running there's no pause — it's meant to be a one-shot take. A siren sounds when time's up.
3. **Re-spin** if the topic doesn't land, or **Reset timer** to restart the same topic without spinning again.
4. **Research 10m** (length configurable) — a separate break timer for when you need a minute to think before talking, independent of the take timer.

## Topics

246 topics across 6 niches — pick which ones are in play from the Niches list in Settings:

- Entrepreneurship
- Marketing
- Branding
- Sales
- Finance
- Leadership

Topics are short, specific business/marketing concepts (e.g. "CAC", "Cap table", "Mental availability") rather than pre-written opinions — the idea is you build the take live.

## Settings

Gear icon in the header opens:
- **Take length** — slider, 15s–180s
- **Research length** — slider, 5–30 min
- **Niches** — checkbox list of which niches to draw topics from
- **Sound** — on/off toggle for the spin ticks, landing chime, and end-of-take alarm

## Log

The "Log" panel shows every topic used this session, in order, with its niche. Remove individual entries to put a topic back in the pool, or reset the whole log to start over with all 246 topics available again.

## Tech notes

- Single HTML file (`take60.html`) — no build step, no dependencies beyond a Google Fonts stylesheet. Just open it in a browser.
- All sound (ticks, chime, siren) is synthesized with the Web Audio API — no audio files.
- State (used topics, current topic, take/research length, niche selection, mute) persists to `localStorage`, so it survives a page reload.
