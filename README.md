# CowinAlerter-Node <img align="right" alt="GitHub package.json version" src="https://img.shields.io/github/package-json/v/akshayitzme/cowinAlerter-node?style=for-the-badge">

<img src="https://i0.wp.com/www.platformafrica.com/wp-content/uploads/2021/03/c2.png?fit=1800%2C550&ssl=1" alt="covid banner"/>

![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=for-the-badge) 
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/akshayitzme/cowinAlerter-node/CodeQL?style=for-the-badge)
![GitHub top language](https://img.shields.io/github/languages/top/akshayitzme/cowinAlerter-node?style=for-the-badge)
![Lines of code](https://img.shields.io/tokei/lines/github/akshayitzme/cowinAlerter-node?style=for-the-badge)
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/atikjaz/cowinAlerter-node)

Automatically checks for available slots every 15 seconds, sends Alerts via Telegram. 

## Features
- Heroku Ready.
- Checks Slot Availability of 5 days.
- Supports  Finding Slots by Pin Code & District Code.
- Personalized Alerts.. Alerts based on Users Age Group, Dose, FirstDose..etc
- Checks Slot Availability in background.

## Set Up

### Heroku

- Fork this Repository
- Add Users in *[Users.json](/Database/Users.json)*
	refer this [gist](https://gist.github.com/akshayitzme/57f4c1cba4d3a22f4f2e145b94a225e1)
- Connect Forked GitHub repo to Heroku.
- Set Telegram Bot Id in Heroku Config Vars. *[see guide](https://devcenter.heroku.com/articles/config-vars)* also see *[env.example](env.example)*
- Add NodeJs Buildpack.
- Deploy App

### LocalHost 
- Clone this Repository
- Add Users in *[Users.json](/Database/Users.json)*
	refer this [gist](https://gist.github.com/akshayitzme/57f4c1cba4d3a22f4f2e145b94a225e1)
- Set Telegram Bot Id in `.env` file.  see *[env.example](env.example)*
- Install Dependencies
	 `yarn install`  or  `npm i`
- Run Server
	```bash 
	node index
	```
**Works well in all other Hosting Platforms.**

## Notes
- to find district ID, use this [API](https://apisetu.gov.in/public/marketplace/api/cowin#/Metadata%20APIs/districts)

## References
[APISetu](https://apisetu.gov.in/public/marketplace/api/cowin#/)

## Licence
![GitHub](https://img.shields.io/github/license/akshayitzme/cowinAlerter-node?style=for-the-badge)
