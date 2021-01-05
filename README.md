# cursednews
CursedNews python app for Linux
## About 
From my desire to augment eDEX-UI by GitSquared with a news search feature that is something akin to Neo's newspaper search for Morpheus in The Matrix. 

## Examples 
* "scanning news sources..."
┌─────────────────────────
│ scanning news sources...
└─────────────────────────
│ 0: ```xml<abc-news-au>``` ABC News (AU)
│ 1: ```xml<al-jazeera-english>``` Al Jazeera English
│ 2: ```xml<ars-technica>``` Ars Technica
│ 3: ```xml<associated-press>``` Associated Press
│ 4: ```xml<bbc-news>``` BBC News
│ 5: ```xml<bbc-sport>``` BBC Sport 

* "scanning headlines"
┌─────────────────────────
│ scanning headlines for ```xml<associated-press>```...
└─────────────────────────
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

* "q" - quits
* "p" - pauses
* "r" - resumes
* "0" - summarizes article 0
* "1" - summarizes article 1
* ...
* "l" - return to list from summary

* You can also edit the populated .config/cursednews/cursednews.xml and "include" only specific sources rather than allow them to "default".

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

To install:
git clone https://github.com/dwfalk/cursednews
chmod +x cursednews
apt install python3-lxml
apt install python3-pip
python3 -m pip install requests
register for a free newsapi.org key [here](http://newsapi.org/register) .
create initial config file .config/cursednews/cursednews.xml using the example below

```xml
<cursednews>
  <news_api_key>YOUR_NEWS_API_KEY_GOES_HERE</news_api_key>
</cursednews>
```

