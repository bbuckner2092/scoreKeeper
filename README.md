In the #scorekeeper we will make a game that will consist of 2 players.
Objective: to get to the specified number first.
How to set up this game:
1) Created a html and js file.
2) Built the boilerplate in addition to adding a script tag to connect the 2 files.
3) Gave each button an id so that we could reference it in our js logic.
4) Used two vars to specify the different <buttons> that would have an .addEventListener.

5) Used a <span> tag in the HTML so that way when the player "clicks" the button the entire h1 would NOT change, just the 0.  We also included an id so we could "select" it in our logic.

6) Inside our p1Button, we added p1Score++ so it will increment by 1 each time the button is pressed.  Immediately, we made the p1Display = p1Score so that way as the score is increased so is the text in our HTML.