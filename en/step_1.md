The micro:bit has two buttons, button A and button B.

They can be programmed so something happens when only A is pressed, only B is pressed, or when A+B are pressed together.

You can find the `on button pressed`{:class='microbitinput'} block in the `Input`{:class='microbitinput'} menu.

<img src="images/input-on-ButtonA.png" alt="Input menu expanded showing the `on button pressed` block highlighted." width="350"/>

To use the `on button pressed`{:class='microbitinput'} block, drag it onto the workspace.

```microbit
input.onButtonPressed(Button.A, function () {
	
})
```

This is an event block. You can put other blocks inside of it and they will run when the event happens. In this case, the event is button A being pressed.

In the `Basic`{:class='microbitbasic'} menu, you can find the `show string`{:class='microbitbasic'} block.

<img src="images/basic-blocks.png" alt="Basic menu expanded showing the `show icon` block highlighted." width="350"/>


Place this block inside the `on button pressed`{:class='microbitinput'} block.

Change the string `Hello` to a message of your choice. We have used `Breathe` in this example.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showString("Breathe")
})
```

You can add more blocks inside the `on button pressed`{:class='microbitinput'} block as needed.

Test your program. When the simulator restarts, press button A and your message will show on the LED screen.

### Add other buttons

You can have many events in a single program!

Open the `Input`{:class='microbitinput'} menu, and drag another `on button pressed`{:class='microbitinput'} block into the workspace.

At first, the block will be faded out, because you can only have one reaction for each event.

Use the drop-down menu to change the event to button `B` being pressed instead of button A.

<img src="images/changebutton-menu.gif" alt="Animation showing the drop-down menu on the `on button pressed` block. Button B is chosen and the block is no longer greyed out." width="350"/>

The block will no longer be faded out.

You can add your desired code blocks inside this button code block.

### Use the logo on V2

Version 2 of the micro:bit also uses pressing the logo as an event.

In the `Input`{:class='microbitinput'} menu, you can also find the `on logo pressed`{:class='microbitinput'} block.

Drag the block into the workspace. You can add other code blocks inside this block as needed.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.showIcon(IconNames.Heart)
})
```
