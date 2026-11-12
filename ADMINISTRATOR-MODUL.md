# Administrator Modul

Man gelangt in das _Administator Modul_ über z.B. andere Module im _Home_ (linke Auswahlleiste) und _Applications_. Wenn diese grau ist, dann ist der Zugang dazu nicht gewährleistet.

- [ ] Bei Installation einer ÄKTA ist generall eine Aktivation ID, welche vergeben wird.
      ! Wenn diese Aktivation ID nicht bekannt ist, dann die MAC-Adresse der Lizens suchen.
- [ ] Log-Files können generiert werden. Dies kann nach Datum und User sortiert werden. Der Art von Log-Einträgen kann ebenso gefiltert werden mit Checkboxes.
- [ ] _My Systems_ zeigt welches System verbunden ist. Hier ist die **Seriennummer** gelistet (z.B. 3269678) auch auf der **Rückseite des Systems mit Aufkleber**. IP-System und Treiberkonfiguration.
- [ ] _My Systems_ zeigt auch die **Systemkomponenten**.
      ! Neue Komponente einbauen: Unter _Edit_ kann man Komponenten hinzufügen bzw. Ventilkomponententypen auswählen / ändern.
- [ ] Software kann **aktualisiert werden** über _Software download_ (online von Cytiva) und dann kann man über _System Properties_ und _Import_ das heruntergeladene _.zip_ File hochladen. **Während dies Treibersoftware installiert wird (blinkt viel) nicht ausschalten, sondern einfach durchlaufen lassen.**


#### Database Management und Backup

Wenn alte Methoden oder Resultate offen sind, dann kann man diese hier schließen, damit Überschreiben wieder möglich wird.

Wenn die Installation **lokal** ist, dann kann dieses Backup unter `C:\ProgamData\Cytiva\UNICORN Database\Backup` gespeichert werden. Am besten den Backup-Folder zu etwas in der Cloud ändern.

- [ ] Bei Aktualisierung Backup herunterladen. Auf neue Version.
- [ ] Nach Aktualisierung hineinladen um es zu haben.

#### Archive und Retrieve: Daten bewahren aber Speicherplatz freihalten (Deletion with Microsoft)

Archivieren des Ergebnisses: Man hat mit der neuen **Microsoft Express** (gratis Installierung mit Unicorn) nur **10 GB** Speicherplatz. Am besten von **alten Mitarbeitern** (_Free Selection_ und _Pick Result_) und alte System Logs vor einem gewissen Datum löschen.


#### Advanced Settings

- [ ] Passwörter können hier geändert werden.


## User Setup
- [ ] Nach default **User** Installation gibt es einen Admin-Benutzer.
- [ ] **Mindestens einen zweiten User mit Administratorrechten erstellen.**
- [ ] Wenn der einzige Administrator sich sonst ausloggt, kann ihn niemand zurückstellen.
      ! Einzige Alternative: Backup einspielen.
- [ ] Man kann ein _Lock Account_ einführen.

#### Access Group Properties
- [ ] Für User vs. Administrator kann man Rechte vergeben und diesen einzeln Unicorn-User zuordnen.
- [ ] Unter _Folders_ kann man neue Top-Folder hinzufügen, damit man die Methoden und Daten im Zugang limitieren kann. Es ist wahrscheinlich gut, neben _DefaultHome_ noch weitere Top-Folder einzuführen.
