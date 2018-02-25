In the #scorekeeper we will make a game that will consist of 2 players.
Objective: to get to the specified number first.
How to set up this game:
1) Created a html and js file.
2) Built the boilerplate in addition to adding a script tag to connect the 2 files.
3) Gave each button an id so that we could reference it in our js logic.
4) Used two vars to specify the different <buttons> that would have an .addEventListener.

5) Used a <span> tag in the HTML so that way when the player "clicks" the button the entire h1 would NOT change, just the 0.  We also included an id so we could "select" it in our logic.

6) Inside our p1Button, we added p1Score++ so it will increment by 1 each time the button is pressed.  Immediately, we made the p1Display = p1Score so that way as the score is increased so is the text in our HTML.

7) Followed the same steps from step 6, but we made sure to use the vars for p2 instead.

8) Added a var gameOver that keeps track of our game state. Once we have reached our specified number then neither player should be able to update their score.
    We set the gameOver var to false because at the very start of the game gameOver is NOT true!
    We included an if statement in order to change the "states" of the game. Simply put, if !gameOver then we simply add 1 to the player score.  If the pScore === winningScore then the player is UNABLE to update his score any further, and gameOver = true;

9) Added the css file in addition to a link tag in the head to connect the css stylesheet to the html file.
    Created a class called .winner that has the color green.

10) Included .classList.add("winner"); to both the p1Score === winningScore and p2Score === winningScore so that the color of the text will change once that player has reached the specified number.

11) Added an eventListener on the resetButton.
    OnClick, the p1 and p2Scores return to 0, the p1 and p2Display.textContent return to 0, and made gameOver = false; so that way we can continue to play after the reset button is clicked.

12) Created 2 new vars, numInput and winningScoreDisplay.
    numInput consist of the actual "input value" that the user can manipulate.

    winningScoreDisplay consist of the textContent that will be "displayed" when the usere "changes" the winning Score".  Instead of using an # we were able to simply use "p span" since there was only 1 paragraph with a span in it.

13) Created a reset(); that consisted of all of the code from our resetButton.  
    Placed this new reset function inside of the resetButton and the numInput so that way we could DRY up our code and make sure that the game will continue to reset when the value is changed.