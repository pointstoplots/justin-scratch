Scratch project for exploring different ideas.  

You'll need to install `nba-cli` before using this project.

```
git clone https://github.com/caged/nba-cli
cd nba-cli
npm install
nba-stats --help
```

### Getting started

```
script/bootstrap
```


### Notes

* Data includes potentially duplicate headers that are differentiated by casing.  FGmG vs. FGMG.
* Percentile is computed later as:

```
Percentile = e.WorsePPP / (e.WorsePPP + e.BetterPPP) * 100
```

* The defensive [Handoff dataset](http://stats-prod.nba.com/wp-json/statscms/v1/synergy/player/?category=Handoff&limit=500&name=defensive&q=2474171&season=2016&seasonType=Reg) is incorrect.  Note the results where `PlayerIDSID` is a team abbreviation and `FGA` is a players last name.
