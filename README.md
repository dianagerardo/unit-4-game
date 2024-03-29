# unit-4-game
### Before You Begin

1. Create a new GitHub repo called `unit-4-game`, then clone it to your computer.

2. Inside the `unit-4-game` folder, create an `index.html` file.

3. Still inside the `unit-4-game` directory, make a folder called `assets`.
* Inside the `assets` directory, make three additional folders: `javascript`, `css` and `images`.
* In the `javascript` folder, make a file called `game.js`.
* In the `css` folder, make a file called `style.css`.
* In the `css` folder, make a file called `reset.css`. Paste into it the code found from the Meyerweb Reset.
* In the images folder, save any of the images you plan on using.

4. Set up your repository to deploy to Github Pages.

5. Push the above changes to GitHub. 

6. Choose whichever game you want to make from the choices below. The CrystalsCollector game is the recommended option, but if you are looking for an extra hard challenge then take a stab at the Star Wars exercise. (Note: Only choose the Star Wars Exercise if you are feeling very comfortable with the material covered in class. The Crystal Collector activity is plenty challenging enough!).

### Option One: CrystalsCollector Game (Recommended)

![Crystal Collector](Images/1-CrystalCollector.jpg)

1. [Watch the demo](https://youtu.be/yNI0l2FMeCk).

2. The player will have to guess the answer, just like in Word Guess. This time, though, the player will guess with numbers instead of letters. 

3. Here's how the app works:

* There will be four crystals displayed as buttons on the page.

* The player will be shown a random number at the start of the game.

* When the player clicks on a crystal, it will add a specific amount of points to the player's total score. 

* Your game will hide this amount until the player clicks a crystal.
* When they do click one, update the player's score counter.

* The player wins if their total score matches the random number from the beginning of the game.

* The player loses if their score goes above the random number.

* The game restarts whenever the player wins or loses.

* When the game begins again, the player should see a new random number. Also, all the crystals will have four new hidden values. Of course, the user's score (and score counter) will reset to zero.

* The app should show the number of games the player wins and loses. To that end, do not refresh the page as a means to restart the game.

##### Option 1 Game design notes

* The random number shown at the start of the game should be between 19 - 120.

* Each crystal should have a random hidden value between 1 - 12.

##### Option 1 Game Coding Notes
The app should keep a track of the wins and losses without resetting or changing when the page is refreshed-

1. Generate a random number for both the number to guess and the crystal's value. The value of the crystal will be hidden.
//Math.floor((Math.random() * 120) + 19)

2. When player clicks on crystal add points to the total score
//$("#crystal").click(function (){}
// score = score + valueofcrystal

3. Compare the score to the number to guess
//function compareScores() {}

4. If scores match:
//if (crystalGame.scoreCounter === crystalGame.computerGuess) {}
then:
a. Update wins:
//crystalGame.wins++

//else if (crystalGame.scoreCounter > crystalGame.computerGuess) {}
b. Update losses:
crystalGame.loss++




