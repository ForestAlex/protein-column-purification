# protein-column-purification

An ÄKTA protocol and method introduction.

(Roland Viertlmayr)

----------------------------
Learnings:
* use a 20-40 mM imidazole buffer for washing, only use 1x IMAC
* use Option 1: Size Exclusion (SEC) and then pool fractions
* use Option 2: IEX and then pool fractions (proteins will likely separate)
* use a 3-wavelength detector where you can monitor 3-wavelengths at the same time


----------------------------

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

(vgl. Abb. 7): IEX immer, HIC nur für Polishing, SEC nur für Polishing, AC nur für Capture


### Performance Parameters 
**CSRR**: Capacity, Speed, Resolution, Recovery
! Man kann nur 2 pro Schritt machen.
- Capture: Speed + Capacity (beispielsweise His-FF, HIC Sepharose-FF) 1x Reinigung
- Polishing: Capacity + Resolution (beispielsweise HIC Sepharose-FF) 2x Reinigung von anderen Proteinen
- Polishing: Resolution + Recovery (beispielszweise SEC, IEC mit sehr flachem Gradient, -P vs. +P nur 1 Phosphorylierung) 3x Reinigung oft nur von anderen Isoformen

## Chromatografie: Allgemeine Vorbereitung
1. Equilibration of Column (to Sample Conditions)
2. Sample Application
3. Wash
4. Elution
5. Equilibration of Column (to Storage Solution)

**Entscheidung für Aufreinigungsschritte**

(vgl. Abb. 8): 1-Schritt (>80%), 2-Schritt (>95%), 3-Schritt Aufreinigung (>99%)

- [ ] 1-Schritt: AC + Dialyse + Aufkonzentration
- [ ] 2-Schritt: AC + (Dialyse) + SEC + Aufkonzentration
- [ ] 3-Schritt: AC + IEX + (Dialyse) + SEC + Aufkonzentration

z.B. AC HisTrap FF (90 µm), AIEX Resource Q 7.6 pH (linear gradient), SEC 75 10/300 GL

### Auswahl der Säule
- FF = fast flow (90 µm) hohe Flussraten und schlechte Auftrennung
- HP = high performance (34 µm) Trennung der beiden Peaks (aber UV-Signal in rot zeigt, das Protein immer noch in Shoulder)
- Resouce S (15 µm, alle Partikel gleich groß)
- Mini S (3 µm, alle Partikel gleich groß)

(vgl. Abb. 9): rotes UV-Signal des Targetproteins vs. allgemeines UV-Signal welches die Säule zu trennen schafft

_Manual protein purification and tools for process development_ (mit Zentrifuge bis zu 96x verschiedene Puffer)
