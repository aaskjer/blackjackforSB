## Classic Blackjack Game for streamer.bot

:game_die: **Dynamic Betting** Bet a specific amount or let the script randomly select a bet if none is specified.
:star: **Special Win Conditions** Instant wins for a 5‑card Charlie or three 7s.
:warning: **Tie-Breaker Logic** If you tie with the dealer, a backup card can be drawn to determine the outcome.
:moneybag: **Configurable Payouts** Natural blackjack pays 3:2; standard wins pay 1:1, with some multipliers.
:arrow_forward: **Multi-Platform Support** Compatible with Twitch, YouTube, and Trovo.
:lock: **Singleplayer Game** Every user has it's own Game instance!


[center][wrap="warning"]CBJG may not work properly with alpha version of SB![/wrap][/center]
# **Import Files**  
:inbox_tray: **[Releases](https://github.com/aaskjer/blackjackforSB/releases)**


# **Installation**
:warning: **Prerequisite**: A working point system is required.
1. Import the script into Streamer.bot.
2. Drop the 'cards' folder into the root folder of SB.
3. Adjust arguments if needed.
    *(Optional)* Add the OBS overlay:
    1. Install https://obsproject.com/forum/resources/source-copy.1261/
    2. In OBS: `Tools > Source Copy > Load scene > blackjack-OBS-import.json`
    3. Check if the images are still look fancy.
4. Start playing Blackjack!


# **Commands**  
- `!blackjack <bet>`: Start a new game with your bet (or leave out the bet to use a random amount).
- `hit`: Draw an additional card.
- `stand`: End your turn and let the dealer play.
- `repeat`: for crowded chats so you can see your current cards again.


# **Changelogs**

**v7**
* Now, the game creates one shared deck per game instance. Dealer and the player draw from the same shared shuffled deck, unlike before.
* Renamed the Scene to `Blackjack - Game` to prevent overwriting old setups
* The Game now correctly set up a scene and a browser source for the cards in OBS. 
  * All you need to do is, drop the `cards` folder in the root folder of your streamer.bot and everything should be good.
  * The Design for the game is up to you, but you still can use `source copy` to import my copy of the game if you want to use my images.
