# Stress Meter

A calm companion that reads your body and work rhythm, and nudges you to rest well before burnout. It never tells you that you are stressed. An avatar shows how your body is doing, and one short suggestion tells you what to do about it.

This repo is an interactive prototype of the mobile app (V2).

## Try it

Open `index.html` in a browser, or publish it with GitHub Pages (below).

In the prototype you can:

- Tap the avatar to move through the five states: Recharged, Steady, Busy, Stretched, Needs a pause
- Tap **?** to see why the app thinks you are in that state
- Take a break: live timer, breathing circle, then a before and after check
- Tap any signal (heart rate, HRV, breathing, skin temperature) for detail
- Switch between Home, Insights and Profile, and change settings in Profile

### Start in a specific state

Add parameters to the URL:

| Parameter | Values | Example |
|---|---|---|
| `mood` | `recharged`, `steady`, `busy`, `stretched`, `pause` | `?mood=busy` |
| `tab` | `home`, `insights`, `profile` | `?tab=insights` |
| `screen` | `tabs`, `break`, `done` | `?screen=break` |
| `speed` | `1x`, `10x`, `30x` (break timer speed, default `30x`) | `?speed=1x` |

## Publish with GitHub Pages

1. Create a new repository on GitHub and upload everything in this folder.
2. Open **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then **Save**.
4. After a minute the app is live at `https://<your-username>.github.io/<repo-name>/`.

## Design

- **Fonts:** Bricolage Grotesque (headings), Hanken Grotesk (text), IBM Plex Mono (data), from Google Fonts
- **Base:** white `#FFFFFF`, text `#121614`, secondary text `#4F5854`, hairlines `#E4E9E5`
- **Primary green:** `#06874C`
- **State colours:** Recharged `#FFE27A`, Steady `#BDEFD0`, Busy `#F3E3C3`, Stretched `#FFCFA3`, Needs a pause `#C9DCF7`

## Files

```
index.html          The whole app: markup, styles, logic, a small template
                    renderer and Preact 10.24.3
licenses/           Preact MIT licence
assets/avatars/     Avatar images for each state
```

No build step and no install. Everything runs in the browser.
