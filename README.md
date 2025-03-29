# Brackito!

![Brackito Logo](https://github.com/user-attachments/assets/73fe952b-270a-430c-9875-6d16ac63cf63)

**Brackito** is a simple yet feature-rich **cloud**-enabled tournament **bracket editor and visualizer**!

Organize your tournaments with an easy-to-use UI and update your brackets **live on the cloud** for your participants to see!

## Installation

🚀 **HTML Version:** [Brackito v1.html](https://github.com/FiFiFiZ/Brackito/blob/1221f32ba39174f723c6c6297ca90041bd8315e1/Brackito%20v1.html)

🐈 **Scratch Version:** [Brackito v1.sb3](https://github.com/FiFiFiZ/Brackito/blob/1221f32ba39174f723c6c6297ca90041bd8315e1/Brackito%20v1.sb3) (Cloud will only work if uploaded to Scratch and run on TurboWarp.)

## Instructions
### Editing brackets

- To **create** a live **online** bracket, type **"``1``"** at the initial prompt to enable admin mode.

- To make your bracket **offline**, save your bracket code and load it at the initial prompt by typing "``/load``".

![Editing](https://github.com/user-attachments/assets/ebd4b499-6f1d-4a45-ae8f-a77e61e33373)

### Reading brackets

To check on the currently live bracket, leave the initial prompt blank and enter. 

Hovering over the "``•LIVE``" label indicates the last modification done on the bracket.

- Move around with your mouse or arrows (or gliding with your finger on mobile).
- Zoom in and out with the scroll wheel.

![Cloud](https://github.com/user-attachments/assets/faf4b72b-48e9-4b9f-bbca-97adb6cf6c5c)

## Documentation

The bracket uses a special **"Pool to Double-Elimination"** format:

- Seeded players are first sorted in a serpentine pattern in groups of 3~4 depending on the number of participants. 
Group match winners proceed to "Winner's Bracket", losers proceed to "Loser's Bracket".

- There can be up to 3 groups of 3 participants in the pool phase; if the number of participants isn't a multiple of 4, then: `number_of_groups_of_3 = 4 - (number_of_participants % 4)`

This bracket system also advantages a higher seed in many ways:

- Group matches count ties as wins for the higher seeded player to advantage a higher seed. In the double-elimination phase however, a strict win is required.

Although the system advantages high seeds, it still gives lower-seeded players more chances than a regular double-elimination tournament would by making the lowest possible amount of matches played before elimination 3 (this increases to 4 if the player is in a 4-player-group, which in a bigger tournament is more likely).

## Credits
https://stackoverflow.com/questions/8355264/tournament-bracket-placement-algorithm - Helpful post on how to recursively set up the Winner's Bracket.

https://officepoolstop.com/Brackets.aspx - Browser-based small tournament maker, allowed for analyzing the order in which Loser's Bracket matches are ordered.

https://www.youtube.com/watch?v=h7ZvnNlRLJg&ab_channel=FIVBTUTO - Video about pool matches explaining how they are set up.







