# Lern-Bericht-Zahlenspiel
Samuel Lucena

## Einleitung

Ich habe ein Zahlenspiel programmiert.

## Was habe ich gelernt?

Ich habe gelernt mit Spielerinput umzugehen sodass mein Programm nicht abschmiert.

## Beschreibung

Als ich angefangen habe viel mir es recht schwer überhaupt so ein Zahlenspiel zu programieren. Aber mit den Mitteln die ich zur verfügung hatte wie Youtube oder Reddit fand ich schnell raus wo meine Fehler waren.
![final_632041d1629d2c13c50d1b2b_665932](https://user-images.githubusercontent.com/110893302/189854568-39c4845d-b162-4f7a-95cb-b0deac529aae.gif)
das einzige Problem das ich noch hatte war das mein Projekt immer abschmierte, wenn ich nicht eine Zahl eingab. Ich habe zuerst überlegt was ich dagegen unternehmen kann und habe mit der Hilfe von Marek und dem Internet eine Lösung gefunden:
```csharp
while (check == false)
{
    try
    {
        Console.ForegroundColor = ConsoleColor.White;
        Console.Write("Denke dir eine Zahl aus zwischen " + min + " - " + max + ": ");
        Console.ForegroundColor = ConsoleColor.Cyan;
        guess = Convert.ToInt32(Console.ReadLine());
        check = true;
    }
    catch
    {
        Console.WriteLine("ERROR");
        check = false;
    }
}
check = false;
```

## Verifikation

Ich bin auf eine Lösung gekommen die mein Problem behoben hat. Jetzt weiss ich auch wie ich try catch richtig anwenden.

# Reflektion zum Arbeitsprozess

Am Anfang des Projekts war ich sehr unproduktiv und unmotiviert da ich nicht wusste wie ich anfangen sollte. Ich habe auch immer andere gefragt mir zu Helfen. Mit der Zeit kam ich besser rein und habe mich ins Zeug gelegt um Zeitlich auf dem neusten Stand zu sein.


**VBV**: Ich muss wenn ich gut arbeite bessere Pausen einteilen und wenn ich unmotiviert bin mich besser selbsständig um das Problem kümmern.
