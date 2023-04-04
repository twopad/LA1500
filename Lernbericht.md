# Lernbericht
Rose(Nursiwat, Marku, Warnebold, Lucena)
## Einleitung
Wir haben im Lernatelier den Auftrag bekommen, in Gruppen etwas zu programmieren. Wir haben uns entschieden, ein Spiel mit Unity zu programmieren.
## Was haben wir gelernt?

Wir haben gelernt, wie man in Unity Musik einfügt.
## Beschreibung
Wir haben in unserem Programm mit `m_MusicSource` den `audioClip` abspielen lassen.
Dieses `m_MusicSource` sucht den Audio-Clip, der bei dem grauen Block (_siehe Bild_) eingefügt wurde und spielt in Dank `bool looping = true` immer wieder ab, bis man in den nächsten Bildschirm kommt.
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

Hier oben bei `Sound ID` bestätigt das Programm einfach, dass es den gewählten Sound (_Im Bild rechts bei Music Source_) abspielt und loopt.

![image](https://user-images.githubusercontent.com/110893302/229719745-94e1558f-0d89-46dd-95a8-0507a8412661.png)

## Verifikation

**Text:**  
* Der Text zeigt, dass wir erklären können, wie die gezeigte Methode aufgebaut ist und wir verstanden haben, wie jene funktioniert.

**Bild:**  

* Das Video zeigt, dass wir diese Funktion in unserem Spiel richtig einbauen konnten.

**Code:**  

* Der Code zeigt, dass wir das Prinzip von Musik in Unity verstanden haben, und es in weiteren Projekten mit Visual Studio verwenden können.

# Reflektion zum Arbeitsprozess

**Was gut an unserer Arbeit lief:**

* An unserer Arbeit hat besonders das Zusammenarbeiten gut funktioniert. Auch zu viert konnten wir produktiv an einer Aufgabe arbeiten, ohne vom Thema abzuschweifen. Die Arbeitspakete haben wir gut verteilt, weshalb wir einen guten Überblick hatten.

**Was nicht gut an unserer Arbeit lief:**

* Unser Projekt verlief schlussendlich nicht genau wie geplant, jedoch ist das für uns kein schlechter Aspekt. Obwohl wir uns zuerst Gedanken darüber gemacht haben, welches das Konzept unseres Projektes sein sollte, haben wir während der Umsetzung festgestellt, dass sich das Spiel in eine etwas andere Richtung veränderte.

**VBV**: Wir haben viel zu viel Zeit verloren beim Verknüpfen von Unity, ansonsten verlief unser Projekt sehr gut und alle haben etwas profitieren können.

