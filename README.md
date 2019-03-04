# Description
Thanks to [BattleSnake](https://battlesnake.io) for the amazing competition and online platform!

A simple (incomplete and buggy) snake made during the 2019 BattleSnake competition in Victoria, BC made by [coco99166](https://github.com/coco99166), [Yuming H](https://github.com/yuming-h), [ajyxc](https://github.com/ajyxc), [yaoharry](https://github.com/yaoharry) and myself. 

I am making a _hopefully improved_ continuation of this snake on my own [here](https://github.com/MuchToKnow/sauder)

The snake currently evaluates *single* gamestates and doesn't attempt any prediction.  The snake can pathfind and move to food but doesn't handle cases where
* There is no food on the board
* There is no current viable path to food

The snake is quite naive and considers other snakes and itself as walls, not considering that their tail will be vacated in the next turn.

It is quite incomplete and you can feel free to fork and add:
* Attacking patterns
* Holding patterns
* Defending patterns
* Predicted game state consideration

# Getting Started

A simple [Battlesnake AI](https://battlesnake.io) written in Javascript for NodeJS.

To get started you'll need a working NodeJS development environment, and at least read the Heroku docs on [deploying a NodeJS app](https://devcenter.heroku.com/articles/getting-started-with-nodejs).

If you haven't setup a NodeJS development environment before, read [how to get started with NodeJS](http://nodejs.org/documentation/tutorials/). You'll also need [npm](https://www.npmjs.com/) for easy JS dependency management.

This client uses [Express4](http://expressjs.com/en/4x/api.html) for easy route management, read up on the docs to learn more about reading incoming JSON params, writing responses, etc.

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Running the AI locally

Fork and clone this repo:

```shell
git clone git@github.com:battlesnakeio/starter-snake-node.git
cd battlesnake-node
```

Install the client dependencies:

```shell
npm install
```

Create an `.env` file in the root of the project and add your environment variables (optional).

Run the server with auto-reloading on file change:

```shell
npm start
```

Test the client in your browser at <http://localhost:5000>

## Deploying to Heroku

Click the Deploy to Heroku button at the top or use the command line commands below.

Create a new NodeJS Heroku app:

```shell
heroku create [APP_NAME]
```

Push code to Heroku servers:

```shell
git push heroku master
```

Open Heroku app in browser:

```shell
heroku open
```

Or go directly via <http://APP_NAME.herokuapp.com>

View/stream server logs:

```shell
heroku logs --tail
```

## Deploying to [Zeit](https://zeit.co/)

Install the now cli and sign up for a [zeit account](https://zeit.co/docs/v1/getting-started/introduction-to-now/).

Deploying is simply:

```shell
now
```
