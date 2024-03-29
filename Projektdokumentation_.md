# Projekt-Dokumentation

Gruppe Rose: Lucena, Marku, Nursiwat, Warnebold

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 21.02.2023 | 0.0.1  | Wir haben uns in der Gruppe erstmal näher kennengelernt und haben uns zusammen abgesprochen, welche Themen überhaupt infrage kommen würden. Zum Schluss haben wir uns für ein Spiel, dass wir Growrun genannt haben, entschieden. |
| 28.02.2023 | 0.02   | Heute haben wir die User Storys, Arbeitspakete und Testfälle aufgeschrieben. Wir haben Unity heruntergeladen und angefangen zu realisieren.   |
| 07.03.2023 | 0.02   | Heute haben wir viele Arbeitspakete realisiert und zwei der Gruppe haben angefangen die Präsentation vorzubereiten.|                             
| 14.03.2023|0.03 | Wir haben weiter Realisiert und den grössten Teil fertig realisiert. |
|21.03.2023| 0.04| Heute haben wir die Arbeitspackete die noch zu erledigen waren fertig gestellt. Im Spiel sind die Wichtigsten Arbeitspackete fertig.|
| 04.04.2023       | 1.0.0   | Wir haben heute den lernberricht geschrieben und das exploratives testen durch geführt. |                                                        

## 1 Informieren

### 1.1 Ihr Projekt

Wir machen ein 3D-Game in Unity und C#. Es ist ein Runner Spiel. Man steuert einen Charakter, der nach links und rechts bewegen kann. Auf dem Weg sind Hindernisse, denen man ausweichen muss. Ausserdem hat es auf dem Weg Münzen, die man einsammeln kann. Unity ist für uns alle neu. Es ist unser erstes 3D Spiel. Es ist anspruchsvoll, doch sehr spannend. Wir wollen viel über Unity und 3D Spiele lernen und erfolgreich unser erstes Spiel programmieren.

### 1.2 User Stories
|
| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    |  Muss           |  F  | Als ein User möchte ich, dass ich ein Level auswählen kann, damit ich spielen kann.|
| 2    |  Muss           |  F  | Als ein User möchte ich, dass ich automatisch nach vorne gehen kann.  |
| 3    |  Muss           |  F  | Als ein User möchte ich, dass ich mein Charakter nach rechts bewegen kann, damit mein Charakter nicht in die Hindernisse reinläuft. |
| 4    |  Muss           |  F  | Als ein User möchte ich, dass ich mein Charakter nach links bewegen kann, damit mein Charakter nicht in die Hindernisse reinläuft. |
| 5    |  Muss           |  F  | Als ein User möchte ich, dass ich das Level wiederholen kann, falls ich verliere, damit ich noch eine Chance bekomme, das Level zu bewältigen. |
| 6    |  Muss           |  F  | Als ein User möchte ich, dass ich zum nächsten Level gehen kann, falls ich das gespielte Level überwinde, damit ich nicht immer beim selben Level bleibe. |
| 7    |  Muss           |  F  | Als ein User möchte ich, dass ich mit meinem Charakter Münzen auf dem Weg sammeln kann, damit ich mir coole Skins später kaufen kann.|
| 8    |  Muss           |  F  | Als ein User möchte ich, dass wenn ich durch eine Türe, die dich kleiner macht, laufe kleiner werde. |
| 9    |  Muss           |  F  | Als ein User möchte ich, dass wenn ich durch eine Türe, die dich grösser macht, laufe grösser werde.  |
| 10   |  Muss           |  F  | Als ein User möchte ich, dass ich, wenn ich grösser bin, mehr Münzen sammeln kann, damit das Spiel einfacher für mich wird. |
| 11   |  Muss           |  F  | Als ein User möchte ich, dass ich auch schrumpfen kann, damit das Spiel schwieriger wird |
| 12   |  Kann           |  Q  | Als ein User möchte ich, dass ich einen Shop öffnen kann, damit ich Skins kaufen kann. |
| 13   |  Kann           |  Q  | Als ein User möchte ich, dass ich mit Münzen einen Skin kaufen kann, damit ich cooler aussehe. |
| 14   |  Kann           |  Q  | Als ein User möchte ich, dass die Levels immer schwieriger werden, damit es eine Herausforderung für mich ist.  |
| 15  |  Kann           |  Q  | Als ein User möchte ich, dass ich im Level Menu sehen kann, welche Levels ich schon bewältigt habe, damit ich weiss wie viele ich noch vor mir habe. |
|16|Kann | Q | Als ein User möchte ich eine Anzeige haben, wie viel Münzen ich schon gesammelt habe, damit ich weiss, wann ich einen Skin kaufen kann.|
|17 |Kann | Q |Ich möchte als User die Lautstärke des Spieles bestimmen können.|


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |  Applikation gestartet      |   Level im Menu ausgewählt.     |   Level gestartet             |
| 2.1  |  Level gestartet            |     -    |  Spieler automatisch nach vorne gehen                |
| 3.1  |  Spieler geht automatisch nach vorne     |     rechte Pfeiltaste drücken      |     Spieler bewegt sich nach rechts         |               
| 4.1  |  Spieler geht automatisch nach vorne      |    linke Pfeiltaste drücken        |      Spieler bewegt sich nach links        |               
| 5.1  |  Spieler läuft in ein Hindernis rein und verliert     |    Auf Level wiederholen klicken       |    Level startet neu         |               
| 6.1  |  Spieler bewältigt das Level     |    -       |      Nächstes Level vorgeschlagen        |               
| 7.1  | Spieler läuft durch eine grösser werdende Türe im Level durch      |   -          |      Spieler wird grösser        |       
| 8.1  | Spieler läuft durch eine kleiner werdende Türe im Level durch      |   -       |       Spieler wird kleiner    |       
| 9.1 |   Level läuft und Spieler ist grösser geworden    |     -      |    Grösser Fläche wird vom Spieler abgedeckt, also einfacher Münzen aufzusammeln    |       
| 10.1 |   Level läuft und Spieler ist kleiner geworden    |  -         |     Kleiner Fläche wird vom Spieler abgedeckt, also schwieriger Münzen aufzusammeln   |  
| 11.1 |  Benutzer ist im Menu des Spieles    |     Auf Shop klicken     |    Man kommt ins Shop und sieht alle möglichen Skins, die man kaufen kann       |      
| 12.1 |  Benutzer ist im Shop des Spieles     |     Skin auswählen     |    Skin wird im Tausch von Münzen gekauft         |     
| 13.1 |  Nächstes Level wird gestartet |     -        |    Dieses Level ist schwieriger, als das vorherige     |               
| 14.1 |  Benutzer ist im Menu des Spieles     |   Auf Level Menu klicken        |   die Levels, die es gibt, sehen.          |   
| 15.1 |  Benutzer ist im Level Menu des Spieles    |      -     |     Die Levels, die er noch nicht bewältigt/bewältigt hat sehen         |   
|16.1| Benutzer ist im Menü des Spieles |  -  |Die Münzen, die man eingesammelt hat, werden angezeigt.|
|17.1 | Benutzer ist im Menü des Spieles  | Lautstärke auswählen | Der Spielsound wird leiser/lauter.|


