# Turtle-Race-Game
<h2>To simulate a race between multiple turtles, where the user bets on which turtle will win based on color.<br>
  The turtles move forward by a random distance in each loop iteration until one crosses the finish line.</h2>
<h3>Project Details</h3>
<h4>1.User Interaction</h4>
<ul>
  <li>
    The game begins by showing a prompt to the user asking:<br>
    <p>"Which turtle will win the race? Enter a color:"</p>
  </li>
  <li>
    The user inputs one of the six turtle colors: ["red", "orange", "blue", "green", "yellow", "pink"].
  </li>
</ul>
<h4>2. Turtle Setup</h4>
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
<h4>3. Starting the Race</h4>
<ul>
  <li>The race starts only if the user has placed a bet (i.e., input is not empty).</li>
  <li>The game loop (while is_race_on) continues until one turtle crosses the finish line (x > 230).</li>
</ul>
<h4>4. Turtle Movement</h4>
<ul>
  <li>In each iteration of the loop:
    <ul>
      <li>Every turtle moves forward by a random distance between 0 and 10 (inclusive).</li>
      <li>
        As soon as a turtle crosses the finish line:
        <ul>
          <li>The race stops (is_race_on = False).</li>
          <li>The turtle that wins is identified by its pencolor.</li>
          <li>A message is printed indicating whether the user's chosen turtle color won or lost.</li>
        </ul>
      </li>
    </ul>
  </li>
</ul>
<h4>5. Game Exit</h4>
<ul>
  <li>The game window stays open until the user clicks on it, using:
  <p>screen.exitonclick()</p>
  </li>
</ul>

<h3>Modules Used</h3>
<h4>1. turtle (standard Python module)</h4>
<ul>
  <li>Used for drawing and animating the turtle shapes on screen.</li>
  <li>Key functions and classes used:
  <ul>
    <li>Turtle(): creates turtle objects.</li>
    <li>Screen(): controls the graphics window.</li>
    <li>screen.setup(width, height): sets window size.</li>
    <li>turtle.shape("turtle"): sets turtle shape.</li>
    <li>turtle.color(): sets turtle color.</li>
    <li>turtle.penup(): lifts pen so it doesn’t draw lines.</li>
    <li>turtle.goto(x, y): positions the turtle.</li>
    <li>turtle.forward(distance): moves turtle forward.</li>
    <li>turtle.xcor(): gets turtle’s x-coordinate.</li>
    <li>screen.textinput(title, prompt): gets input from user.</li>
    <li>screen.exitonclick(): keeps window open until clicked.</li>
  </ul> 
  </li>
</ul>
<h4>2. random (standard Python module)</h4>
<ul>
  <li>Used for generating a random movement distance for each turtle on every loop iteration.</li>
  <li>Function used:
    <ul>
      <li>random.randint(0, 10): returns a random integer between 0 and 10 inclusive.</li>
    </ul>
  </li>
</ul>
