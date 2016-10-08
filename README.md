# HACK UMASS

# PickApp

## Pitch



## Requirements

* Features
	* connect people
	* create pickup games
	* create teams based on match making
	* create pickup leagues
	* track your fitbit stats for the games you play - *potential feature*
	* rating your teammates and teams you play against
		* helps create a better enviornment
		* helps to match, or not match, players together based off of compatibilty
		* keeps people a little more responsible
* Match Making
	* Inputs
		* interest level
		* sport
		* location
			* get through user input
			* get through auto locate
		* skill level
		* team size (3v3, 5v5, etc)
		* age
		* availablity
* Invite Team Members
* UI/UX
	* simple
		* easy to use
		* intuitive
	* need an account
		* name
		* username
		* password
		* profile
			* interest levels in various sports
			* skill level
			* age
			* availablity
			* average rating
			* past performance
				* teams played on
				* leagues played in
	* rating system
		* 1-5 scale
		* sportsmanship
		* recommend
		* would play again		

## Technologies

* Frameworks
	* Front-End
		* React Native
		* React
	* Backend
		* MongoDB for database
		* Sails
* Change Management
	* Github

## Models

* **User**
	* email
	* password
	* name
	* userprofile
* **UserProfile**
	* user
	* interest
		* sport
		* rating from 0 - 5
	* skill
		* sport
		* rating from 0 - 5
	* age
	* availablity
		* day
		* times: array of arrays (i.e. [[13,15],[16,20]])
	* rating
	* teams
		* users
		* rating
		* date
	* leagues
* **Team**
	* users
	* ratings
	* average rating
* **Game**
	* team
	* datestamp

## Ideas
* Automated Calendar
* Pick App
	* Connects you with people in your area to form teams
	* Helps create pickup games
		* finds X other players around you
		* creates an X vs X game
	* Helps you create leagues

## Brainstorming Session

### Pick app

Pick app is a new and innovative way to connect you with other people in your area to play pickup games.

* Tinder??
	* set a radius (maybe 50 mi or something)
	* automatically grabs your area
	* could overwrite which area
* Match Making?
	* inputs
		* interest level
		* skill level (only partially considered)
		* location
		* age
		* team size (3v3, 5v5, etc)
		* what type of sport you want to play
		* available times
* Leagues?
	* place you based on match making (for the whole team)
	* pick your distribution (tiers of wins/losses)
	* logistics
		* captains of teams
		* min # of teams (maybe 2?)
		* captain can choose teammates
* Program Language?
	* maybe React Native?