# Säulen reinigen

## SEC Säulen

- [ ] Man kann die Säulen locker länger als Ablaufdatum verwenden.
- [ ] REGELMÄSSIG REINIGEN.
- [ ] Wenn der Fluss kaum mehr läuft (fast zu spät): Nun mit **kleinen Volumen** NaOH reinigen (aus dem Kapillarloop).

## Column Performance Test
- [ ] _Method Editor_ öffnen.
- [ ] Isokratische Methode: 1-2 CV einer Lösung mit einem kleinen **Testmolekül**.
- [ ] z.B. Aceton (2%) in Wasser
- [ ] z.B. NaCl (0.8 M) als Tracer in 0.4 M NaCl damit die Säule nicht komplett von 0.8 M als Front getroffen wird
- [ ] _Column Performance Test_ auswählen
- [ ] unter _Manual loop filling_ mit einem Kapillarloop
- [ ] _Column Position_ einfüllen und Flussrichtunng

Nun weitergehen in das **Evaluation Module**.

Auswerten der Integration mit verschiedenen Parametern.

- [ ] **Asymmetrie**: zwischen 0.8-1.2 in Ordnung. Bei höherer Asymmetrie (wenn sie gepackt ist, dann nachpacken) oder bei vorgepackten Säulen **reinigen**. Dies bedeutet, dass die oberen Partikel verdeckt und nicht zugänglich sind und Moleküle einen "Umweg suchen müssen" und später kommen. Waschen.
- [ ] **Asymmetrie am Anfang**: Dies bedeutet es gibt "Abkürzungen" manche kommen zu früh. Dies indiziert Risse (schwer handzuhaben) oder Luft (Säule verkehrt herum einhängen und versuchen, die Luft herauszuwaschen).
- [ ] **Plates/m** im Column: Wieviele Trennstufen hat die Säule? Je mehr, desto besser. (ca. 35k für SEC Column)
- [ ] **Plattenhöhe**: Je weniger hoch die Platte, desto besser.
- [ ] **Reduzierte Plattenhöhe**: Plattenhöhe dividiert pro Partikeldurchmesser. Wieviele Partikel braucht man um eine Trennebene aufzubauen? Ideal: **1-2** Partikel für Ebene. Wenn es eine Größenverteilung gibt, braucht es **2+** Partikel. **3-5** ist für hochauflösende Säulen akzeptabel.

## Welche Puffer zum Waschen?

- [ ] Auf Cytiva Produktseite gehen.
- [ ] Unter _Documents_ der Säulen das Dokument für **Maintenance and Cleaning of Columns** unter _Instructions for use_.

! Wichtig: **Chemical Stability**, **Flussratenvorgaben**, **Drücke** einhalten.

## Column Logbuch

- [ ] _Column Handling_ und oben im Fenster auf dem Tab _Column Logbook_ die **Column ID** erstellen.
- [ ] Dadurch Säulen anlegen und dann bei dem Start der Methode diese Säule auswählen (z.B. max. Druck, num. of run since cleaning, etc.)
- [ ] Erinnerung setzen für **nach 10 Läufen ist Reinigung notwendig**.

## Benutzerdefinierte Säule
- [ ] In _Method Editor_ unter _Column Handling_ (Symbol mit den Säulen im Header) mit _New_ mit _Technique_ und _Resin Type_ einfüllen in einen gewissen _Säulentyp_.
- [ ] Cytiva überschlägt die Säulenparameter grob. 
- [ ] Die Säulenhöhe entspricht der notwendigen Bindungskapazität.
- [ ] Bei welchem Druck wurde die Säule gepackt?
- [ ] **Säulenpacken: Kurs von Cytiva in München.**
