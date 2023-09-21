The micro:bit has two buttons, the A button and the B button.

They can be programmed so something happen when only A is pressed, only B is pressed, or when A+B are pressed together.

--- task ---

From the <code style="background-color: #D400D4">Input</code> menu, drag out the <code style="background-color: #D400D4">on button pressed</code>  block.

Place it in the workspace.

<div style="position:relative;height:calc(400px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:50%;height:100%;" src="https://makecode.microbit.org/---codeembed#pub:_P4CDHUfAFEc2" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

This is an event block, you can put other blocks inside of it and they will all run when the event happens. In this case the event is button A being pressed.

--- task ---

From the <code style="background-color: #1E90FF">Basic</code> menu, drag a <code style="background-color: #1E90FF">show string</code> block and place it inside the <code style="background-color: #D400D4">on button pressed</code>  block.

Change the string `Hello` to a message of your choice. We have used `Breathe` in this example.

<div style="position:relative;height:calc(400px + 5em);width:100%;overflow:hidden;"><iframe style="position:relative;top:0;left:0;width:50%;height:100%;" src="https://makecode.microbit.org/---codeembed#pub:_WjPT901f50td" allowfullscreen="allowfullscreen" frameborder="0" sandbox="allow-scripts allow-same-origin"></iframe></div>

--- /task ---

You can add more blocks inside the <code style="background-color: #D400D4">on button pressed</code>  block as needed.

--- task ---

From the <code style="background-color: #E63022">Music</code> menu, drag out a <code style="background-color: #E63022">play melody</code> block.

Place it inside the <code style="background-color: #D400D4">on button pressed</code>  block.
--- /task ---

--- task ---

Test your program - when the simulator restarts, press Button A. Your message will show on the led screen and your melody will play.

--- /task ---

### Adding other buttons

You can have many events in a single program!

--- task ---

Open the <code style="background-color: #D400D4">Input</code> menu and drag another <code style="background-color: #D400D4">on button pressed block</code>  into the Workspace.

--- /task ---

At first the block will be faded out, because you can only have one reaction for each event.

--- task ---

Use the dropdown to change the button for the event to `B` instead.

<img src="images/changebutton-menu.gif" alt="Animation showing the drop down menu on the `on button pressed` block. Button B is chosen and the block is no longer greyed out." width="350"/>

--- /task ---

--- task ---

Add blocks to run when you press Button B.

--- /task ---

--- task ---

Repeat the above steps to add Button A+B to your workspace.

--- /task ---
