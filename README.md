# football.json

Free open public domain football data in the JSON (JavaScript Object Notation)
data interchange format.

Leagues include:

- English Premier League
- Deutsche Bundesliga
- Spanish Primera División ("La Liga")
- Italian Serie A
- and more

Example - Premier League 2015/16 Match Schedule (Fixtures and Result) - [`2015-16/en.1.json`](https://github.com/openfootball/football.json/blob/master/2015-16/en.1.json):

``` json
{
  "name": "English Premier League 2015/16",
  "rounds": [
    {
      "name": "Matchday 1",
      "matches": [
        {
          "date": "2015-08-08",
          "team1": {
            "key": "manutd",
            "name": "Manchester United",
            "code": "MUN"
          },
          "team2": {
            "key": "tottenham",
            "name": "Tottenham Hotspur",
            "code": "TOT"
          },
          "score1": 1,
          "score2": 0
        },
        {
          "date": "2015-08-09",
          "team1": {
            "key": "arsenal",
            "name": "Arsenal",
            "code": "ARS"
          },
          "team2": {
            "key": "westham",
            "name": "West Ham United",
            "code": "WHU"
          },
          "score1": 0,
          "score2": 2
        },
        ...
      ]
    }
  ]
}
```


Example - Premier League 2015/16 Clubs - [`2015-16/en.1.clubs.json`](https://github.com/openfootball/football.json/blob/master/2015-16/en.1.clubs.json):

``` json
{
  "name": "English Premier League 2015/16",
  "clubs": [
    {
      "key": "chelsea",
      "name": "Chelsea",
      "code": "CHE"
    },
    {
      "key": "arsenal",
      "name": "Arsenal",
      "code": "ARS"
    },
    {
      "key": "manutd",
      "name": "Manchester United",
      "code": "MUN"
    },
    ...
  ]
}
```


## Automate, Automate, Automate

Note: The JSON files get (auto-)generated using the football.db datasets, thus, please do NOT
edit the JSON files but the source files in the country repos e.g.:

- English Premier League in [`/en-england`](https://github.com/openfootball/eng-england)
- Deutsche Bundesliga in [`/de-deutschland`](https://github.com/openfootball/de-deutschland)
- Spanish Primera División ("La Liga") in [`/es-espana`](https://github.com/openfootball/es-espana)
- Italian Serie A  in [`/it-italy`](https://github.com/openfootball/it-italy)
- and so on


If all works weekly updates get pushed by the skriptbot.
See the [`skriptbot/football.json`](https://github.com/skriptbot/football.json) scripts for
the (auto-)update machinery.



## Contributions Welcome - Add Your Leagues and Tournaments!

Any leagues or tournaments missing? Contributions welcome!
For starting your own repo from scratch see the [Mauritius League Quick Starter Kit](https://github.com/sportkit/mu-mauritius).


## License

The football.json schema, data and scripts are dedicated to the public domain. Use it as you please with no restrictions whatsoever.


## Questions? Comments?

Send them along to the
[Open Sports & Friends Forum/Mailing List](http://groups.google.com/group/opensport).
Thanks!