### 1.4 Diagramme
[<img width="422" alt="image" src="https://user-images.githubusercontent.com/110892575/220322647-f30f1589-278a-4aef-9509-8c1940a2dc88.png">](https://bbbaden.sharepoint.com/:i:/r/sites/Lernatelier20222023/Freigegebene%20Dokumente/Rose/Screenshot%202023-02-21%20111141.png?csf=1&web=1&e=wvJqmU)

![grafik](https://user-images.githubusercontent.com/110892623/223351584-04c042c8-31d3-4c03-ab08-2752e2b538e0.png)


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit(in min) |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 07.03 | Nursiwat | Den Startbildschirm erstellen| 45' |
| 1.B     | 07.03 |  Nursiwat | Das Level Menü erstellen| 45' |
| 2.A     | 07.03 |Marku        | Spieler läuft automatisch nach vorne| 45'|
| 3.A     | 07.03 |Warnebold           | Hindernisse erstellen|45'|
| 3.B     | 07.03 |  Warnebold         | Verschiedene Hindernisse sind auf dem Weg|45'|
| 4.A | 07.03 |   Warnebold        | Den Spieler mit den Pfeiltasten nach links bewegen können.|45'|
| 4.B | 07.03 |  Lucena         | Den Spieler mit den Pfeiltasten nach rechts bewegen können.|45'|
| 5.A  | 14.03 | Lucena           | Level kann man wiederholen, wenn man es nicht geschafft hat.|45' |
| 5.B  | 07.03 | Lucena           | Wenn man im Level gegen ein Hindernis läuft, muss man das Level wiederholen| 45'|
| 6.A| 14.03 | Nursiwat          | Man bekommt die option zum nächsten Level zu gehen, wenn man es bewältigt hat. | 45' |
| 7.A| 07.03 | Marku          | Münzen sammeln | 45'|
| 7.B | 14.03 | Marku           | Münzen können gespeichert und benutzt werden| 45' |
| 7.C | 14.03 | Marku           | Man kann mit Münzen Skins im Shop kaufen| 45'|
| 8.A | 14.03 | Warnebold          | Den Spieler kleiner machen, wenn er durch eine verkleinerungs Tür läuft  |45' |
| 9.A | 14.03 | Lucena          | Den Spieler grösser machen, wenn er durch eine vergrösserungs Tür läuft  |  45'  |
| 10.A| 14.03 | Lucena          | Die Hitbox von dem Spieler wird geändert, wenn er grösser wird.|45' |
| 11.A|14.03 | Nursiwat         | Die Hitbox von dem Spieler wird geändert, wenn er kleiner wird.|45' |
|12.A|14.03  | Nursiwat                      |Den Shop für Skins wird erstellt|45'|
|13.A|14.03 |  Marku                   |Skins im Shop für Münzen kaufen|45'|
|14.A| 14.03 | Marku                  | Plattform, wo man darauf rennt, erstellen   |45'|
|15.A|14.03 |Warnebold         |  Im Menü kann man sehen, welche Levels man schon bewältigt hat.|45'|
| 16.A| 14.03 | Nursiwat          | Es wird angezeigt, wie viel Münzen man eingesammelt hat. |45'|

Total: 990 min



## 3 Entscheiden

Wir haben uns für ein Runnerspiel entschieden, weil keiner aus unserer Gruppe so ein Spiel programmiert hat und wir es lustig fanden.

Wir haben uns entschieden, mit Unity zu arbeiten, da wir etwas Neues lernen wollten.


## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |  07.03  |   Nursiwat      |      45'         |         60'       |
| 1.B  |  07.03  |   Nursiwat      |      45'         |         30'       |
| 2.A  |  07.03  |   Marku         |      45'         |         40'       |
| 3.A  |  07.03  |   Warnebold     |      45'         |         30'       |
| 3.B  |  07.03  |   Warnebold     |      45'         |         50'       |
| 4.A  |  07.03  |   Warnebold     |      45'         |         -         |
| 4.B  |  07.03  |   Lucena        |      45'         |         -         |
| 5.A  |  07.03  |   Lucena        |      45'         |         25'       |
| 5.B  |  07.03  |   Lucena        |      45'         |         25'       |
| 6.A  |  14.03  |   Nursiwat      |      45'         |         45'       |
| 7.A  |  07.03  |   Marku         |      45'         |         40'       |
| 7.B  |  14.03  |   Marku         |      45'         |         -         |
| 7.C  |  14.03  |   Marku         |      45'         |         -         |
| 8.A  |  07.03  |   Warnebold     |      45'         |         25'       |
| 9.A  |  07.03  |   Lucena        |      45'         |         25'       |
| 10.A |  07.03  |   Lucena        |      45'         |         25'       |
| 11.A |  07.03  |   Nursiwat      |      45'         |         25'       |
| 12.A |  14.03  |   Nursiwat      |      45'         |         -         |
| 13.A |  14.03  |   Marku         |      45'         |         -         |
| 14.A |  07.03  |   Marku         |      45'         |         25'       |
| 15.A |  14.03  |   Warnebold     |      45'         |         -         |
| 16.A |  14.03  |   Nursiwat      |      45'         |         -         |




## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |  04.04   |  Level gestartet        |  Lucena     |
| 2.1  |  04.04   |  Spieler geht automatisch        |  Lucena      |
| 3.1  |  04.0|  Spieler bewegt sich nach rechts        |  Lucena      |
| 4.1  |  04.04    |  ch nach link        |   Lucena     |
| 5.1  |   04.04    |  Level startet neu        | Marku      |
| 6.1  |  04.04   |  Nächstes Level vorgeschlagen        |  Nursiwat      |
| 7.1  |   04.04 |  Spieler wird grösser        |  Lucena      |
| 8.1  |  04.04  |  Spieler wird kleiner        |   Lucena     |
| 9.1  |  04.04  |  Spieler Fläche ist grösser        |   Nursiwat     |
| 10.1  |   04.04  | Spieler Fläche ist kleiner         |  Nursiwat      |
| 11.1  |  04.04   | Shop mit Skins die man kaufen kann         |   Warnebold     |
| 12.1  | 04.04  | Skin für münzen bekommen         |  Warnebold      |
| 13.1  |  04.04    | Schwierigeres Level         |   Nursiwat     |
| 14.1  |  04.04   | Alle Level die es gibt         |  Marku      |
| 15.1  | 04.04   | Levels die noch nicht bewletigt sind         |  Marku      |
| 16.1  |  04.04  | Eingesammelte Münzen         |  Warnebold      |
| 17.1  |   04.04   | Sound wird lauter oder leiser         |  Warnebold      |



### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    | Spiel startet| Maus ganz nach links|Nichtr von der Karte fallen|Nicht von der Karte gefallen|
| II   | Spiel läuft  |linke Pfeiltaste| Charachter bewegt sich nach links|Passiert nichts|
| III  | Spiel beendet|nichts   |Man kommt ins nächste Level|Man kommt ins gleiche Level|


## 6 Auswerten

![Lernbericht](https://github.com/twopad/LA1500/blob/main/Lernbericht.md)
