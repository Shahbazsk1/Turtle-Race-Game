# Turtle-Race-Game
<h2>To simulate a race between multiple turtles, where the user bets on which turtle will win based on color.<br>
  The turtles move forward by a random distance in each loop iteration until one crosses the finish line.</h2>
<h3>Project Details</h3>
<h4>1.User Interaction</h4>
<ul>
  <li>
    The game begins by showing a prompt to the user asking:<br>
    "Which turtle will win the race? Enter a color:"
  </li>
  <li>
    The user inputs one of the six turtle colors: ["red", "orange", "blue", "green", "yellow", "pink"].
  </li>
</ul>
<h4>
  2. Turtle Setup
  <ul>
    <li>
      Six turtles are created using a loop:
      <ul>
        <li>Each has a unique color from the color list.</li>
        <li>Their starting positions are along the left side of the screen (x = -230) and spaced vertically by different y_positions.</li>
        <li>The turtles are stored in a list all_turtles.</li>
      </ul>
    </li>
  </ul>
</h4>


3. Starting the Race
The race starts only if the user has placed a bet (i.e., input is not empty).

The game loop (while is_race_on) continues until one turtle crosses the finish line (x > 230).

4. Turtle Movement
In each iteration of the loop:

Every turtle moves forward by a random distance between 0 and 10 (inclusive).

As soon as a turtle crosses the finish line:

The race stops (is_race_on = False).

The turtle that wins is identified by its pencolor.

A message is printed indicating whether the user's chosen turtle color won or lost.

5. Game Exit
The game window stays open until the user clicks on it, using:

python
Copy
Edit
screen.exitonclick()
