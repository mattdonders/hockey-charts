# Hockey Analytics Charts
Automatically generated hockey charts (via data from Natural Stat Trick).

## Usage
This Python script requires (at least) an NHL Short Name (ex - New Jersey Devils becomes Devils). If no `gameid` argument is passed into the script it will determine if the game is being played today and will wait until it finds an intermission to generate charts. 

```
$ python all_charts.py --help
usage: all_charts.py [-h] --team TEAM [--gameid GAMEID]

optional arguments:
  -h, --help       show this help message and exit
  --team TEAM      NHL Team Shortname
  --gameid GAMEID  NHL Game ID
```

The script will also try to detect a local html (ex - `20100.html`) file that is a dump of a Natural Stat Trick Full Report for that game_id within the project folder. If it detects a local file, it will use that instead of going to Natural Stat Trick to retrieve a new Full Report file.

## To-Do
- Add sample images to repository & this README file.
- Better logging, error handling and completion notification.
- Convert GameScore chart to an appropriate graph / chart.
