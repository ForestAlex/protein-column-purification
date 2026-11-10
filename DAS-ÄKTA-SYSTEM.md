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
