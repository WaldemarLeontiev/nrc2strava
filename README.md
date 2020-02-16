# nrc2strava

Most accurate way to import NRC & NTC activities to Strava (includes elevation & heart rate data)

## Install

- Install [Node](https://nodejs.org/)
- **npm install**

## Usage

- Specify **env** variables
- **npm start nike** - fetch all Nike Run Club activities that have **GPS** data and create gpx files
- **npm start strava** - upload all gpx files to Strava

### Notes

1. Gpx file for activity without GPS data will not be created
2. You need to specify **env** variables to fetch and upload
3. You can get **NIKE** bearer token by login to your account - [website](https://www.nike.com/), and look for any _api.nike.com_ request
4. You need _activity:write_ scope **STRAVA** token, you can get it by login to [website](http://strava-statistics.herokuapp.com/) and change the scope in url on strava auth page, then look for token cookie
5. Duplicated activities will not be loaded
6. It is just a fast working solution