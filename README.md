# The Regime

A board game about surviving Stalin's Great Terror. This repository holds the playtest build: the whole game in one web page.

Play it at https://christianabbat-glitch.github.io/the-regime/

## Playing online

1. One player (the host) opens the page and taps **Play online → Host a game**, types a name and gets a four-letter room code.
2. Everyone else opens the same page, taps **Play online → Join a game** and types the code (or the host shares the room link).
3. The host fills any empty seats with the computer and starts the game.

Each player sees only his own hand; the board and the log are shared.

The host's browser runs the game, so the host has to keep the page open until the game ends. If the host's page reloads, the game resumes from the start of the current round.

## Files

- `index.html`: the whole game: rules engine, board, computer players and the online play code.

Online play syncs through a Firebase Realtime Database (project `the-regime-26978`). The Firebase web config inside `index.html` is public by design; access is limited by the database rules to signed-in (anonymous) players.

A rules change only needs a new `index.html` pushed here. Rooms opened with an older version of the page ask players to reload.
