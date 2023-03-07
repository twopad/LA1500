# Projekt-Dokumentation

Gruppe Rose: Lucena, Marku, Nursiwat, Warnebold

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
|  21.02.2023    | 0.0.1   | Wir haben uns in der Gruppe erstmal näher kennengelernt und haben uns zusammen abgesprochen, welche Themen überhaupt infrage kommen würden. Zum Schluss haben wir uns für ein Spiel, dass wir Growrun genannt haben, entschieden. |
| 28.02.2023 | 0.02 | Heute haben wir die User Storys, Arbeitspakete und Testfälle aufgeschrieben. Wir haben Unity heruntergeladen und angefangen zu realisieren.                                                             |
|       | 1.0.0   |                                                              |

## 1 Informieren

### 1.1 Ihr Projekt

Wir machen ein 3D-Game in Unity und C#. Es ist ein Runner Spiel. Man steuert einen Charakter, der nach links und rechts bewegen kann. Auf dem Weg sind Hindernisse, denen man ausweichen muss. Ausserdem hat es auf dem Weg Münzen, die man einsammeln kann. Unity ist für uns alle neu. Es ist unser erstes 3D Spiel. Es ist anspruchsvoll, doch sehr spannend. Wir wollen viel über Unity und 3D Spiele lernen und erfolgreich unser erstes Spiel programmieren.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    |  Muss           |  F  | Als ein User möchte ich, dass ich ein Level auswählen kann, damit ich spielen kann.|
| 2    |  Muss           |  F  | Als ein User möchte ich, dass ich automatisch nach vorne gehen kann.  |
| 3    |  Muss           |  F  | Als ein User möchte ich, dass ich mein Charakter nach rechts bewegen kann, damit mein Charakter nicht in die Hindernisse reinläuft. |
| 4    |  Muss           |  F  | Als ein User möchte ich, dass ich mein Charakter nach links bewegen kann, damit mein Charakter nicht in die Hindernisse reinläuft. |
| 5    |  Muss           |  F  | Als ein User möchte ich, dass ich das Level wiederholen kann, falls ich verliere, damit ich noch eine Chance bekomme, das Level zu bewältigen. |
| 6    |  Muss           |  F  | Als ein User möchte ich, dass ich direkt zum nächsten Level gehe, falls ich das gespielte Level überwinde, damit ich nicht immer beim selben Level bleibe. |
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
| 6.1  |  Spieler bewältigt das Level     |    -       |      Nächstes Level beginnt automatisch        |               
| 7.1  |  Level läuft   |    rechte/linke Pfeiltaste        |     Ton         |
| 8.1  | Spieler läuft durch eine grösser werdende Türe im Level durch      |   -          |      Spieler wird grösser        |       
| 9.1  | Spieler läuft durch eine kleiner werdende Türe im Level durch      |   -       |       Spieler wird kleiner    |       
| 10.1 |   Level läuft und Spieler ist grösser geworden    |     -      |    Grösser Fläche wird vom Spieler abgedeckt, also einfacher Münzen aufzusammeln    |       
| 11.1 |   Level läuft und Spieler ist kleiner geworden    |  -         |     Kleiner Fläche wird vom Spieler abgedeckt, also schwieriger Münzen aufzusammeln   |  
| 12.1 |  Benutzer ist im Menu des Spieles    |     Auf Shop klicken     |    Man kommt ins Shop und sieht alle möglichen Skins, die man kaufen kann       |      
| 13.1 |  Benutzer ist im Shop des Spieles     |     Skin auswählen     |    Skin wird im Tausch von Münzen gekauft         |     
| 14.1 |  Nächstes Level wird gestartet |     -        |    Dieses Level ist schwieriger, als das vorherige     |               
| 15.1 |  Benutzer ist im Menu des Spieles     |   Auf Level Menu klicken        |   die Levels, die es gibt, sehen.          |   
| 15.1 |  Benutzer ist im Level Menu des Spieles    |      -     |     Die Levels, die er noch nicht bewältigt/bewältigt hat sehen         |   
|16.1| Benutzer ist im Menü des Spieles ||Die Münzen, die man eingesammelt hat, werden angezeigt.|
|17.1 | Benutzer ist im Menü des Spieles  | Lautstärke auswählen | Der Spielsound wird leiser/lauter.|


### 1.4 Diagramme
[<img width="422" alt="image" src="https://user-images.githubusercontent.com/110892575/220322647-f30f1589-278a-4aef-9509-8c1940a2dc88.png">](https://bbbaden.sharepoint.com/:i:/r/sites/Lernatelier20222023/Freigegebene%20Dokumente/Rose/Screenshot%202023-02-21%20111141.png?csf=1&web=1&e=wvJqmU)
![grafik](https://user-images.githubusercontent.com/110892623/220322854-83762dce-c406-4e83-b9e3-902da2116f30.png)



## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit(in min) |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 07.03 | Nursiwat | Den Startbildschirm erstellen| 45' |
| 1.B     | 07.03 |  Nursiwat | Das Levelmenü erstellen| 45' |
| 2.A     | 07.03 |Marku        | Spieler läuft automatsich nach vorne| 45'|
| 3.A     | 07.03 |Warnebold           | Hindernisse erstellen|45'|
| 3.B     | 07.03 |  Warnebold         | Verschiedene Hindernisse sind auf dem Weg|45'|
| 3.C | 07.03 |   Warnebold        | Den Spieler mit den Pfeiltasten nach links bewegen können.|45'|
| 4.A | 07.03 |  Lucena         | Den Spieler mit den Pfeiltasten nach rechts bewegen können.|45'|
| 5.A  | 14.03 | Lucena           | Level kann man wiederholen, wenn man es nicht geschafft hat.|45' |
| 5.B  | 07.03 | Lucena           | Wenn man im Level gegen ein Hinderniss läuft, muss man das Level weiderholen| 45'|
| 6.A| 14.03 | Nursiwat          | Man geht automatisch zum nächsten Level, wenn man es bewältigt hat. | 45' |
| 7.A| 07.03 | Marku          | Münzen sammeln | 45'|
| 7.B | 14.03 | Marku           | Münzen können gespeichert und benutzt werden| 45' |
| 7.C | 14.03 | Marku           | Man kann mit Münzen Skins im Shop kaufen| 45'|
| 8.A | 14.03 | Warnebold          | Den Spieler kleiner machen wenn er durch eine verkleinerungs Tür läuft  |45' |
| 9.A | 14.03 | Lucena          | Den Spieler grösser machen wenn er durch eine vergrösserungs Tür läuft  |  45'  |
| 10.A| 14.03 | Lucena          | Die Hitbox von dem Spieler wird geändert, wenn er grösser wird.|45' |
| 11.A|14.03 | Nursiwat         | Die Hitbox von dem Spieler wird geändert, wenn er kleiner wird.|45' |
|12.A|14.03  | Nursiwat                      |Den Shop für Skins wird erstellt|45'|
|13.A|14.03 |  Marku                   |Skins im shop für Münzen kaufen|45'|
|14.A| 14.03 | Marku                  | Plattform, wo man drauf rennt, erstellen   |45'|
|15.A|14.03 |Warnebold         |  Im Menü kann man sehen welche Levels man schon bewältigt hat.|45'|
| 16.A| 14.03 | Nursiwat          | Es wird angezeigt wie veiel Münzen man eingesammelt hat. |45'|

Total: 990 min

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
