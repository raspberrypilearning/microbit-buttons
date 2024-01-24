Το micro:bit έχει δύο κουμπιά, το κουμπί A και το κουμπί B.

Μπορούν να προγραμματιστούν έτσι ώστε κάτι να συμβαίνει όταν πατιέται μόνο το Α, όταν πατιέται μόνο το Β ή όταν πατιόνται τα Α+Β μαζί.

Μπορείς να βρεις το μπλοκ `όταν πιεστεί το πλήκτρο button`{:class='microbitinput'} στο μενού `Είσοδος`{:class='microbitinput'}.

<img src="images/input-on-ButtonA.png" alt="Input menu expanded showing the `on button pressed` block highlighted." width="350"/>

Για να χρησιμοποιήσεις το μπλοκ `όταν πιεστεί το πλήκτρο button`{:class='microbitinput'}, σύρε το στον χώρο εργασίας.

```microbit
input.onButtonPressed(Button.A, function () {
	
})
```

Αυτό είναι ένα μπλοκ συμβάντος. Μπορείς να τοποθετήσεις άλλα μπλοκ μέσα σε αυτό και θα τρέξουν όταν συμβεί το συμβάν. Σε αυτήν την περίπτωση, το συμβάν είναι όταν πατηθεί το κουμπί A.

Στο μενού `Βασικά`{:class='microbitbasic'}, μπορείς να βρεις το μπλοκ `εμφάνισε συμβολοσειρά`{:class='microbitbasic'}.

<img src="images/basic-blocks.png" alt="Basic menu expanded showing the `show string` block highlighted." width="350"/>

Τοποθέτησε αυτό το μπλοκ μέσα στο μπλοκ `όταν πιεστεί το πλήκτρο button`{:class='microbitinput'}.

Άλλαξε τη συμβολοσειρά `Hello` σε μήνυμα της επιλογής σου. Έχουμε χρησιμοποιήσει το `Ανάπνευσε` σε αυτό το παράδειγμα.

```microbit
input.onButtonPressed(Button.A, function () {
    basic.showString("Ανάπνευσε")
})
```

Μπορείς να προσθέσεις περισσότερα μπλοκ μέσα στο μπλοκ `όταν πιεστεί το πλήκτρο button`{:class='microbitinput'} αν χρειάζεται.

Δοκίμασε το έργο σου. Όταν ξαναξεκινήσει ο προσομοιωτής, πάτησε το κουμπί A και το μήνυμά σου θα εμφανιστεί στην οθόνη LED.

### Πρόσθεσε κι άλλα κουμπιά

Μπορείς να έχεις πολλά συμβάντα σε ένα μόνο πρόγραμμα!

Άνοιξε το μενού `Είσοδος`{:class='microbitinput'} και σύρε ένα ακόμη μπλοκ `όταν πιεστεί το πλήκτρο button`{:class='microbitinput'} στον χώρο εργασίας.

Στην αρχή, το μπλοκ θα ξεθωριάσει, επειδή μπορείς να έχεις μόνο μία αντίδραση για κάθε συμβάν.

Χρησιμοποίησε το αναπτυσσόμενο μενού για να αλλάξεις το συμβάν σε πάτημα του κουμπιού «Β» αντί για το κουμπί Α.

<img src="images/changebutton-menu.gif" alt="Animation showing the drop-down menu on the `on button pressed` block. Button B is chosen and the block is no longer greyed out." width="350"/>

Το μπλοκ δεν θα είναι ξεθωριασμένο πλέον.

Μπορείς να προσθέσεις τα μπλοκ κώδικα που θέλεις μέσα σε αυτό το μπλοκ κώδικα κουμπιού.

### Χρησιμοποίησε το λογότυπο στο V2

Η έκδοση 2 του micro:bit χρησιμοποιεί επίσης το πάτημα του λογότυπου ως συμβάν.

Στο μενού `Είσοδος`{:class='microbitinput'}, μπορείς επίσης να βρεις το μπλοκ `on logo pressed`{:class='microbitinput'}.

Σύρε το μπλοκ στον χώρο εργασίας. Μπορείς να προσθέσεις κι άλλα μπλοκ κώδικα μέσα σε αυτό το μπλοκ, αν χρειάζεται.

```microbit
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    basic.showIcon(IconNames.Heart)
})
```
