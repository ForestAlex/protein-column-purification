# Service

- [ ] System muss **immer** laufen, wenn es im 4°C Kühlraum steht (**bei uns der Fall**). 
- [ ] Einmal pro Woche die Kolbenhinterspülung tauschen (50 ml 20% Ethanol).
- [ ] Einmal pro Monat den Filter im Mixer austauschen (vorfiltern der Puffer). Dafür Kappe abschrauben. Gummidichtung am Mixer lassen. Widerstand überwinden zum Aufdrehen. (Unten sitzt Rührknochen, braucht man nicht angreifen.) Man nimmt den Filter mit einer Pinzette heraus. Den runden Filter tauschen. Wenn das Gitter/Netz darunter beschädigt ist, dann dieses möglicherweise mittauschen. Mit dem Stempel evt. den Filter festdrücken. Gerade aufstellen und gerade zudrehen, damit der Rührknochen nicht beschädigt wird. (Kontrolle: Leicht schütteln und zuhören. Bei Klack-Klack-Klack ist alles okay).
- [ ] ! Wenn der Druck größer als 0.2 MPa ohne Column ist, dann ist dieser Filter verstopft.
- [ ] Bei Stromausfall **48 h** in der Raumtemperatur auftauen lassen. Und dann wieder auf **4°C** stellen.

**Tubings**


- beige = 1 mm
- grün = 0.75 mm (größerer Durchmesser, für besserer Volumentransport)
- orange = 0.50 mm (kleinerer Durchmesser, für bessere Auflösung, auch zu Fraktionator)
- blau = 0.25 mm


# Neue Konnektoren an ÄKTA anschließen

- [ ] ! System abschalten. (Alles außer Mixer hat alles elektronisch. Strom vs. Daten laufen immer über dasselbe Kabel.)
- [ ] Auf der Rückseite _Uninet_ Konnektoren. (grau = _firewire_ F9R, schwarz = _größer_). Wenn nichts angeschlossen ist, dann ist **Terminatorwiderstand** als Platzhalter dort. In der Box aufbewahren, wenn Komponente angesteckt wird.
- [ ] Auf dem Bauteil befindet 
- [ ] Bei 4°C Kühlraum kann man das System für max. **15 min.** (Risiko: Kondenswasser) abschalten.


# 0. Tubing und Verbindungen

Tubing nicht mit Werkzeugen festziehen. Kapillaren 1-2 mm abschneiden von dem Tubing. Wenn die _fingertight connectoren_ sich gar nicht mehr bewegen, sollte man diese austauchen.

! Bei _fingertight connections_ den Schlauch beim Hineinschrauben hineinstecken. Danach mit leichtem Gegenzug testen.

! Nicht mit Werkzeugen bei Undichtheiten festziehen. Nur öffnen mit Werkzeugen. Bei Undichtheiten liegt es an den Komponenten.

! Tubing mit der **glatten** und nicht der **schrägen** Seite des Kapillarcutters abschneiden (Orientierung für Klinge an Pfeil).

Auf manchen Komponenten befinden sich RFD-Chips. Mixer kann man z.B. tauschen bei 1-10 ml/min (1.4 ml Mixer gut). Bei 20-25 ml/min (5 ml Mixer).


# 1. Probeneinlass

Luftsensor (_Air Sensor_) um zu verhindern. 


# 2. Puffereinlass (kommen vor Pumpen, schwarz)

Man hat meist zwei Puffer. (Beispielsweise 7x Inlet Valve A, 7x Inlet Valve B). Dies erlaubt bis zu 7 verschiedene Puffer zu verwenden. Wenn in den _Invlet Valves_ die schwarzen Plättchen weggenommen werden, gibt es einen _Air Sensor_. Manchmal gibt es auch 2x A, 2x B Kombi-Ventile (aber es ist kein _Air Sensor_ verbaut).

# 3. Pumpen (silberfarben)

Jede Pumpe besteht aus 2x silberfarbenen Pumpenköpfen, damit es zu keinem pulsierenden Fluss kommt. Das funktioniert so: Ein Kolben füllt sich mit Puffer, der zweite Kolben drückt in das System und dann gegengleich. 

! WICHTIG: Über den Pumpenköpfen sitzt das Flügelventil für die Entlüftung. Hier setzt man mit der Spritze an, bis keine Luft mehr kommt. Kolben läuft ansonsten leer durch. 

! WICHTIG: ÄKTA bestimmt über die Pumpenläufe wieviel Volumen "durchgelaufen" ist. Wenn die Pumpe leerläuft, ist das Volumen am Bildschirm nicht mehr richtig.

? ANZEICHEN FÜR LUFT: Unruhige Drucklinie (Schwankungen, kleines periodisches Pattern).


# 4. Pressure Monitor (schwarzes Manifold)

Hat Rückschlagmodule verbaut, um den Puffer nicht passiv durchlaufen zu lassen. Hier sitzt der **System Pressure Monitor**. Hier wird der **Fluss der beiden Pumpen** das erste mal kombiniert. Hier wird der **Gradient gebildet** (abhängig von %B). T-Stück mixt.

