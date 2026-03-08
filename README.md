# Xenolingual Numeral Decoder

A translator for the Eridian base-6 number system from Andy Weir's *Project Hail Mary*.

## Features

- Translates Eridian base-6 numerals to decimal
- Time mode: converts Eridian time units to Earth time (1 unit = 2.366s)
- Offline-capable PWA — works without a connection after first visit
- Installable to home screen

## Numeral System

| Symbol | Value |
|--------|-------|
| ℓ | 0 |
| I | 1 |
| V | 2 |
| λ | 3 |
| + | 4 |
| V̶ | 5 |

Numbers are read left to right in base 6. Keyboard input supported (keys `0`–`5`, `Backspace`, `Esc`).

## Running

```bash
docker compose up --build
```

Docker assigns a random host port — check the logs or run `docker compose ps` to find it.

## Deployment

Hosted at `calculator.caskey.cloud` (home network only). The service worker caches the app on first load so it remains usable offline.
