The micro:bit has two buttons, the A button and the B button.

They can be programmed so something happens when only A is pressed, only B is pressed, or when A+B are pressed together.


In the `Input`{:class='microbitinput'} menu, you could find the `on button pressed`{:class='microbitinput'} block.

<img src="images/input-on-ButtonA.png" alt="Input menu expanded showing the `on button pressed` block highlighted." width="350"/>

To use it, drag it onto the workspace.

```microbit
input.onButtonPressed(Button.A, function () {
	
})
```

This is an event block, you can put other blocks inside of it and they will all run when the event happens. In this case the event is button A being pressed.

In the `Basic`{:class='microbitbasic'} menu, you would find a `show string`{:class='microbitbasic'} block.

<img src="images/basic-blocks.png" alt="Basic menu expanded showing the `show icon` block highlighted." width="350"/>


Place it inside the `on button pressed`{:class='microbitinput'} block.

Change the string `Hello` to a message of your choice. We have used `Breathe` in this example.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showString("Hello!")
})
```

You can add more blocks inside the `on button pressed`{:class='microbitinput'} block as needed.

Test your program - when the simulator restarts, press Button A. Your message will show on the led screen.

### Adding other buttons

You can have many events in a single program!

Open the `Input`{:class='microbitinput'} menu, and drag another `on button pressed`{:class='microbitinput'} block into the Workspace.

At first the block will be faded out, because you can only have one reaction for each event.

Use the dropdown to change the button for the event to `B` instead.

<img src="images/changebutton-menu.gif" alt="Animation showing the drop down menu on the `on button pressed` block. Button B is chosen and the block is no longer greyed out." width="350"/>

The block will no longer be faded out.

You can add the needed code blocks inside the button code block.

### Using the logo on V2

The version 2 of the micro:bit also uses events by pressing the logo.

From inside the `Input`{:class='microbitinput'} menu you could also find the `on logo pressed`{:class='microbitinput'} block.

Drag the block onto the workspace. You could add other code blocks inside as needed.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.showIcon(IconNames.Heart)
})
```