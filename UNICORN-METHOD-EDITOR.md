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



### Für die Kursmethode

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
