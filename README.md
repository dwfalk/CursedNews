# cursednews
A python curses news app for Linux
## About 
From my desire to augment eDEX-UI by GitSquared *(check it out if you haven't already, it's an awesome piece of work)* with a news search feature that is something akin to Neo's newspaper search for Morpheus in The Matrix. 

## Examples 
* "scanning news sources..."
```
┌───────────────────────────────────────────────────────────────────────────
│ scanning news sources...
└───────────────────────────────────────────────────────────────────────────
│ 0: <abc-news-au> ABC News (AU)
│ 1: <al-jazeera-english> Al Jazeera English
│ 2: <ars-technica> Ars Technica
│ 3: <associated-press> Associated Press
│ 4: <bbc-news> BBC News
│ 5: <bbc-sport> BBC Sport 
```

* "scanning headlines"
```
┌───────────────────────────────────────────────────────────────────────────
│ scanning headlines for <associated-press>...
└───────────────────────────────────────────────────────────────────────────
│ 0: Pandemic haunts new year as virus growth outpaces vaccines...
│ 1: Georgia deciding US Senate control in election's final day...
│ 2: Teen charged in Wisconsin protest shootings to enter plea...
│ 3: 'Enough is enough': Ohio lawmakers, family honor Andre Hill...
│ 4: Trump allies scrambling for strategy to overturn Biden win...
│ 5: Loyal soldier Pence torn between Trump, Constitution...
│ 6: If I’ve already had the coronavirus, can I get it again?...
│ 7: EXPLAINER: Breaking down Biden’s Iran problem...
│ 8: One Good Thing: Theft leads to community giving in Miami...
│ 9: American Airlines is grounding emotional-support animals...
```
* "q" - quits
* "p" - pauses
* "r" - resumes
* "0" - summarizes article 0
* "1" - summarizes article 1
* ...
* "l" - return to list from summary

* You can also edit the populated **~/.config/cursednews/cursednews.xml** and "include" only specific sources rather than allow them to "default".

## Credits 
@dwfalk - Original developer

## Dependencies
python3 -m pip install requests

## Category
**Entertainment**

## Tags
#news
#curses
#linux

## Installation:
- git clone https://github.com/dwfalk/cursednews
- cd cursednews
- chmod +x cursednews
- apt install python3-lxml
- apt install python3-pip
- python3 -m pip install requests
- register for a free newsapi.org key [here](http://newsapi.org/register). *Note: Free version limited to 100 requests in a 24hr period.*
- create initial config file **~/.config/cursednews/cursednews.xml** using the example below
```xml
<cursednews>
  <news_api_key>YOUR_NEWS_API_KEY_GOES_HERE</news_api_key>
</cursednews>
```
- ./cursednews

