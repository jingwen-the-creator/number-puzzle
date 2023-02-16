# Meeting Log

This is an informal meeting log we kept for our meetings. The more formal description of our sprints is included in the file [sprint-log.pdf](sprint-log.pdf).

## Meeting Feb 17

### Requirements

- Spring Boot setup

- cs5031.practical2.gameService
  + Make multiple levels: Easy (4 char), Medium (6 char), ...

- REST API / Back-end
  + Endpoints/Routes
  + API Schema
  + Data Structures
    + class: GameState
      + class: Guess (1..6)
      + class: Solution (1)
    + class: EquationParser
    + class: EquationGenerator

- GUI / Front-end
  + JavaScript / Vue.js
  + Representation of the guesses
  + Maybe: Keyboard
  + API client
  
### Questions

- Can we do the different levels?

### Todo until next meeting

- nothing

## Meeting Feb 18

Notes on implementation: https://www.notion.so/P2-c26f968881c148babeec1cf40741f2a2

### Work packages

#### Equation stuff

- EquationParser (priority 2) => P
- EquationGenerator (priority 1) => P
- GuessChecker (priority 3) => J

#### cs5031.practical2.gameService stuff

- GameState => L
- GameStateStore => L

#### REST API stuff

- RestAPI => J

#### GUI stuff

- Vue.js front-end => L
- Calls to the API => L

#### Possible extension

- Store the game states in a database

### Todo until next meeting

- Leo works on front end to make first prototype
- Jingwen works on the REST API + GuessChecker
- Pavalli works on EquationGenerator + EquationParser

> Next meeting: Feb 21 (Monday)

## Meeting Feb 21

Quick meeting to catch up on what we did

## Meeting Feb 22

- Merge branches together
- Agreed on SessionData interface
- Discussed flow of the game

### Todo until next meeting

- Pallavi will finish EquationParser, EquationGenerator & write unit tests
- Jingwen will finish SessionController (& unit tests)
- Leo will finish GameController (& unit tests)

> Next meeting: Feb 25 (Friday) to catch up

## Meeting Feb 25

- Discussed progress
- Jingwen implemented SessionController and proper HTTP Sessions
- Pallavi finished EquationParser and Generator and worked on unit tests
- Leo implemented GameController, HintGenerator and unit tests

### Todo until next meeting

- Unit tests
- Refactoring
- Start integration of client and server

> Next meeting: Mar 1 (Tuesday)

## Meeting Mar 1 (Addendum Mar 3)

- Pallavi presented EquationGenerator and EquationParser
  + basic functionality works flawlessly
  + should maybe make some changes to get rid of the tendency to produce large numbers in the EquationGenerator
  + left todo: unit tests, refactoring, catch exceptions
- Jingwen presented PlayerController
  + PlayerController can create new game, get existing game, and switch games
  + Everything works as required
  + left todo: some more unit tests
- Leo presented GameController
  + GameController can process submitted guesses
  + had to make change to work flow to match what we discussed before
  + everything else works as required
  + left todo: more unit tests

### Todo until next meeting

- Cover the left todos mentioned above
- Leo: client-server integration
- Jingwen: move from non-persistent to persistent storage (MongoDB)
- Pallavi: refactoring and unit testing

> Next meeting: Mar 4 (Friday)

## Meeting Mar 4
- Finished first working release
- Discussed unit tests
- Found bug that rarely generates invalid equations (in this case the equation width was set 4)

### Todo until next meeting
- Pallavi:
  + Exception handling
  + Comments, docstrings
- Leo + Jingwen:
  + DataMongoTest
- General:
  + CI/CD

## Meeting Mar 6
- Implemented tests for mongo database
- implemented swagger UI
- implemented more unit tests for client
- CI/CD

### Todo until LAST meeting (7 Mar)
- Comments, docstrings for EquationParser and EquationGenerator (Pallavi)
- Fix remaining failing tests
- Layout Sprint meeting Log
- CI/CD fix server test

## Meeting Mar 7
- Fixed a new bug we found in the EquationGenerator
- Final fixes
- Write README

### LEFT TODO: SUBMISSION
