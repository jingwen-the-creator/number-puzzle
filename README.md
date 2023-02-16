# CS5031 - P2 - Numble

## Table of Contents

+ [Logs](#logs)
+ [Build & run the project](#building-and-running-the-project)
+ [Playing the game](#playing-the-game)

---

## Logs

The formal Sprint log can be found in the [sprint-log.pdf](sprint-log.pdf). We also kept a more informal meeting log in the file [Meeting-Log.md](Meeting-Log.md).

## Building and running the project

### Setup

The code consists of a separate (Java Spring) server and 
(Vue.js) client. For convenience, we provide two shell
scripts to build and run each.

To build and run the server, run

```bash
./server.sh
```

and to build and run the client, run

```bash
./client.sh
```

### Accessing the server & API documentation

The client exposes the API on `localhost:8081`.
We added Swagger UI to the project, so head to
`localhost:8081/swagger-ui/index.html` to explore
the API. 

You can also get the OpenAPI specification from
`localhost:8081/api-docs`. 

A PDF version of the API documentation (generated with [SwDoc](https://www.swdoc.org/))
which can be found in the [doc directory](doc/api-doc.pdf).

### Accessing the client

The node server of the client runs on `localhost:8080`.
While you can use the API via the command line with
`curl`, the client provides a much better experience.

## Playing the game

> This is a demo for the Vue.js client. 
> If you do want to play the game from the command line
> using curl, we recommend heading to the Swagger UI
> of the application (`localhost:8081/swagger-ui/index.html`)
> to generate the curl commands for convenience!

Playing the game is pretty straightforward. Head to 
`localhost:8080` and start a new game. We strongly
recommend EASY!!

![Login page](doc/images/login.png)

Here's a short demo on how to play the game:

![New game demo](doc/images/client-demo1.gif)

You can also go back to an existing game (finished or not)
using the Game ID (displayed in game above the board).

Here's a demo for that:

![Getting a game demo](doc/images/client-demo2.gif)

For everything else, click the `Help` button at the top 
of the page to learn more about the rules and the game.

