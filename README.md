# Lernbericht

Rose(Nursiwat, Marku, Warnebold, Lucena)
## Einleitung

Wir haben im Lernatelier den Auftrag bekommen, ein Programm mit Windows Forms zu schreiben.
## Was haben wir gelernt?
Wir haben gelernt, wie wir `Key Inputs` in Windows Forms benutzen, um unsere Spielfigur bewegen zu können.
## Beschreibung
Wir haben in unserem Programm die Funktion `keydown` und `keyup` benutzt.
Die Funktion `keydown` prüft, ob eine Taste auf der Tastatur heruntergedrückt wird. Die Funktion `keyup` überprüft, ob eine Taste gerade nicht heruntergedrückt wird. Wir haben das in unserem Programm so eingebaut, dass wir Bool's für alle Tasteninputs haben, die, wenn sie dann `true` sind, die Spielfigur bewegen.
```C#
private void keydown(object sender, KeyEventArgs e)
        {
            if (e.KeyCode == Keys.Space) { if (onground == true) { jump = true; }}
            if (e.KeyCode == Keys.A) { left = true; }
            if (e.KeyCode == Keys.D) { right = true; }
        }
        
private void keyup(object sender, KeyEventArgs e)
        {
            if (e.KeyCode == Keys.Space) { jump = false; onground = false; airtime = false; }
            if (e.KeyCode == Keys.A) { left = false; }
            if (e.KeyCode == Keys.D) { right = false; }
        }
```
_Sobald nun die Leertaste gedrückt wird, wird, wenn `onground` auf `true` ist, `jump` auch auf `true` gesetzt, sodass ein Sprung ausgeführt werden kann. Wenn die Taste losgelassen wird, wird `jump` wieder auf `false` gesetzt. Dasselbe passiert mit den Tasten `a` und `d`._

```C#
this.KeyDown += new System.Windows.Forms.KeyEventHandler(this.keydown);
this.KeyUp += new System.Windows.Forms.KeyEventHandler(this.keyup);
```
_Damit dies jedoch funktioniert, muss zuerst noch ein Event in WinForms erstellt werden._

![image](https://user-images.githubusercontent.com/110893302/229719745-94e1558f-0d89-46dd-95a8-0507a8412661.png)


_Wie man im Video sehen kann, wird, sobald eine Taste gedrückt wird, der Dino nach rechts oder links bewegt oder springt._

## Verifikation

**Text:**  
* Der Text zeigt, dass wir erklären können, wie die gezeigte Methode aufgebaut ist und wir verstanden haben, wie jene funktioniert.

**Video:**  
* Das Video zeigt, dass wir ein Beispiel zur Anwendung von `Key Inputs` kennen und anhand dieses Beispiels weitere Anwendungszwecke nennen können.

**Code:**  
* Der Code zeigt, dass wir verstanden haben, wie wir die beschriebene Methode praktisch anwenden können und diese im VisualStudio umsetzen können.

# Reflektion zum Arbeitsprozess

**Was gut an unserer Arbeit lief:**
* An unserer Arbeit hat besonders das Pair-Programming gut funktioniert, bzw. dass wir in Zweiergruppen gut zusammen arbeiten konnten. Eine Gruppe hat sich dabei vor allem auf den Startbildschirm konzentriert, während sich die andere Gruppe um das eigentliche Spiel gekümmert hat.

**Was nicht gut an unserer Arbeit lief:**
* Auch wenn wir zuerst Gedanken darüber gemacht haben, was das Konzept unseres Projektes sein sollte, haben wir während der Umsetzung gemerkt, dass das Spiel sich immer mehr in eine etwas andere Richtung bewegt, was sich auch anhand der Projektdokumentation bemerkbar gemacht hat.

**VBV**: Sich zum Beginn des Projektes eine klare Struktur des Projektes ausdenken, so dass alle schon am Anfang ein klares Bild vom Projekt haben und so zum Ende des Projektes ein Programm geschaffen wird, welches den ursprünglichen Ansprüchen entspricht.


