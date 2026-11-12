# Unicorn System Control

- [ ] Lagerlösung bei +1 Tage: 1x in Wasser, 1x 20% in Ethanol zurückspülen
- [ ] nach Lagerlösung zurück in Pufferbedingung:
  1. [ ] Tubings in neue Lösung transferieren
  2. [ ] Pump-Wash in Wasser (Inlets spülen)
  3. [ ] System entlüften
  4. [ ] Pump-Wash für die neuen Lösungen (Makro für Inlet, dient den Ethanol aus den Tubings herauszuspülen, spült bei 20 ml/min)
        * **Pump-Wash** endet immer am Injectionsventil.
        * **System-Wash** könnte das ganze System durchspülen.
  5. [ ] Column-Handling unter _Column Type Parameters_
  6. [ ] Druckalarm einstellen (_Pre Column Pressure_ dem _Delta_ anpassen bei nur einem Drucksensor)
  7. [ ] Programm schreiben
         * _Pre column_
         * _Delta column_
         * _Inlet A A1_
         * _Injection valve Manual load_
         * _Column position 1_
         * _Outlet valve [ Waste/Fractionator ]_
         * _System flow_
         * _Other_ (Timer)
  8. [ ] Nach Waschen, pausieren (⏸), Säule anschließen, starten
  9. [ ] Nach Equilibration, Loop anschließen

! Bei **STOP** (⏹) werden alle Ventile und Druckalarme zurückgesetzt.

! Bei **PAUSE** (⏸) bleiben die Ventile und Druckalarme wie in der Methode, der Run wird nicht zwischengespeichert.

`Manche Einstellungen (System Settings): z.B. Waschgeschwindigkeit des Fractionssammlers (zum Abschalten) oder Cassette configuration sowie System High Pressure (wenn man mit hochauflösenden Säulen arbeitet) anpassen. Für den Probensammler kann man Akkumulator vs. Drop Sync.`

### Log file

Alles bekommt ein Log-File, dabei bekommen die meisten Kommandos zwei Einträge (_Issued_ und _Completed_). 

### Process Picture

Erlaubt Interaktion. Es gibt Interaktionsmöglichkeiten soweit das Bauteil interaktiv ist. Mit _Rechtsklick_ und _Detailed Picture_ kann man die Einzelbilder aller Schaltungen anschauen (Abb. 11, 12).  

## System vorbereiten

Längere Zeit für das System (z.B. Fr-Mo) muss das System in 1x in Wasser, 1x 20% in Ethanol lagern. Um den **Pump Wash** auszulösen kann man im _Process Picture_ auswählen. 

## Anstatt des _Process Pictures_ kann man auch _Manual_ und _Set Manual Instructions_ auswählen.
* Pumps
* Flow paths
* Monitors: **UV detectors**
* Alarms: **Pre column pressure**

Ausführen über _Insert_ → _Execute_. Dann fängt das System an zu laufen.

## System Wash

Wäscht das System in genau der bestimmten Konzentration an %B. Es schaltet die Column immer automatisch in _Bypass_. Wenn ein Fractionator verwendet wird, hilft ein _Akkumulator Wash_ (siehe im _Method Editor_) und die Schläuche des Fractionators müssen in einen Abfall füllen.

## Druckalarm

? Volumen an der Säule verloren mit oberem Spalt zeigt, dass Säule Überdruck erfahren hat. Meistens müsste man die Säule dann neu packen.

Säulenparameter in _Column Type Parameters_ anschauen. 
* typical laoding range
* typical peak width at base
* max. pre-column pressure (Säule selber hält dies aus)
* max. delta column pressure (Material innerhalb der Säule hält dies aus)

Im _Process Picture_ die _Pressure Alarms_ auf _Pre Column Pressure_ und _Max. Delta Column Pressure_ angeben. Ab Unicorn 7.10 können die Columnparameter direkt eingestellt werden. 

# Pumpe entlüften

! Wichtig. Aufpassen, dass man nicht zu viel das Ventil öffnet. Bei zu viel öffnen, zieht man Umgebungsluft. Bei zu wenig öffnen "zieht" man und "entgast" man den Puffer. Normalerweise mit stillstehendem System arbeiten. Später idealerweise bei laufenden Pumpen entlüften.

! Entlüften testen/üben über: Ventil zulassen. Spritze anstecken. Ziehen, bis die Pumpe "stark gegenzieht". Nun Ventil öffnen bis "


# System Preparation
- [ ] Tubes transferrieren
- [ ] für jede Lösung einen _Pump Wash_ (Wasser, 20% EtOH)
- [ ] Lösungen nachher für Puffer tauschen (Binding Buffer, Elution Buffer)
- [ ] für jeden Puffer einen _Pump Wash_ (! zuerst Elution, dann Binding Wash, damit das System in Binding fertig vorliegt)
- [ ] Pumpen entlüften (20 ml Spritze über silberfarbenem Pumpenkopf an das schwarze Purge-Ventil anstecken, den Schlauch braucht es nicht) bis nach Öffnen des schwarzen Ventils keine Luft mehr in die Spritze fließt. Für alle Pumpenköpfe wiederholen.

## Loop anschließen
- [ ] 500 µl Kapillarloop von _E → F_ anschließen.
- [ ] Spritze anschließen mit Bindungspuffer.
- [ ] Durch Spritze Kapillarloop mit mehreren Volumen Bindungspuffer anschließen.
- [ ] Spritze zu Spritze mit Probe rasch tauschen. Durch Probenspritze den Kapillarloop laden. **Spritze nun dranstecken lassen, ansonsten hat man ein offenes System zu dem Waste.**

## Superloop
- [ ] benötigt den **System Pressure** Alarm (der Superloop befindet sich vor der Column, würde ansonsten den Pre-Column Pressure nicht fühlen und zerbrechen).
- [ ] oben (E) und unten (F = fill) anschließen an das Ventil
- [ ] mit einer Spritze das Volumen in den Loop spülen (movable seal)
- [ ] mit dem _Inject_ Volumenfluss die Probe ausspülen (mehr Volumen kann ausgespült werden)


## Säule

Säule braucht _female-female Union_ Adapter. Wir geben von **1B** zu **2A**.

Rote Connectoren: für weichere Säulen (wenn diese auch rot sind)

Schwarze Connectoren: ältere Connectoren, härteres Material

