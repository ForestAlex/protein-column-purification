# Unicorn Method Editor

- [ ] 1. System, für welches man die Methode programmieren möchte, auswählen.
- [ ] 2a. Vordefinierte Methode auswählen. Automatisch: _Unicorn lädt Schritte und reiht sie aneinander._
      * Interessant ist die **Phase Library**.
- [ ] 2b. Wichtig! Methodenschritte können mit Rechtsklick umbenannt werden. Dies hilft sehr speziell später im _Evaluation Module_.
- [ ] 3. Column, Flow Rate, Monitor Settings einstellen (möglich: enable pH monitoring)
- [ ] 4. Fractionation Setting (**Vorschlag: über ein gemeinsames Outlet-Valve größere Volumen sammeln**
- [ ] 5. Waschen Settings
- [ ] 6. Elution Settings
     * Für eine Stufenelution mit Upflow gut.
     * Bei linearem Gradienten nie mit Upflow. Immer Säule im Downflow spülen.
- [ ] 7. Fraktionen Settings
      ! bei F9T (haben wir nicht) muss man vordefinieren, welche Platte man verwendet
      ! Größe der Fractionation: In _Column Handling_ im _System Control_ nach **halber Peakgröße** einstellen (z.B. Peakwidth = 3 ml, Fraktionsgröße = 1.5 ml).
- [ ] 8. Reequilibration von Column
      ! _Fill the system with the selected buffer._ (A1)
      ! _Fill the system with the selected buffer._ (A2) mit Wasser
      ! _Fill the system with the selected buffer._ (B2) mit EtOH
      ! Mit ✔️ **Accumulator** wird auch ein _Fractionator Wash_ gestartet.
- [ ] 9. Nun sollte die Säule und das System von Elution zu Bindung zu Wasser zu Ethanol durchgeführt worden sein.
- [ ] 10. _File_ → _Save as_
- [ ] 11. Nun kann man in die _System Control_ und über _File_ → _Open_ und dann **Result directory** auswählen.  


### Miscellaneous phase

Eine frei verfügbare Phase, welche hilft Erinnerungen einzufügen. Beispielsweise:
- [ ] **Message** und **Pause after message** hilft Erinnerungen einzufügen.
- [ ] **New chromatogram** hilft z.B. für _Elution_ ein eigenes Chromatogramm zu machen. Dies wird in ein Ergebnisfile zusammengefügt, aber mit drei Chromatogrammen. Bei sehr langen Läufen hilft dies keine Datenpunkte zu löschen (Unicorn macht das in Chromatogrammen automatisch aufgrund von Speicherplatz.)

### Für die Kursmethode Teil 1

* Affinity Chromatography
* HiTrap Blue HP, 1 ml
* Column Position = 1
* **Flow Rate = 1 ml/min.** (Standard-Flow-Rate)
* Monitor Settings (280 nm)
* keine Fraktionen sammeln
* kein System Wash notwendig
* 20 CV waschen (sehr konservativ **20 CV**)
* Elution mit **Step with fill** (stärkerer Gradient, da durch vorspülen keine Mischung im System) mit 5 CV (eluieren mit **5 CV**)
* nun Fraktionen sammeln in 96 deep well plate mit _Fixed volume fractionation_ mit **1.5 ml** mit _Stop Fractionation at the end of this phase_

### Für die Kursmethode Teil 2 (mit Scouting)

* Anion Exchange Chromatography (AIEX)
* HiTrap Capto Q, 1 ml (Druck, Fluss, **Position**)
* Linearen Gradienten zuerst mit höherer Salzkonzentration in B
* _Column Wash_ Schritt mit Puffer A1
* 280 nm, CV, ml/min. (Air Sensoren für Puffereingänge einschalten, bei Probenpumpe darf kein Häkchen sein damit der nächste Schritt getriggert wird: es würde Stoppen)
     * _control the flow to avoid overpressure_ Häkchen kann man klicken
     * _reduce for cold room_ verringert Flussrate auf 50%
* Equilibration: A1 _System Wash_, Säule **5 CV**, _Reset UV Sensor_
* (Optional: Sample Application: _Inject all sample using air sensor_ und _Finalize sample injection_ und dieser Puffer kommt aus dem **Buffer** des neuen _Sample Application_ Ventils anstatt aus A1 automatisch, daher Tubing diese Puffers **in dieselbe Flasche wie A1** geben. Mit _Prime sample inlet with X ml_ kann man das Anfangstotvolumen verwerfen. Damit unterscheidet sich der **1.** Lauf nicht von folgenden Läufen.)
* Waschen: bei Anionenaustausch ist das Produkt weniger schmutzig, daher nur **5 CV**
* Elution: _linear_ mit **20 CV**
     * **Fractionation**: Wir wollen diesmal **per Peak** fraktionieren (automatische Detektion). 96 deep well plate mit _Peak fractionation volume_ mit Maximalvolumen auffüllen (z.B. 2.2 ml) um den hoffentlich vollständigen Peak hineinlaufen zu lassen (vgl. mit _peak width at base_).
     * **Peak fractionation setting**: _Set level_ und _End level_ einstellen auf 5 mAu und 10 mAu und dann schaut die Säule auch in der Datenbank und wartet ein Minimum von 0.38 min. ab bevor es den Peak wieder beenden kann
* **Startprotokoll hinzufügen**
* **Questions** einstellen
 
### In System Control werden beim Öffnen verschiedene Einblicke angezeigt
* _Variable List_ (Scouting Variables und feste Variablen bleiben grau)
* _Scouting_ Variablen kann man teilweise verändern
* _Calibration_
* _Result Name and Location_
* _Questions_


## System CIP (= Clean in Place)

Diese Protokollvorlage besteht aus unterschiedlichen Phasen. Normalerweise: **Wasser**, **1 M NaOH**, **0.1 NaCl oder Wasser**, **Buffer** (oder 20% Ethanol). Das System spült mit 10 ml/min. für 20 ml per Position des Inlets. Auswahl aller verschiedener Positionen pro Phase. (Für jede Phase wird gewartet bis die Schläuche gespült und dann von uns transferriert werden. Dann macht die ÄKTA weiter.)

## SEC CIP

Man kann die Säule auswählen. Verschiedene Waschlösungen werden dann hinzugefügt. **Hier die Inlets anpassen.** Gewaschen wird in **upflow** bei Isopropanol wird die _Flow Rate_ reduziert. Nur die _Storage Solution_ wird in **downflow** gewaschen. 

## Methodenschleife

Scouting = innerhalb von einer Methode Parameter ändern

Methodenschleife = Methoden so programmieren, dass sich diese aneinanderreihen können (beispielsweise über Peakfraktionierung über Auslassventil)

- [ ] _File_ und _New Method Queue_ (bis zu **3 Systeme** können aneinander gehängt werden)
- [ ] Zuerst einmal ein System.
- [ ] Dann Methode **1** auswählen.
- [ ] Dann Methode **2** auswählen. Die _Start Condition_ kann _immediately_ oder _at ready command_ ausgewählt werden. (Das _ready command_ kommt dann von der ersten Methode.)
       
