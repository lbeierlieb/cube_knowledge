### Weißes Kreuz
- Intuitiv lösen
- Im Anschluss weiße Fläche unten halten

### First Layer (weiße Ecken)
- Eckstein über die richtige Ecke bringen
- Ecke muss auf der vorderen Seite sein, der weiße "Sticker" muss zur Seite weg oder nach oben zeigen
- Falls der Stein rechts ist, dann rechten Sexy-Move: R U R' U'
- Falls der Stein links ist, dann linken Sexy-Move: L' U' L U
- Falls der weiße Sticker nach oben zeigt, dann ist egal ob der Stein rechts oder links ist. Auf der Seite mit den Stein 3x Sexy-Move (Stein ist rechts vorne -> 3x rechter Sexy-Move)

### Second Layer (nicht-gelbe Kanten)
- Nicht-gelbe Kanten oben auf der gelben Seite suchen
- Seitlichen Sticker mit gleichfarbigen Mittelsticker alignen und diese Seite anschauen (grün-rote Kante, rot oben, grün seitlich -> über grünem Mittelstein platzieren und grüne Seite anschauen)
- Prüfen, ob die Kante nach links oder nach rechts eingefügt werden muss
- Kante vom Ziel wegdrehen
- Dazugehörige Ecke hochholen
- Letzte beiden Schritte rückgängig (Kante zurückdrehen, Ecke wieder runter) -> Ecke und Kante sind zu einem Paar zusammengebaut und befinden sich oben
- Paar in den Slot einhämmern
	- erster Hammerschlag (Vorderseite) bringt das Paar an die gewüschte Position
	- zweiter Hammerschlag (Seite)
	- erster Hammer wieder nach oben
	- zweiter Hammer wieder nach oben

### Gelbe Seite: Kanten
- Es können drei Fälle auftreten, die jeweils unterschiedlich gehalten werden müssen
	- Dot (keine Kante gelb), egal wie gehalten wird
	- Corner (zwei Kanten "nebeneinander" gelb), muss hinten links sein
	- Bar (zwei Kanten gegenüber gelb), muss waagerecht gehalten werden
- Algorithmus (F R U R' U'):
	- Front öffnen (im Uhrzeigersinn drehen)
	- Sexy-Move
	- Front schließen
- Ausrichtung und Algorithmus solange wiederholen bis alle Kanten gelb sind

### Gelbe Seite: Ecken
- Es können sieben Fälle auftreten, die folgendermaßen aussehen und gehalten werden müssen
	- Cross (keine Kanten oben sind gelb)
		- Zwei Headlights-Paare: eines der Headlights muss nach links zeigen
		- 1x Headlights: müssen nach links zeigen
	- Space-Invader (zwei nebeneinanderliegende Ecken sind gelb)
		- Headlights: müssen nach vorne schauen
		- keine Headlights: Space-Invader (also seine "freie" Kante) muss nach links schauen
	- L-Case (zwei diagonal gegenüberliegende Ecken sind gelb)
		- die beiden seitlichen gelben Sticker müssen nach vorne und nach rechts schauen
	- Fisch (eine Ecke gelb)
		- Fischkopf und Fischfutter müssen auf der Vorderseite sein
		- Fischfutter rechts -> rechter Fisch, Fischfutter links -> linker Fisch
- Algorithmus (R U R' U  R U2 R') es arbeitet nur die rechte Hand
	- Erste drei Moves wie Sexy-Move