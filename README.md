## Frequently Asked Questions (& Answers)

Q: When (and how often) do the football.json datasets get updated?

A: The football.json datsets of the latest season (that is, 2026 & 2026/27) 
get auto-updated once a day (5 o'clock UTC) from the upstream Football.TXT datasets via a github action,
see the [action log @ yorobot/football.json](https://github.com/yorobot/football.json/actions) for details.

Note, however,  for the upstream Football.TXT datasets for now there's no automatic (daily) update.
See [Updates / Contributions Welcome - Please Update the Football.TXT Sources](#updates--contributions-welcome---please-update-the-footballtxt-sources) for details.



# football.json

Free open public domain football (match fixtures & results) data in the JSON (JavaScript Object Notation)
data interchange format.

Leagues include:

- English Premier League, Championship, League One, League Two
- Deutsche Bundesliga, 2. Bundesliga, 3. Liga
- Spanish Primera División ("La Liga"), Segunda División
- Italian Serie A, Serie B
- French Ligue 1, Ligue 2
- and much more

Example - Premier League 2015/16 Match Schedule (Fixtures and Results) - [`2015-16/en.1.json`](https://raw.githubusercontent.com/openfootball/football.json/master/2015-16/en.1.json):

``` json
{
  "name": "Premier League 2015/16",
  "matches": [
        {
          "round": "Matchday 1",
          "date":  "2015-08-08",
          "team1": "Manchester United",
          "team2": "Tottenham Hotspur",
          "score": { "ft": [1, 0] }
        },
        {
          "round": "Matchday 1",
          "date":  "2015-08-09",
          "team1": "Arsenal",
          "team2": "West Ham United",
          "score": { "ft": [0, 2] }
        },
        ...
  ]
}
```





## How to Use the Public JSON API Service - No API Key Required ;-)

Use the "raw" links served by GitHub (
otherwise you get the complete "formatted" GitHub page). Example:

```
$ curl https://raw.githubusercontent.com/openfootball/football.json/master/2015-16/en.1.json
```


## Updates / Contributions Welcome - Please Update the Football.TXT Sources

Note: The Football.JSON files get (auto-)generated using the datasets in the Football.TXT format, thus, **please do NOT
edit the (auto-)generated JSON files here but the Football.TXT sources upstream in the country repos** e.g.:

- English Premier League, Championship, League One, League Two in [**`/england`**](https://github.com/openfootball/england)  ([**online page index**](https://openfootball.github.io/england/))
- Deutsche Bundesliga, 2. Bundesliga, 3. Liga in [**`/deutschland`**](https://github.com/openfootball/deutschland)  ([**online page index**](https://openfootball.github.io/deutschland/))
- Spanish Primera División ("La Liga"), Segunda División in [**`/espana`**](https://github.com/openfootball/espana)   ([**online page index**](https://openfootball.github.io/espana/))
- Italian Serie A, Serie B in [**`/italy`**](https://github.com/openfootball/italy)   ([**online page index**](https://openfootball.github.io/italy/))
- French Ligue 1, Ligue 2 in [**`/france`**](https://github.com/openfootball/europe/tree/master/france) (in [`/europe`](https://github.com/openfootball/europe))   ([**online page index**](https://openfootball.github.io/europe/))
- and so on


and than wait to get the (auto-)generated football.json updates. If you only edit / patch the (auto-)generated JSON files here without updating
the sources upstream than your changes will get lost / overwritten with the next update.


## Do-It-Yourself (DIY) - How To (Auto)-Generate and Update the football.json Datasets

If you want to help out updating the (auto-)generated football.json datasets right here from the sources - you are more than welcome. See the [`yorobot/football.json`](https://github.com/yorobot/football.json) build scripts to get started
or use your very own.


Or as a quick alternative 
you can use the [`fbtxt2json` command-line tool](https://github.com/sportdb/footty/tree/master/fbtxt2json) to convert any (match data) file in the Football.TXT format to JSON. 

Let's try to convert the English Premier League 2026/27
in the Football.TXT format (see [`england/2026-27/1-premierleague.txt`](https://github.com/openfootball/england/blob/master/2026-27/1-premierleague.txt)) to JSON:

```
$ fbtxt2json england/2026-27/1-premierleague.txt -o en.1.json
```

Tip - Or try to convert the complete [`/england`](https://github.com/openfootball/england) repo at once:

```
$ fbtxt2json . -o ./_site   # run inside /england; output json datasets to _site directory
```



## Add Your Leagues and Tournaments!

Any leagues or tournaments missing? Contributions welcome!
For starting your own repo from scratch see the [League Quick Starter Kit](https://github.com/openfootball/league-starter).


## More - Add Your Scripts Here

Enrique Lopez Magallon (@enadol) writes:

> Greetings! I started coding the following python robot to read the .txt files
> (for instance, "1-bundesliga-i.txt)" and generate an emulated version of the JSONs featured in football.json.
>
> https://github.com/enadol/fbjsonrobot
>
> Just make sure the proper .txt file is on the same folder, launch the file launch.py and that's (almost) it!
> For other leagues, adapt is required.
>
> It's still not perfect, but that's Github is for! 😄
>
> Have fun! ⚽️ ⚽️

Nurgazy Nazhimidinov (@nurgasemetey) writes:

> I use [the football.json datasets] in my tool.
>
> Basically it compares the last season and this season head-to-head results of the [English Premier League] team.
>
> Here is the link: https://compare-last-season.netlify.app/
>
> Here is the source code: https://github.com/nurgasemetey/compare-last-season

Rodolfo Melogli (@BusinessBloomer) writes:

> I use the openfootball Football.TXT fixture data for Serie A and the Premier League to power [fantatools.com](https://fantatools.com/en/), a set of free fantasy-football tools — fixture difficulty ratings and "next 5" run-in rankings for Fantacalcio and FPL.
>
> https://fantatools.com/en/


## License

The football.json schema, data and scripts are dedicated to the public domain. Use as you please with no restrictions whatsoever.



## Questions? Comments?

Yes, you can. More than welcome.
See [Help & Support »](https://github.com/openfootball/help)

