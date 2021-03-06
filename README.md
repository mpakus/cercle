# Cercle CRM for smart people & Trello lovers - Phoenix & Vuejs 

Cercle is a CRM for smart people who need more clients.

Easy to keep track of your sales, partnerships, support tickets, onboarding clients. 

[Try Cercle Today. Click here: http://www.cercle.co/register](http://www.cercle.co/register)

## Why Cercle?
- realtime
- visual
- simple
- API ready
- open source
- free if you install it by yourself
- $1.99 per month with unlimited number of users if we do the hosting for you.

## Current features
- Import CSV
- Contact Tags
- Contact Organization
- Each Contact can be linked to visual Card into a Board
- Board Timeline on a sidebar
- Board Archive/Unarchive
- Card Attachements
- Card Tasks
- Card Comments
- Card Email Notification System for team member
- Oauth for API in Zapier


## Changelog

### June 7 2017, V1.0 Release Candidate

#### New Feature

- Oauth Integration with Zapier
- Add Full name option during CSV Import



## To install Cercle on Local

You need to setup a postgresql DB version 9.5

1. Rename to dev.secret_example.exs to dev.secret.exs
2. Fill out the parameters
3. Run the migration
4. You're good to go!

## To Install Cercle into heroku
1. mix phoenix.gen.secret
2. heroku config:set SECRET_KEY_BASE="your_key_here"
3. heroku config:set POOL_SIZE=18
4. add others parameters from dev.secret into Heroku config:set
5. You're good to go!

## Using Docker For Development
1. Given you already have docker and docker-compose installed on your machine, Simply run these following commands:
```
# Build all and pull images and containers
docker-compose build
# Build application dependencies.
# This will set permission to allow our build script to run.
chmod +x build
./build
# Build the Docker image and start the `web` container, daemonized
docker-compose up -d web
```

## Contribution
Feel free to send your PR with proposals, improvements or corrections!

## License
Copyright © 2016-2017 AK Cercle Inc.

Licence LGPL v3.


