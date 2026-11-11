# Unicorn Evaluation Module

! Wichtige Hintergrundinformationen für **Konzentrationen** und **Peak Evaluation** und andere Berechnungen unter **Help** mit schönen Bildern verwendbar.

! Im **System Control** kann man direkt mit dem oberen **Curve Button** in dieses _Evaluation Module_ switchen.


### Navigation für das Öffnen

- [ ] Mit kleinen Pfeilen kann man in der Ordnerstruktur nach den Ergebnissen filtern, mit einem Preview kann man eines davon laden.
- [ ] Doppelklick/Ein Klick mit _Open Compare_.
- [ ] Mit _fx_ (rechts) kann man die Peak Integration ausschalten.
- [ ] Mit dem kleinen schwarzen Dreieck (rechts) kann man weitere Linien zufügen.
- [ ] Mit Klick auf diesen Eintrag in der Legende kann man _Color_ etc. ändern. Dabei ändert sich automatisch auch die Beschriftung auf der _y-Achse_ mit.
- [ ] Mit Klick auf die _x-Achse_ kann man CV, ml, min umtauschen.
- [ ] Mit Hover über _x-Achse_ kann man **benannte** Methodenschritte grau hinterlegen.
- [ ] Peakkurve analysieren. **Je größer der Oligomerisierungszustand** (oder mit Schulter) desto später eluiert es von Säule, da es höhere Ladungen trägt.

* Bei UV-Linie ist der Wert auf meistens exakt 2 mm angezeigt.


### Manuelle Analyse der Kurve

* mit vertikalem Ergebniscursor punktweise
* oder durch Markieren (Ziehen über) einen Bereich als Tabelle
* **Zoomen:** mit Halten der linken Maustaste und ziehen über zu vergrößernden Bereich
* **Herauszoomen:** mit Doppelklick auf linke Maustaste

! Je kleiner die Säule, desto wichtiger das System mit den Puffern einzuspülen (z.B. bei 1 ml Säulenvolumen). **Wichtig für die Ribosomenaufreinigung.**


### Fehler welche passieren

* Im _Method Evaluator_ mit **Only show suggested** Columns kann man vorsortieren, welche Säulen für das System empfohlen sind.
  
? Driftende Basislinie in UV-Linie: **Luftblase in Flusszelle**. ! In diesem Fall einen _System Wash_ durchführen. Oder: Mit _Hold_ (☀) das System einfrieren.

? Peak kommt bei der Applikation, nicht erst in Elution. ! Dies ist entweder _Flowtrough_ oder eine _Überladung der Säule_. 

? Conductivity kommt nicht schnell auf Baseline in Equilibration zurück. Dies zeigt z.B. oft, dass man ein größeres System verwendet mit größeren Totvolumen.

? Manche Häkchen oder Funktionen im _Method Editor_ waren nicht verfügbar obwohl sehr neue Funktion. Dies kann sein, wenn z.B. der Treiber und das System nicht mehr zusammenpassen. Treiber aktualisieren.

? Druck ist sehr hoch (höher als 0.2 MPa). ! Dann zuerst den Filter tauschen. Ansonsten den Restriktor kalibrieren.

? Druck bricht ein an gewissen Stellen. ! Wenn ÄKTA ein Ventil dreht, dann könnte ÄKTA auf eine Sackgasse treffen und extrem hohen Druck aufbauen (z.B. Injektionsventil) und die ÄKTA fährt daher den Druck stark runter. 
