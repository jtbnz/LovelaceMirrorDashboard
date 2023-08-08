# LovelaceMirrorDashboard
public view of my mirror dashboard
<a href="Mirror.png"><img src="Mirror.png" height=400></a>
* Layout: I ended up using Layout-Card and Card-Mod to change it to a single column with horizontal and vertical cards filled with the individual cards. found some extra settings to remove the vertical scroll bar

* Time and Date, I wanted the date above the time and I ened up using two different cards - probably could have used the digital-clock one for both

* Location using Life360 and a mushroom template card, the icon changes colour based on battery charge and card-mod to increase the font-size. Kiosk mode used to remove all the extras.

* Shopping List: We use alexa shopping list, so first I changed from anylist to todoist and synced the shopping list into HA, unfortunately there is little control over the shopping list card so then I found the todoist card which meant I didnt need to sync the list to home assistant but it is there now!  Also I have started playing with the powertodoist version of the card which I will probably move over to.

* Energy Now: using energy-flow-plus but about to move over to powerflow plus when I get a chance both from the same developer

* Rain radar: weather-radar-card

* Live Rain and Wind is coming from my netatmo integration (shared data from neighbour as well!)

* Calendar: Atomic Calendar synced to a google shared calendar

Running on a Raspberry Pi, I used [Marco Pascucci](https://mpascucci.github.io/)  guide to autostarting a webpage - just remember to take out the --icognito flag otherwise you will spend hours trying to figure out why your settings are not being saved!

I also have mmwave sensor mounted above the monitor so using hass-screenapi I set an automation to detect presence and turn on the monitor.


**Credits:** 
Layout Card [https://github.com/thomasloven/lovelace-layout-card](https://github.com/thomasloven/lovelace-layout-card)
Card Mod [https://github.com/thomasloven/lovelace-card-mod](https://github.com/thomasloven/lovelace-card-mod)
Kiosk Mode [https://github.com/NemesisRE/kiosk-mode](https://github.com/NemesisRE/kiosk-mode)
Remove vertical scroll bar [https://community.home-assistant.io/t/unnecessary-scroll-bars-using-views-with-layout-cards-like-horizontal-layout-card/493187/4](https://community.home-assistant.io/t/unnecessary-scroll-bars-using-views-with-layout-cards-like-horizontal-layout-card/493187/4)
Guide to sync alexa to todoist (but use the updated script below) [https://community.home-assistant.io/t/sync-your-alexa-todoist-shopping-list-to-the-home-assistant-shopping-list/274277/103](https://community.home-assistant.io/t/sync-your-alexa-todoist-shopping-list-to-the-home-assistant-shopping-list/274277/103)
Updated alexa shoppinglist sync [https://github.com/fenty17/ha-shopping-list-sync](https://github.com/fenty17/ha-shopping-list-sync)


Todoist-card [https://github.com/grinstantin/todoist-card](https://github.com/grinstantin/todoist-card)
powertodoist-card [https://community.home-assistant.io/t/powertodoist-card-lists-kanbans-and-much-more-beta-release/583251/31](https://community.home-assistant.io/t/powertodoist-card-lists-kanbans-and-much-more-beta-release/583251/31)

Time: [https://github.com/fufar/simple-clock-card](https://github.com/fufar/simple-clock-card)
Date: [https://github.com/wassy92x/lovelace-digital-clock](https://github.com/wassy92x/lovelace-digital-clock)

Energy flow: [https://github.com/flixlix/energy-flow-card-plus](https://github.com/flixlix/energy-flow-card-plus)
Powerflow:[https://github.com/flixlix/power-flow-card-plus](https://github.com/flixlix/power-flow-card-plus)

Rain Radar [https://github.com/Makin-Things/weather-radar-card](https://github.com/Makin-Things/weather-radar-card)

Calendar [https://github.com/totaldebug/atomic-calendar-revive](https://github.com/totaldebug/atomic-calendar-revive)

Marcos Guide to starting a raspberry pi into a webpage [https://mpascucci.github.io/tutorial/rpi/](https://mpascucci.github.io/tutorial/rpi/)

Remotely turn on and off the monitor [https://github.com/muddyland/hass-screenapi](https://github.com/muddyland/hass-screenapi)
