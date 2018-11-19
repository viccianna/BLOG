# BLOG

Ein Blog über unser programmiertes Spiel auf Snap! (The Beauty and Joy of Computing)

[1. Einleitung](#1)

[2. Die Geschichte des Spiels](#2)

[3. Das Spiel](#3)

## <a name="1"></a> Einleitung 
Willkommen auf unserem 2. Blog über unser Spiel. Hier erklären wir alles rund um unser Spiel, wie es funktioniert und auch wie wir mit Problemen umgegangen sind und sie gelöst haben. Dazu haben wir auch Bilder, um alles verständlicher zu machen und damit ihr auch ein Bild vor Augen habt.

Viel Spaß beim lesen!

Als kleine Einführung:
In unserem Spiel gibt es das Flugzeug, einen Meteor und einen Strich. Zu Anfang des Spiel interargiert man mit dem Flugzeug, welcher den Spieler also als Begleiter zur Seite steht. Es fragt den Spieler, ob er mit auf eine Mission möchte. Danach fliegt man mit ihm zu einem fremden Planeten. Hier beginnt dann das eigentliche Spiel. Das Ziel ist es, den Meteor mithilfe des Striches davon abzuhalten, den Boden zu berühren. Dies macht der Spieler indem er den Strich mit der Maus lenkt. Um das Spiel auch  etwas spannend zu machen, verkleinert sich der Strich nach einer gewissen Zeit. Folgenderweise gibt es also 2 Szenarios, wi e das Spiel ausgehen kann. Entweder ist das Spiel gewonnen wenn der Meteor den Boden nicht beruhrt hat bis die Zeit abgelaufen ist oder das Spiel ist verloren sobald der eben genannte Fall doch zutreffen sollte. Je anchdem ob man gewinnt oder verliert hat man als Spieler die Welt geretten oder auch nicht. Und darin liegt die Intention des Spiels, darin verschieden Welten zu retten.

Soviel zum Hintergrund des Spiel, jetzt erklären wir euch das Spiel!

## <a name="2"></a> Die Geschichte des Spiels
Auf dem ersten Bild hier sind die Gesamten Befehle des Flugzeugs zu sehen. (Welche Befehle für die einzelnen Szenen zuständig sind, sind rot eingekreist.)

Der Befehl "Wenn *Fahne* angeklickt" bedeutet, dass wenn man das Symbol (oben rechts) anklickt, beginnt das Spiel uns somit alle Befehle. das bedeutet für den ersten Hintergrund (Erde), dass dieser jetzt auftauchen soll. Der Darauffolgende bedeutet, das das Kostüm "airplane1" angezogen wird. "Airplane1" steht für das Flugzeug und der Kasten "setzte Größe auf 50%" bedeutet, dass das Kostüm auf eine andere Größe gesetzte werden aknn und in unserem Fall war das Flugzeug zu groß. Daher haben wir es sozusagen kleiner auftauchen lassen. Das die genannten Befehle in einem lilanen Kasten sind heißt nichts anderes als das sie zu der Kategorie Aussehen gehören. (Es gitb ganz links auf der Projektseite eine Liste mit verschiedenen Kategorien: Bewegung, Aussehen, KLang, Stift, Steuerung, Fühlen, Operatoren und Variabeln. Zu diesen genannten Themen gibt es eine Reihe von Befehlen die man auswählen kann.) Als nächsten Befehl hat das Flugzeug 3 blaue Befehle. Diese gehören zur Bewegung. Diese geben die Ausrichtung und Koordinaten an. Der letzte Befehl der Szene ist hier in hellbalu zu sehen. In den Kasten kann man eine Frage reinschreiben und wir haben uns für "Hallo! Mein name ist Flugzeug! Wie heißt du kleiner Astronaut?" entschieden. Durch das aktivieren von "Antwort" im Zusammenhang mit dem Fragebefehl, kann der Spieler nun antworten.

![bsp stride](flugzeugbefehl1.png)

Nachdem der Spieler geantwortet hat, fragt das Flugzeug "Hast du Lust mit auf eine Mission mitzukommen um die Welten zu retten?" und auch darauf kann der Spieler antworten. Danach folgt von dem Kostüm die Nachricht, dass es jetzt los geht.

![bsp stride](flugzeugbefehl12.png)


Durch den folgenden Befehl aus dem Themenbereich Steuerung "Wiederhole 50 Mal" werden die in dem Befehl enthaltenen Befehle in diesem Fall 50 Mal wiederholt. Die in dem eben gennaten Befehl enthaltenen Befehle bedeuten, dass das Flugzeug erst ein paar Schritte geht, sich dann um ein paar Grad (15°) dreht und dann erneut ein paar Schritte geht. Zusammengesetzt und in Ausführung sieht es dann schließlich so aus, dass das Flugzeug um den Planenten fliegt und dies 2 Mal. Zum Schluss sagt der Befehl "gehe zu X=200 Y=200", dass das Kostüm aus dem Bild fliegt.

![bsp stride](flugzeugbefehl3-2.png)

Der nächste Befehl "sende *Bühnenwechsel* an alle" bedeutet, dass einen Nachricht an alle anderen Kostüme sowie Hintergründe gesendet wird. Dadurch können die verschiedenen Sprites kommunizieren. Diese Nachricht wird in unserem Fall an den Hintergrund gesendet. Mit dem Befehl "Wenn ich ... empfange" führt er die ihmgehörigen Befehle erst dann aus, sobald er die Nachricht bekommt. Danach soll das Flugzeug eine Sekunde warten und schließlich in "Richtung 90" zeigen und zu den Koordinaten X:10 Y:-70 gehen. Das letzte was das Flugzeug in dieser Szene zu dem Spieler sagt ist "So, hier beginnt unsere erste Mission. Wir werden uns gleich diesen noch unbekannten Planeten mal näher anschauen, was meinst du?". Nachdem man geantwortet hat kommt erneut der Befehl "Wiederhole (10 Mal)". Dieser Befehl beinhaltet diesmal die Drehung um 15°, die Änderung der Größe um -5 und das Gehen von 10 Schritten. zusammengesetzt sieht das im Spiel so als, als würde das Flugzeug auf den Planeten zufliegen und dann verschwinden.

![bsp stride](flugzeugbefehl4.png)

## <a name="3"></a> Das Spiel
Nachdem das Flugzeug dann auf den Planent zufliegt und dort verschwindet, findet sich der Spieler auf dem fremden Planeten wieder. Als nächstes beginnt dann schon das "richtige" Spiel. Dieses Szenario besteht aus dem ersten Strich (rot) und dem Meteor "Metheory". ZUnächst bewegt sich der Meteor auf die Mitte der Bildschirms zu und fängt dann an sich zufällig durch den Raum zu bewegen.

![bsp stride](meteor-2.png)

Auf den oberen Bild sind die aktiven Befehle, also die die in diesem Moment aktiv sind, wieder markiert. Diese beziehen sich hier auf den Metheor. Das untere Bild zeigt die Befehle die auf den ersten Strich zutreffen. 

![bsp stride](strichrot.png)

Wie schon oben gesagt, besteht nun der Sinn des Spiels darin, den Meteor davon abzuhalten aud den Boden zu kommen. Um also dies zu bewerkstelligen habe wir die Befehle links oben auf dem Bild. Dieser setzt sich aus dem Befehl "wenn ich *strich1* empfange", "anzeigen", "ziehe Kostüm *strich1* an", "gehe zu X=30 Y=-130", "sende *jetzt* an alle", "wiederhole bis *berühre?*" und "setzte X auf *Maus X Position*" zusammen. Das "Anzeigen" muss dort sein da wir mit dem Befehl "Wenn *Fahne* angeklickt" die Sprite erstmal versteckt haben. Dies haben wir gemacht, damit der Strich erst auftaucht, wenn sie die Nachricht bekommt. Nachdem Sie dann also zu sehen ist, soll sie zu den oben genannten Koordinaten gehen und eine Nachricht an alle schicken. Den Befehl sendet sie aber im Prinzip an sich selber, was man auf dem Befehlblock rechts auf dem Bild sehen kann. Auf die Nachricht folgend hat sie dann den Befehl, etwas Bestimmtes auszuführen und dass ist der X Koordinate der Maus zu folgen. Mit den Koordinaten und dem folgen der Maus, bewegt sich der Strich also auf einer Linie (X). Somit kann der Meteor also immer abgeprallt werden.
Nach nun 10 Sekunden wechselt der Strich sein Kostüm zu einem kleineren, blauen Strich. Dies ist dann sozusagen die nächste Schwierigkeitsstufe, da das Treffen des Meteors nun sschwieriger wird durch die kleinere Fläche. Nach weiteren 10 Sekunden wechselt das Kostüm erneut und ein noch kleinerer Pinker Strich taucht nun auf. 
Durch folgende Befehle haben wir den Kostümwechsel programmiert:

![bsp stride](strichebefehle.png)

Die letzten Befehle "verstecken" und "sende *schwarzes Loch* an alle" bedeuten, dass der Strich nach den insgesamt 30 Sekunden verschwinden soll. Der Andere sendet eine Nachricht, in dem Fall an ein anders Kostüm. Das Kostüm "Schwarzes Loch" taucht also nur dann auf, wenn das Spiel gewonnen ist. Es taucht wie auch die vorherigen Kostüme nach dem Befehl "wenn ich ... empfange" auf. Seine aufgabe solles sein den Meteor aufzusaugen. Damit ist dei Gefahr für den Planenten sozusagen vernichtet.

![bsp stride](schwarzesloch.png)

Das verschwinden des Meteors wird dadurch visualisiert, dass die Befehle des Schwarzen Loches daraus bestehen, dass es zu den Koordinaten X=0 und Y=0 geht und dann dort für ein paar Sekunen bleibt. Nach der Wartezeit soll sich auch diese Sprite verstecken. Danach ist der letzte Befehl dieser Sprite, dass sie "sende *buehneyouwon* an alle senden" absendet. Die Nachricht empfängt dann das Flugzeug.
Da das Spiel in diesem Fall gerade gewonnen wurde, kommt in der nächsten Szene wieder das Flugzeug angeflogen gefolgt von Konfetti. Dem Spieler wird dann gratuliert, dass er diese Welt gerettet hat. Durch die untenstehenden Befehle wird ausgesagt, dass das Flugzeug von den Koordinaten X=-500 Y=0 zu X=0 Y=0 "gleitet". Umgesetzt sieht das so aus als würde es von außerhalb in die Mitte des Bilds fliegen. Dabei haben wir erneut eine gewisse Ausrichtung angegeben und die Größe festgelegt. Zum Schluss sagt es "DANKE! Du hast uns gerettet!!"

![bsp stride](.png)

Kommen wir nun zum anderen Fall, wenn man das Spiel verloren hat. Man verliert in diesem Spiel, wie schon erwähnt, wenn man den Meteor nicht aufhält, den Boden zu berühren. Denn wenn er das tut, dann wird die Welt von ihm zerstört. Wenn dies eintritt sind folgende Befehle dafür zuständig:

![bsp stride](.png)

Die Befehle für den Meteor bestehen daraus, dass er erstmal zu den Koordinaten X=0 und Y=0 wandern soll. Danach sendet er die Nachricht "sende *flugzeugkommen* an alle" ab und wartet 10 Sekunden. Die Zeit ist nötig, damit die damit verbundenen Befehle noch Zeit haben sich auszuführen, bevor der letzte Befehl "stoppe *alles*" eintritt, denn damit wird das Spiel beendet und es passiert nichts mehr. In diesem Fall muss man das Spiel noch einmal von vorne anfangen.
Die Nachricht die vorhin abgesendet wurde bekommt wieder da Flugzeug. Seine ersten Befehle sind genau die Gleichen wie bei dem Fall das man gewonnen hat. Die Szene endet damit, dass das Flugzeug zu den Koordinaten X=500 Y=0 "gleitet" und davor sagt: "Diese Welt konnten wir nicht retten, aber vielleicht beim nächsten Mal!"
