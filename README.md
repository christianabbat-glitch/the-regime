# The Regime

A board game about surviving Stalin's Great Terror.

Play it at https://christianabbat-glitch.github.io/the-regime/

## The current playtest (the reset)

`index.html` is the reset version: secret owners, a corridor where men come forward, five department meetings (Propaganda, NKVD, Industry, Red Army, Judiciary) run with split agenda/response cards, the Lubyanka and its trials, the sharashka, the Gulag queue, the White Sea Canal and exile. The blue NKVD deck is the clock, with one final round after its last card. There is no declared winner yet.

### Online play

Press **Play online** on the start screen, host a room and send the link; the computer plays any empty seat. Every player's browser runs the same game from the same seed, and only decisions travel through Firebase (`rooms/<CODE>/moves`), so every change to the rules or cards applies to online games automatically. A player who reloads replays the room's decisions and catches up. Everyone in a room must be on the same version of the page; a room made with an older version will ask joiners to refresh. For testing several seats on one machine, add `&fake=1` to the address: tabs then share a stand-in database instead of Firebase.

## The classic version

`classic/index.html` is the earlier chips-and-fuses game, including its online play (Firebase rooms): https://christianabbat-glitch.github.io/the-regime/classic/
