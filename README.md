# football.json

Free open public domain football data in the JSON (JavaScript Object Notation)
data interchange format.

Leagues include:

- English Premier League
- Deutsche Bundesliga
- Spanish Primera División ("La Liga")
- Italian Serie A
- and more

Example - Premier League 2015/16 Match Schedule (Fixtures and Result) - [`2015-16/en.1.json`](https://raw.githubusercontent.com/openfootball/football.json/master/2015-16/en.1.json):

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


Example - Premier League 2015/16 Clubs - [`2015-16/en.1.clubs.json`](https://raw.githubusercontent.com/openfootball/football.json/master/2015-16/en.1.clubs.json):

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

## How to Use the Public JSON API Service - No API Key Required ;-)

Use the "raw" links served by GitHub (
otherwise you get the complete "formatted" GitHub page). Example:

```
$ curl https://raw.githubusercontent.com/openfootball/football.json/master/2015-16/en.1.clubs.json
```


## Updates / Contributions Welcome - Please Update the Source Text Files

Note: The JSON files get (auto-)generated using the football.db datasets, thus, **please do NOT
edit the JSON files but the source text files in the country repos** e.g.:

- English Premier League in [`/eng-england`](https://github.com/openfootball/eng-england)
- Deutsche Bundesliga in [`/de-deutschland`](https://github.com/openfootball/de-deutschland)
- Spanish Primera División ("La Liga") in [`/es-espana`](https://github.com/openfootball/es-espana)
- Italian Serie A  in [`/it-italy`](https://github.com/openfootball/it-italy)
- and so on



<!--
## Automate, Automate, Automate


If all works weekly updates get pushed by yorobot.
See the [`yorobot/football.db`](https://github.com/yorobot/football.db) build scripts for
the (auto-)update machinery.

  todo: add how to build your own json files from the source datsets - why? why not?
-->


## Contributions Welcome - Add Your Leagues and Tournaments!

Any leagues or tournaments missing? Contributions welcome!
For starting your own repo from scratch see the [League Quick Starter Kit](https://github.com/openfootball/your-league-starter).



## More

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

## License

![](https://publicdomainworks.github.io/buttons/zero88x31.png)

The football.json schema, data and scripts are dedicated to the public domain. Use it as you please with no restrictions whatsoever.


## Questions? Comments?

Send them along to the
[Open Sports & Friends Forum/Mailing List](http://groups.google.com/group/opensport).
Thanks!