# 5. Ethanolbehälter

20%iges Ethanol (ca. 40 ml) muss vorhanden sein. (Schlauch herausnehmen und beim Waschen am Anfang schauen, dass etwas gut tropft.) Damit ist die Zirkulation gewährleistet. Diese Zirkulation über Kolben in der Spülung muss gewährleistet werden, damit Puffer aus Niederdruckbereich in Ethanol transferiert wird und sich alle Sachen lösen.

? ANZEICHEN FÜR PROBLEM: Wenn die Pumpe leerläuft (Hochsalzpuffer) durch Hochdruckdichtung. Puffer von Hochdruckbereich in Niederdruckbereich. Reservoir läuft über (Hochdruckdichtungen passen nicht).

# 6. Mixer (Online/Inline Filter)

Mixer hilft nach dem Pressure Monitor dem T-Stück extra hinzu, um einen sauber gemischten Gradienten zu gewährleisten. Mixer beinhaltet einen Filter und einen Mischknochen und dies kann umgangen werden (Mixer aber am System montiert lassen, sonst gibt es ein Problem). Als Alternative kann man ein _Mixerventil-Umleitung_ machen.

# (Ausgangsventil)

# 7. Injektionsventil

Probe kann über **Injektionsloop**, **Superloop** oder **Probenpumpe** geladen werden. 

* Bei einer Probenpumpe gibt es den _Sample Pump_ (V9IS Probeneinlassventil) mit S1-S7 für verschiedene Proben und Puffer und Air-Sensor. 
* Bei einem Kapillarloop kann es einen _Loop Valve_ geben. Meistens nur für kleinere, oder mehrere, Proben.

# 8. Säule

Pre-column pressure Monitor.

! Prüfen, ob man die richtigen Drücke für die Säule eingestellt hat.
! Prüfen, ob man in _upflow_ oder in _downflow_ arbeitet.

**Reinigung erfolgt immer im Upflow.** (Damit können die Unreinheiten am besten gewaschen werden.)

# 9. UV-Detektor

U9-D Detektor für 190 nm - 700 nm in 1 nm Schritten einstellbar mit einer Xenon-Blitzlampe. Sobald das System eingeschaltet wird, aktiviert sich der Detektor.

U9-T Detektor mit LED (für **T**-win Detektor bei 260 nm und 280 nm). Man kann in der Software 260/280 Verhältnis einstellen für Protein vs. DNA/RNA.

U9-L Detektor mit LED (misst nur 280 nm).

# 10. Conductivity (Leitfähigkeitssensor)

Sehr stabil, kaum Notwendigkeit für Kalibrierung. Mit einem schwarzen Ring: **Flow Restriktor**. Der Flow Restrictor sitzt hinter den Detektormodulen und versucht zu verhindern bei Entgasung des Puffers die Probe und hält den Druck nach der Säule auf **ungleich 0** (er hält +0.2 MPa nach der Säule).

! ENTGASUNG: Nach der Säule sollte sich der Druck nicht auf 0 absenken. Der Flow Restriktor garantiert einen Gegendruck, damit nachher nicht der Puffer plötzlich entgast.

# 11. pH Valve 

pH-Elektrode muss kalibriert werden und muss angeschlossen werden unter Anschluss _pH-valve_.

! Lagerung der pH-Elektrode (white dummy) sollte außerhalb der ÄKTA gesammelt werden, da ansonsten die Buffer in die pH-Elektrodenwände schlecht einwandern.

# 12. Outlet valve

Der _Flow-Through_ sollte sammelbar sein, das _Peak-to-Loop_ kann extra eingefügt werden mit einem 10-Positionen Auslassventil. Normal:

* OUT 1 = für Fraktionssammler
* WASTE

# 13. Fractionator F9R Karussel

! Tubing auf die richtige Länge mit dem _Tube Adjustment_ Tiefloch am Arm einstellen. Aufschrauben des _fingertight connectors_ und dann auf richtige Tiefe einstellen, und dann wieder schwarz am Connector zuschrauben.

Für Drehung: den Arm auf die Seite drehen. Danach den schwarzen Knob auf der Seite mitöffnen bei Bewegung des Karussels.

Für Einstellung des Arms: Höhe einstellen und _tube fit sensor_ gut einstellen. (Wenn dies nicht der Fall ist, dann ist der Sensor evt. kaputt. Dann mit hoher Prozentigkeit an Isopropanol waschen des Sensors bevor man ihn nachbestellt.)

# 14. Fractionator F9C mit dem Plattensensor

Die Plattenadaptoren werden automatisch erkannt. Die Kamera macht sogar bei 96-well Platten noch extra ein Foto, um sich den Plattentyp zu lernen. Weiße Abdeckung am Arm entfernen. Mit dünnem Seidenpapier (wie bei NanoDrop) mit Ethanol reinigen. Kamera und _Drop Sync_ Sensor reinigen.

# Möglich: Versatile valve

* Beispielsweise verschiedene Säulen einschalten.
* Beispielsweise verschiedene Detektoren zwischenschalten.
