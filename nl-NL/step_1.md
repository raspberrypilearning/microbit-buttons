De micro:bit heeft twee knoppen, de A knop en de B knop.

Je kunt iets programmeren als alleen A wordt ingedrukt, alleen B wordt ingedrukt, of wanneer A+B samen worden ingedrukt.

Je kunt het blok `wanneer knop wordt ingedrukt`{:class='microbitinput'} vinden in het `Invoer`{:class='microbitinput'} menu.

<img src="images/input-on-ButtonA.png" alt="Input menu expanded showing the `on button pressed` block highlighted." width="350"/>

Om het `wanneer knop wordt ingedrukt`{:class='microbitinput'} blok te gebruiken, sleep je het naar het bewerkingspaneel.

```microbit
input.onButtonPressed(Button.A, function () {
	
})
```

Dit is een gebeurtenisblok. Je kunt andere blokken erin zetten en ze worden uitgevoerd wanneer de gebeurtenis plaatsvindt. In dit geval is de gebeurtenis het indrukken van knop A.

In het `Basis`{:class='microbitbasic'} menu vind je het `toon tekens`{:class='microbitbasic'} blok.

<img src="images/basic-blocks.png" alt="Basic menu expanded showing the `show string` block highlighted." width="350"/>

Plaats het in het `wanneer knop wordt ingedrukt`{:class='microbitinput'} blok.

Verander de string `Hello` naar een bericht van jouw keuze. We hebben in dit voorbeeld `Ademen`` gebruikt.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showString("Ademen")
})
```

Je kunt zo nodig meer blokken toevoegen in het blok `wanneer knop wordt ingedrukt`{:class='microbitinput'}.

Test je programma. Wanneer de simulator opnieuw opstart, druk je op knop A en je bericht wordt op het LED-scherm getoond.

### Andere knoppen toevoegen

Je kunt veel gebeurtenissen in één programma hebben!

Open het `Invoer`{:class='microbitinput'} menu en sleep een ander `wanneer knop wordt ingedrukt`{:class='microbitinput'} blok in het bewerkingspaneel.

In eerste instantie wordt het blok grijs van kleur, omdat je per gebeurtenis slechts één reactie kunt hebben.

Gebruik het vervolgkeuzemenu om de gebeurtenis te wijzigen in het indrukken van knop 'B' in plaats van knop A.

<img src="images/changebutton-menu.gif" alt="Animation showing the drop-down menu on the `on button pressed` block. Button B is chosen and the block is no longer greyed out." width="350"/>

Het blok krijgt weer de normale kleur.

Je kunt de gewenste codeblokken toevoegen binnen dit nieuwe knop-codeblok.

### Gebruik het logo op V2

Versie 2 van de micro:bit gebruikt ook het indrukken van het logo als gebeurtenis.

In het `Invoer`{:class='microbitinput'} menu kun je ook het `bij logo ingedrukt`{:class='microbitinput'} blok vinden.

Sleep het blok naar het bewerkingspaneel. Indien nodig kun je andere codeblokken binnen dit blok toevoegen.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.showIcon(IconNames.Heart)
})
```
