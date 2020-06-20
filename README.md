# Python-The-Odds-Api-Wrapper
Python wrapper around The Odds-Api.
## Description & Implementation
A full Python Wrapper around The Odds-API which provides sports odds data for loads of sports from bookmakers around the world.
Get your free API key at https://the-odds-api.com/. 
## Usage
Please refer to https://the-odds-api.com/liveapi/guides/v3/ for detailed instructions for The Odds-Api. Below is a simple example of the usage.
```
from oddsapi import OddsClient

client = OddsClient(api_key="your api key")
sports = client.retrieve_sports()
odds = client.retrieve_odds(
    sport_key='americanfootball_ncaaf',
    region='us',
    mkt='spreads'
)
print(f"Requests Remaining: {client.requests_remaining}")
print(f"Requests Used: {client.requests_used}")
```