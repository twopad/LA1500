# Lernbericht

Rose(Nursiwat, Marku, Warnebold, Lucena)
## Einleitung

Wir haben im Lernatelier den Auftrag bekommen in Gruppen etwas zu programmieren. Wir haben uns entschieden ein Spiel mit Unity zu Programmieren.

## Was haben wir gelernt?
Wir haben gelernt, wie man in Unity Musik einfügt.
## Beschreibung
Wir haben in unserem Programm die Funktion `keydown` und `keyup` benutzt.
Die Funktion `keydown` prüft, ob eine Taste auf der Tastatur heruntergedrückt wird. Die Funktion `keyup` überprüft, ob eine Taste gerade nicht heruntergedrückt wird. Wir haben das in unserem Programm so eingebaut, dass wir Bool's für alle Tasteninputs haben, die, wenn sie dann `true` sind, die Spielfigur bewegen.
```C#
void PlayMusic(AudioClip audioClip, bool looping = true)
        {
            if (m_MusicSource.isPlaying)
                return;
           
            m_MusicSource.clip = audioClip;
            m_MusicSource.loop = looping;
            m_MusicSource.Play();
        }
       
        public void PlayMusic(SoundID soundID, bool looping = true)
        {
            PlayMusic(m_Clips[soundID], looping);
        }
```
_Sobald nun die Leertaste gedrückt wird, wird, wenn `onground` auf `true` ist, `jump` auch auf `true` gesetzt, sodass ein Sprung ausgeführt werden kann. Wenn die Taste losgelassen wird, wird `jump` wieder auf `false` gesetzt. Dasselbe passiert mit den Tasten `a` und `d`._
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

* An unserer Arbeit hat besonders das Zusammenarbeiten gut funktioniert. Auch zu viert konnten wir produktiv an einer Aufgabe arbeiten, ohne vom Thema abzuschweifen. Die Arbeitspakete haben wir gut verteilt, weshalb wir einen guten Überblick hatten.


**Was nicht gut an unserer Arbeit lief:**

* Unser Projekt verlief schlussendlich nicht genau wie geplant, jedoch ist das für uns kein schlechter Aspekt. Obwohl wir uns zuerst Gedanken darüber gemacht haben, welches das Konzept unseres Projektes sein sollte, haben wir während der Umsetzung festgestellt, dass sich das Spiel in eine etwas andere Richtung veränderte.


**VBV**: Wir haben viel zu viel Zeit verloren beim Verknüpfen von Unity, ansonsten verlief unser Projekt sehr gut und alle haben etwas profitieren können.

