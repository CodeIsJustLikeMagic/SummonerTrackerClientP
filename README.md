# SummonerTrackerClientP
SummonerTracker Overlay

Press the hotkey (default: ^) to open the Setter Window in game and start timing summoner spells.
The summoner spell Buttons will assume that the spell has been used 7 seconds ago. 
The "-1min" Buttons will assume the spell has been used 1 minute ago.
To remove a spell timer press the button again.

If another summoner on your team uses the overlay you will share information with each other.

When you start the overlay it will create a tray icon (next to the time and date in the windows tool bar).
From there you can set your prefered hotkey (examples include: ^; space; shift+s) and move the Information Display Window and the Setter Window.

The overlay is not visible if you play in fullscreen mode.

[Download here](https://github.com/CodeIsJustLikeMagic/SummonerTrackerClientP/releases/latest)


How it works: The riot live game api is used to find current game information to set the champions and spells in the Setter Overlay.
(Please be aware that the ulimate cooldows are not loaded via api. They are allways tracked with 110 seconds cooldown regardless of champion)
Information is shared via mqtt. Your team information (Summonernames and teamid) is used to create the topic. All your team members listen and publish to the same topic.

The positions of the windows and the hotkey are saved in %Appdata%\SummonerTrackerOverlay after you have started the overlay once.

This Tracker DOES NOT track spells automatically. You have to start the timers yourself.
