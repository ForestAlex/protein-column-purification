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
- [ ] Man kann sich mehrere x- und y-Achse verwenden.
- [ ] Export mit _.csv_ möglich.
      
* Bei UV-Linie ist der Wert auf meistens exakt 2 mm angezeigt.

* Man darf mit dem System über das Mixerumgangsventil auch Probe laden.

* Bei zu niedrigem Druck den _Flow Restrictor_ an den _System Pressure Monitor_ anhängen.

### Manuelle Analyse der Kurve

* mit vertikalem Ergebniscursor punktweise
* oder durch Markieren (Ziehen über) einen Bereich als Tabelle
* **Zoomen:** mit Halten der linken Maustaste und ziehen über zu vergrößernden Bereich
* **Herauszoomen:** mit Doppelklick auf linke Maustaste

! Je kleiner die Säule, desto wichtiger das System mit den Puffern einzuspülen (z.B. bei 1 ml Säulenvolumen). **Wichtig für die Ribosomenaufreinigung.**

### Exportieren

Export als _.csv_ möglich. Man kann auch _Reports_ erstellen.

### Dokumentation

Unter _Documentation_ kann man _Text Instructions_ und **Save as** die Originalmethode verwenden. (Also: Wenn ein Ergebnis gut passt, dann kann man die Methode so wieder reproduzieren.

Unter _Documentation_ kann man in _Notes_, _Columns_, _Method information_ wichtige Informationen über den Run bekommen und wie das System bestückt ist.

### Integration

! Entweder über Orientierung an Fraktionen. Oder, dies ausklammern und dann kann man einen Bereich markieren. Am besten bei manueller Markierung nicht in den Peak hineinschreiben. Sondern, man sollte die Baseline für den Computer zur Berechnung überlassen.

Wenn man _Align Peaks to Fraction_ herausnimmt, kann man die kleinen blauen Marker verschieben. Dann mit **Rechtsklick** und _Split_ kann man **Schultern der Peaks** teilen. Die Peaktabelle wird entsprechend angepasst.


- [ ] Extinktionskoeffizienten direkt richtig für das Protein eingeben. Dann wird die **Proteinmenge** ziemlich richtig berechnet.

- [ ] Dies als **Anhaltspunkt** für den Verlust in den Aufreinigungen oder die Wahl der nächsten Säule in Kapazität verwenden.

### Überlagerung von Peaks

- [ ] In der File-Übersicht zwei auswählen und mit Rechtsklick gemeinsam öffnen.
- [ ] Unter _Axes_ mit [X] _Zero at Phase start_ (z.B. Elution) kann man die Peaks überlagern.
- Gestrige Säule HighTrap blue (30 µm) war 1/3 so groß wie die Q Säule (90 µm). Daher konnte man Oligomerzustände besser trennen.

Bei **ÄKTA GO** vs. **ÄKTA PURE** arbeitet man nur mit einer Pumpe und ist ungenauer.


### Evaluation Classic

- [ ] _Operations_ mit _Open Curves to Compare_ kann man Kurven spiegeln, überlagern. 
- [ ] Differential, wo die Steigung des UV-Signals am höchsten ist, kann man verwenden, um eine Stufe einzufügen. Mit _Operations_ (muss x-Achse in Zeit haben) und _First Order_ Radiobutton kann man die Ableitung der Kurve überlagern. Mit dem vertikalen Marker kann man in den maximalen Wert der Ableitung gehen und mit **Conc. %B** angezeigt diesen Wert von **Conc. %B** an diesem linearen Gradienten für ein Stufenverfahren verwenden. (**Nicht** ins Retentionsmaximum.)
- [ ] _Activity histogram_ kann man z.B. für Enzyme ins Chromatogramm hinzufügen.


### Fehler welche passieren

* Im _Method Evaluator_ mit **Only show suggested** Columns kann man vorsortieren, welche Säulen für das System empfohlen sind.
  
? Driftende Basislinie in UV-Linie: **Luftblase in Flusszelle**. ! In diesem Fall einen _System Wash_ durchführen. Oder: Mit _Hold_ (☀) das System einfrieren.

? Peak kommt bei der Applikation, nicht erst in Elution. ! Dies ist entweder _Flowtrough_ oder eine _Überladung der Säule_. 

? Conductivity kommt nicht schnell auf Baseline in Equilibration zurück. Dies zeigt z.B. oft, dass man ein größeres System verwendet mit größeren Totvolumen.

? Manche Häkchen oder Funktionen im _Method Editor_ waren nicht verfügbar obwohl sehr neue Funktion. Dies kann sein, wenn z.B. der Treiber und das System nicht mehr zusammenpassen. Treiber aktualisieren.

? Druck ist sehr hoch (höher als 0.2 MPa). ! Dann zuerst den Filter tauschen. Ansonsten den Restriktor kalibrieren.

? Druck bricht ein an gewissen Stellen. ! Wenn ÄKTA ein Ventil dreht, dann könnte ÄKTA auf eine Sackgasse treffen und extrem hohen Druck aufbauen (z.B. Injektionsventil) und die ÄKTA fährt daher den Druck stark runter. 

**? Druckalarm bei Ethanol.** ! Dies ist der höheren Viskosität geschuldet. Unter _System Control_ und _System Settings_ den Fractionator Wash von 20 ml auf 10 ml herunterfahren.
