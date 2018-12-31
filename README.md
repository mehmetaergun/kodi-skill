# <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/tv.svg' card_color='#40DBB0' width='50' height='50' style='vertical-align:bottom'/> Kodi Control Skill
Control KODI open source media center with Mycroft.ai

## About 
Utilize the kodi API and Python library for controlling the KODI open source media center with Mycroft.ai. The control is mostly geared towards videos/movies but is capable of handling cursor navigation as well.
The Kodi Skill uses conversational dialog to help you to control your KODI instance more naturally. 

## Examples 
* "play the movie guardians of the galaxy on Kodi"
* "play the film planet of the apes on Kodi"
* "turn kodi subtitles on"
* "turn kodi subtitles off"
* "skip movie forward"
* "skip movie backward"
* "pause the movie on Kodi"
* "re-start the movie on Kodi"
* "stop the movie on Kodi"
* "show the movie information"
* "hide the movie information"
* "turn kodi notifications on"
* "turn kodi notifications off"
* "move the cursor up / down / left / right / back / select / cancel"
* "move the cursor right 3 times"
* "move the cursor down twice"
* "update the kodi library"
* "clean the kodi library"
* "list recently added movies"
* "list the movies by genre"
* "list the movies by studio"
* "list movie sets"
* "list movies by title"
* "list movies by actor"
* "list all movies"
## Conversational Context
** If mycroft.ai locates more than one movie that matches your request it will permit you to itterate through your requests
using conversational context.
* eg. "hey mycroft:"
* Request: "play the movie Iron Man on Kodi"
* Response: "I have located 3 movies with the name Iron Man, would you like me to list them?"
* Request: "yes" / "no"
* Response: "Iron Man, to Skip, say Next, say play, to play, or Cancel, to stop"
* Request: "next" / "skip"
* Response: "Iron Man 2"
* Request: "play" / "select"
* Response: "o-k, attempting to play, Iron Man 2"
## Cinemavision Addon
If mycroft.ai locates the addon CinemaVision it will prompt the user if this addon should be used during the 
playback of the movie that was selected.
* Response: "Would you like to play the movie using cinemavision?"
* Request: "yes / no"
## Youtube Addon
* Request: "play some Elton John from youtube on Kodi
* Request: "Play the official captain marvel trailer from youtube on Kodi"
* Request: "Stop youtube"
## Credits 
* Cadair, PCWii
* Original work forked from https://github.com/Cadair/mycroft-kodi; https://github.com/pcwii/kodi-skill
## Category
**Media**
## Tags
'#kodi, #mycroft.ai, #python, #skills'
## Require 
Tested on platform_picroft (others untested) 
## Other Requirements
- [Mycroft](https://docs.mycroft.ai/installing.and.running/installation)
- kodipydent
## Further Reading
- [KODI API](https://kodi.wiki/index.php?title=JSON-RPC_API/v8)
- [CinemaVision](https://kodi.wiki/view/Add-on:CinemaVision)
## Installation Notes
- Configure Kodi to “allow remote control via HTTP”, under the Kodi settings:services
- Configure Kodi to “allow remote control from applications on other systems”, under the Kodi settings:services
- Under Kodi settings:services note the port number (8080)
- Configure home.mycroft.ai to set your kodi instance ip address and port number
## Todo
- Enable Kodi Volume Control (TODO)
- Explore removing CinemaVision (TODO)
