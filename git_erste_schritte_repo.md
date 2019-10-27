## Repository

---
### Fragen:
* Wo legt Git seine Informationen ab?


  
### Übungsziele:
* Erstelle ein lokales Git Repository

---



## Repositories anlegen
Ein neues Repository anlegen, oder eines von einer bestehenden URL herunterladen


Legt ein neues lokales Repository mit dem angegebenen Namen an

```
$ git init [project-name]
```

Klont ein Projekt und lädt seine gesamte Versionshistorie herunter

```
$ git clone [url]
```

## Änderungen vornehmen
Änderungen überprüfen und eine Commit-Transaktion anfertigen


Listet alle zum Commit bereiten neuen oder geänderten Dateien auf
```
$ git status
```

Zeigt noch nicht indizierte Dateiänderungen an
```
$ git diff
```


Indiziert den derzeitigen Stand der Datei für die Versionierung
```
$ git add [file]
```


Zeigt die Unterschiede zwischen dem Index ("staging area") und der aktuellen Dateiversion
```
$ git diff --staged
```

Nimmt die Datei vom Index, erhält jedoch ihren Inhalt
```
$ git reset [file]
```


Nimmt alle derzeit indizierten Dateien permanent in die Versionshistorie auf
```
$ git commit -m "[aussagekräftige Nachricht]"
```


