# Espresso 1:2

A tiny, free web app (PWA) to log your espresso shots and get one clear piece of advice for the next one — aiming for a **1:2 ratio in 25–30 s**.

**▶ Try it: https://theod997.github.io/espresso-app/**

🌍 Available in **English, Français, Español, 中文, 日本語** — the app picks your phone's language and you can change it anytime in **⚙ Settings**.

Built around a Gaggia Classic Pro and a Kingrinder K6 hand grinder, but the dialing-in logic works with any machine.

---

## Features

- **Fast shot logging** with big +/- buttons: coffee, dose, grinder clicks, time, yield, taste (sour / balanced / bitter), notes
- **Shot diagnosis**: ratio and time vs. target, with targets adjusted to roast level (light 1:1.8–2.5, medium 1:1.8–2.2, dark 1:1.8–2.0)
- **One change at a time**: the app tells you which single variable to adjust (grind, yield, temperature or puck prep) and suggests a **next recipe** you can apply in one tap
- **Smart checks**: choked shots, estimated time at target yield, temperature hints when time and ratio are fine but the shot tastes sour or bitter, puck-prep hints when results are inconsistent at the same setting
- **Per-coffee dashboard**: best setting so far, % of shots on target, sparklines for clicks and ratio
- **Freshness warnings** based on roast date (best 7–30 days after roasting)
- **History** with edit/delete, **CSV export and import** (backup or move to a new phone)

## Privacy & offline

- No account, no server, no tracking: everything is stored **locally on your device**.
- Every user starts with an empty app — nothing is shared between users.
- Works offline once installed.

## Install on your phone

**Android (Chrome):** open the link → menu **⋮** → **Add to Home screen** → **Install**.
**iPhone (Safari):** open the link → **Share** → **Add to Home Screen**.

## Back up your data

Shots live in your browser only: they are lost if you uninstall the app, clear browser data or switch phones.
Export regularly with **History → Export CSV**, and restore with **History → Import CSV**.

## Tech

Plain HTML/CSS/JavaScript in a single `index.html` — no framework, no build step. Translations are in the `I18N` object at the top of the script; adding a language means adding one block.

To push an update to installed apps, bump the cache name (`espresso-app-v1`) in `service-worker.js`.

## Feedback

Issues, suggestions and translation fixes are welcome.
