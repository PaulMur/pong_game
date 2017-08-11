# A Super simple Ping Pong game

This is a super simple Ping Pong game using the HTML5 Canvas and JavaScript, There is a multiplayer version and a single player version.

```
    To control the single player game simply use the mouse movement on screen

    To control the multiplayer game one player must use 'W' and 'S' to move and the other player must use '↑' and '↓'
```

There are simple code pieces which will allow you to change settings such as speed and placement.

``` Javascript
    var ballX = 50;
    var ballY = 50;
    var ballSpeedX = 15;
    var ballspeedY = 7;

    var player1Score = 0;
    var player2Score = 0;
    const WINNING_SCORE = 3;

    var showingWinScreen = false;

    var paddle1Y = 250;
    var paddle2Y = 250;
    const PADDLE_HEIGHT = 100;
    const PADDLE_WIDTH = 15;
```

The Constands are items of fixed value from the start such as WINNING_SCORE which controls how many points are needed to win and PADDLE dimensions.

In the onload function is where the game is run and how it is controlled, You can see a simple frames per second monitor which allows you to set the FPS of the game

``` Javascript
    var framesPerSecond = 30;
    setInterval(function() {
        moveEverything();
        drawEverything();
    }, 1000/framesPerSecond);
```

Hav fun! This repo is open to improvements.