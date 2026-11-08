# Oche Legends

A retro pixel-art darts game for the browser, for one or two players.

Time your throw as the hand drifts across the board, then work your way up a ladder of sixteen pub players, or pick a player and try to win a 16-player knockout tournament. Games available are 501, 301 and Round the Clock, played as best of 1, 3 or 5.

Matches have a recorded scorer calling scores and legs, and the title screens have their own music. In a 2 player game, each player picks one of the sixteen characters to play as. All the characters are fictional.

## Controls

- The arrow keys flip the hand's diagonal direction.
- Space, or a tap on a phone, throws the dart.
- 1 opens the ladder, 2 a 2 player game, 3 the tournament, P practice and Esc the menu.

## Portraits

Each character has a 48 x 48 portrait. Finished pixel art goes in `PORTRAIT_DATA` in `index.html` as a data URI keyed by the character's id; anyone without one gets a portrait drawn in code from their look in `OPPONENTS`. All 16 players now have portraits generated with PixelLab (pixellab.ai) from text descriptions of their personas; the drawn-in-code versions remain as a fallback.

## Scorer voice

Clips live in `sounds/voice`. Per-character calls (`name-<id>.mp3` and `game-<id>.mp3`) are optional: add the id to the list next to `VOICE` once both files exist.

The whole game is a single `index.html` file with no build step. Open it in a browser to play locally.
