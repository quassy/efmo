# Taktik

Die Taktiken sind mit der [Aufstellung] zusammen das Herzstück zur Spielberechnung bei FM-O. Jedoch sind sie teilweise relativ komplex, wenn man mehrere Dinge gleichzeitig machen möchte.

Die Grundeinstellungen zu Spielbeginn bei Härte, Einsatz und Taktik sind jeweils "normal". Möchte man mit "normal" in einem dieser Bereiche beginnen, und hat dies auch eingestellt, wird bei "ausgeführt" immer "nein" stehen, da es ja von vornherein schon so war, und daher keine Taktikänderung nötig war.

! Grundprinzip

Es gibt 6 Optionen, die eingestellt werden können. Diese sind:

*'''Taktik''': Allgemeine Ausrichtung. Von Abwehrriegel bis Brechstange sind 7 Möglichkeiten vorhanden.
*'''Härte''': Die Härte gibt an, wie aggressiv Spieler in die Zweikämpfe geben. Sie kann in 5 Stufen von "Nonnenhockey" bis "brutal" eingestellt werden. Je aggressiver die Zweikämpfe geführt werden, desto mehr können gewonnen werden. Jedoch steigen auch das [Verletzungsrisiko|Verletzungen] der eigenen und gegnerischen Spieler, sowie das Risiko auf Verwarnungen und Platzverweise, die [Sperren] nach sich ziehen.
*'''[Einsatz]''': Mit viel Einsatz gehen die Spieler weitere Wege, mit wenig joggen sie mehr. 5 Stufen.
*'''[Aus-/Einwechslungen|Wechsel]''': Maximal werden 3 Wechsel pro Spiel ausgeführt. Einstellen kann man mehr.
*'''Spielposition''': Wer nach einem Wechsel wo spielt. Ideal ist immer "Minute größer 1", da dann die Umstellung immer direkt nach dem Wechsel erfolgt.
*'''Manndeckung''': Soll ein MD, Lib oder ZM den gegnerischen Spieler decken oder nicht? Gibt es nur zwei Gegner, die gedeckt werden können, aber drei Spieler haben die Anweisung, führt sie einer nicht aus.


! Bedingungen für Taktiken

Es gibt 5 Bedingungen für Taktiken, unter denen eine Taktik einsetzen soll oder eben nicht. Diese sind:

*'''Minute''': Logisch. Beachte: Minute größer/kleiner gilt für '''jede''' Minute, die diese Bedingung erfüllt, auch die 1. Minute.
*'''Tordifferenz''': Auch logisch. -2 ist 2 Tore Rückstand, 0 ist unentschieden, +2 ist 2 Tore in Führung.
*'''Eigene Spieler''': Es geht um die Anzahl der eigenen Spieler auf dem Platz.
*'''Gegner. Spieler''': Hier geht es um die Anzahl der gegnerischen Spieler auf dem Platz.
*'''Karten'''_ Hier geht es um die Anzahl der Karten für die eigenen Spieler '''auf dem Platz'''. Eine Gelbrote Karte führt also zur Reduzierung der Karten um 1, ebenso eine Auswechslung.

! Wie stelle ich Taktiken ein?

Grundsätzlich stellt man Taktiken folgendermaßen ein:

* ''Auswahl der Option''
* ''(Auswahl der Stufe, der Position oder des Wechsels falls vorhanden)''
* ''Auswahl der Bedingung'' (wenn man hier nichts eingibt, wird die Option zu Spielbeginn ausgeführt)
* ''Auswahl weiterer Bedingungen'' (optional)

'''Alle Einzeltaktiken mit mehreren Bedingungen sind UND-verknüpft'''. Es müssen also ''alle'' eingestellten Bedingungen erfüllt sein.
Verschiedene Taktiken sind ODER-verknüpft.

Bereits in anderen Spielen verwendete (also alte) Taktiken lassen sich auch über eine Auswahlbox im Taktikmenü hinzufügen.

'''Bei mehreren Taktiken mit gleichen Bedingungen wird immer die obere (zuerst eingegebene) durchgeführt. Wenn man also möchte, dass der stärkere MD deckt, wenn der Gegner mit nur einem Stürmer spielt, sollte man "Manndeckung" zuerst bei ihm einstellen.'''

! Häufig gemachte Fehler/Ausführung der Taktiken

Taktiken werden nur dann ausgeführt, wenn sie sich nicht in sich widersprechen. Ebenso muss eine neue Bedingung eintreten, damit eine Taktik ausgeführt wird. Gelten verschiedene Optionen gleichzeitig, weil alle Bedingungen erfüllt sind, werden die Optionen, deren Bedingungen später erfüllt wurden, nicht ausgeführt (bei Gleichzeitigkeit die in der Taktik hinten stehenden).

!! Beispiel 1

*''Einsatz wenig wenn Tordifferenz größer 1 und kleiner -2''

Die Taktik wird nicht ausgeführt, da sie einen Spielstand erfordern würde, bei dem man gleichzeitig mit mehr als einem Tor führt und mehr als zwei Toren im Rückstand liegt. Und den gibts einfach nicht. 

Besser wäre in diesem Fall, zwei Taktiken zu erstellen, einmal ''Einsatz wenig wenn Tordifferenz größer 1'' und ''Einsatz wenig wenn Tordifferenz kleiner -2''

!! Beispiel 2

*''Härte rauh nur zu Spielbeginn einmalig ausführen''
*''Härte normal wenn Tordifferenz größer 0''
*''Härte rücksichtsvoll wenn Tordifferenz größer 1''

Die zweite und dritte Taktik schließen sich nicht gegenseitig aus. Wenn man mit zwei Toren führt, ist die Tordifferenz sowohl größer 0, als auch größer 1. Daher wird die später eintreffende Taktik nicht ausgeführt.

Besser wäre, die zweite Taktik auf ''Härte normal wenn Tordifferenz '''gleich''' 1'' zu ändern. Damit schließen sich alle drei Taktiken gegenseitig aus.

!! Beispiel 3

*''Spieler X für Spieler Y wenn Minute kleiner 80 und Tordifferenz kleiner 1''

Nicht schön, aber selten und unpraktisch. Die Bedingung ist auch zu Spielbeginn erfüllt. Also wird der Wechsel gleich in der 1. Minute erfolgen.

Besser: Einfügen einer weitern Minutenbedingung, sowas wie ''und Minute größer 70''. Damit wird der Spieler zwischen der 71. und 79. Minute eingewechselt.

## Einsatz

Der Einsatz ist eine [Taktik], die man für eigene Spiele vornehmen kann. Die Standardeinstellung für Einsatz, sofern kein anderer eingestellt ist, ist immer "normal".

Es gibt 5 Stufen von Einsatz:
*"kein"
*"wenig"
*"normal"
*"hoch"
*"sehr hoch"

Alle 5 Stufen sind Abstufungen und haben Vor- und Nachteile. Bei höherem Einsatz als "normal" steigt die Stärke des eigenen Teams leicht an, weil man mehr Einsatz zeigt. Dafür steigen das Verletzungsrisiko, das Risiko auf Karten, und der Verlust von [Frische] auch mit höherem Einsatz. Bei niedrigerem Einsatz als "normal" ist es genau umgekehrt.
