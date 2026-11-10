# protein-column-purification

An ÄKTA protocol and method introduction.

(Roland Viertlmayr)

## Vor der Chromatographie

- [ ] Basisparameter des Proteins kennen: `pI, Exc. Coeff., MW (molecular weight)`
  * für BSA: MW = 69.3 kDa, pI = 5.82, Exc. Coeff. (0.1%) 280 nm: 0.72 ml/mg cm (beispielsweise über ProtParam)
- [ ] Möglichkeit der Reinigung erkennen

## Möglichkeiten der Chromatografie
* **IEX** (Ion Exchange Chromatography): Große und schnelle Beads vs. kleine hochauflösende Beads (z.B. für Isoformen)
* **HIC** (Hydrophobic Interaction Chromatography): über starke Salzlösung wird das Protein aus seiner Hydrathülle gelöst und kann dann mit dem Säulenmaterial interagieren
* **SEC** (Size Exclusion Chromatography): Auftrennung über Aufhaltszeit in Säule (kleine Proteine kommen später)
* **AC** (Affinity Chromatography): Protein bereits mit speziellem Tag hergestellt.

- [X] siehe auch Abbildungsdokument in Abb. 1

### IEX (Abb. 2)
* Der isoelektrische Punkt (pI) bestimmt, wann das Protein keine Ladung hat.
* ! Der pH-Wert sollte nie der pI sein, da das Protein sonst aggregiert.
* pH über pI (pH > pI): Protein hat eine negative Ladung.
* pH unter pI (pH < pI): Protein hat eine positive Ladung.
* Die Säule hat nun eine gegenteilige Ladung.
* Elution folgt mit steigender Salzkonzentration ➡️ Die Ionen verdrängen das Protein im Gradienten von der Säule ab einem bestimmten Punkt.

### HIC (Abb. 3)
* ! Nicht zu hohe Salzkonzentration (nicht exzessiv) sonst fällt Protein aus.
* Zuerst löst man in einer hohen Salzkonzentration und nimmt dem Protein die Hydrathülle weg (bindet an Säule).
* Nun löst man mit einem Gradienten immer schwächerer Ionenkonzentration und gibt dem Protein die lösliche Hydrathülle zurück.
* Das Protein löst sich von der Säule.

### SEC (Abb. 4)
* Benötigt nur einen Puffer die ganze Zeit (_isocratic technique_).
* Das Säulenmaterial besteht aus Poren von klein bis groß. Die großen Proteine diffundieren nicht in die Poren und waschen schnell durch. Die kleinen kommen erst später heraus.
* ! Je nach Säule bestimmen sich unterschiedliche Cutoff (kDa) Größen.

### AC
* Poly-His-Tag: Nickel oder Cobalt auf der Säule (eluiert mit Imidazol)
* MBP-Tag: Maltose-binding-tag (mit Maltose auf der Säule)
* Antigen-Antibody: Antibody auf der Säule
* Step-Tag: Streptavidin auf der Säule

## CiPP = Capture, intermediate Purification, Polishing
- [ ] frühe Schritte: Extraktion und Vorbereitung
- [ ] schneller Schritt: frühe Capture und schnelle Trennung von Proteasen
- [ ] letze Schritte: Aufreinigung
- peak-to-loop Elution kann helfen, um weniger Protein in Schritten zu verlieren
