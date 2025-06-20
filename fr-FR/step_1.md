Le micro:bit possède deux boutons, le bouton A et le bouton B.

Ils peuvent être programmés de sorte que quelque chose se produit lorsque seulement A est pressé, seulement B est pressé, ou lorsque A+B est pressé ensemble.

Tu peux trouver le bloc `lorsque le bouton est pressé`{:class='microbitinput'} dans le menu `Entrée`{:class='microbitinput'}.

<img src="images/input-on-ButtonA.png" alt="Input menu expanded showing the `on button pressed` block highlighted." width="350"/>

Pour utiliser le bloc `lorsque le bouton est pressé`{:class='microbitinput'}, fais-le glisser sur l'espace de travail.

```microbit
input.onButtonPressed(Button.A, function () {
	
})
```

Ceci est un bloc événement. Tu peux mettre d'autres blocs à l'intérieur et ils s'exécuteront quand l'événement se produit. Dans ce cas, l'événement est le bouton A pressé.

Dans le menu `Base`{:class='microbitbasic'}, tu peux trouver le bloc `afficher texte`{:class='microbitbasic'}.

<img src="images/basic-blocks.png" alt="Basic menu expanded showing the `show string` block highlighted." width="350"/>

Place ce bloc à l'intérieur du bloc `lorsque le bouton est pressé`{:class='microbitinput'}.

Remplace le texte `Hello` par un message de ton choix. Nous avons utilisé `Respire` dans cet exemple.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showString("Breathe")
})
```

Tu peux ajouter plus de blocs à l'intérieur du bloc `lorsque le bouton est pressé`{:class='microbitinput'} si nécessaire.

Teste ton programme. Lorsque le simulateur redémarre, appuie sur le bouton A et ton message s'affichera sur l'écran LED.

### Ajouter d'autres boutons

Tu peux avoir beaucoup d'événements dans un seul programme !

Ouvre le menu `Entrée`{:class='microbitinput'}, et fais glisser un autre bloc `lorsque le bouton est pressé`{:class='microbitinput'} dans l'espace de travail.

Au début, le bloc sera estompé, car tu ne peux avoir qu'une seule réaction pour chaque événement.

Utilise le menu déroulant pour modifier l'événement en appuyant sur le bouton `B` au lieu du bouton A.

<img src="images/changebutton-menu.gif" alt="Animation showing the drop-down menu on the `on button pressed` block. Button B is chosen and the block is no longer greyed out." width="350"/>

Le bloc ne sera plus estompé.

Tu peux ajouter les blocs de code que tu souhaites à l'intérieur de ce nouveau bloc de code de bouton.

### Utiliser le logo sur la V2

La version 2 du micro:bit utilise également la pression sur le logo comme un événement.

Dans le menu `Entrée`{:class='microbitinput'}, tu peux également trouver le bloc `sur le logo appuyé`{:class='microbitinput'}.

Fais glisser le bloc dans l'espace de travail. Tu peux ajouter d'autres blocs de code à l'intérieur de ce bloc si nécessaire.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.showIcon(IconNames.Heart)
})
```
