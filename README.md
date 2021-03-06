istim-games
============
[![Build Status](https://travis-ci.org/istim/istim-games.png?branch=master)](https://travis-ci.org/istim/istim-games)

Game manager API for the Istim Gaming Platform.
 
 
 
## Services
### Games
  - Publish game
    - ```POST to game/create```
  - Edit game info
     - ```PUT to game/:id```
  - Remove game
    - ```DELETE to game/:id```
  - Like a game
    - ```POST to game/:id/like```
  - Get all available games
    - ```GET to game/```
  - Get a  game
    - ```GET to game/:id```
 
### Achievements
  - Create achievements for a game
    - ```POST to achievement/create```
  - Edit achievements info
    - ```PUT to achievement/:id```
  - Remove achievement
    - ```DELETE to achievement/:id```
  - Get available achievements for a specific game
    - ```GET to game/:id/achievements```
  - Get all available achievements
    - ```GET to achievement/```
  - Get a  achievment
    - ```GET to achievement/:id```
 
## Dependencies
### User API
  - Authentication
  

## Examples of game and achievement

``` 

   var game = {
    name: 'Joguim dos Leleks - Lesk\'s Origin',
    description: 'Joguim dos Leleks, a origem das lelekagens',
    releaseDate: new Date(),
    publisher: 1,
    likes: 0,
    id: 1,
    systemRequirements: "Um PC da Xuxa"
  };
``` 
``` 
  var achievement = {
    title: 'Let\'s Lek',
    decription: 'Domine o poder da zuera',
    icon: 'http://imgsapp.oimparcial.com.br/app/noticia_130321921166/2013/02/15/129893/20130215154254551863i.jpg',
    game: 5,
    id: 1
  }

```
