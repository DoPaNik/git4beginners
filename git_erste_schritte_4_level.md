## 4 Level

---
### Fragen:
* Wie kann ich Änderungen in Git aufzeichnen?
* Wie kann ich den Status meines Repository überprüfen?
* Wie kann ich kennzeichnen, welche Änderungen ich vorgenommen habe und warum?
  
### Übungsziele:
* Überführe eine oder mehrere Dateien durch die 4 Level (Create/Modify-Add-Commit-Zyklus)

* Erkläre wo in jeder Phase dieses Zyklus Informationen gespeichert sind

* Unterscheide zwischen deskriptiven und nichtdeskriptiven Commit-Meldungen.

---





### Working Directory
Erstellen einer neuen Datei
```
$ touch test.txt
```


###  Index / Staging Area

Lege die Datei auf den Stage
```
$ git add test.txt
```

### Repository
Erstelle deine erste Revision
```
$ git commit -m "Mein erster Commit" 
```
### Remote Repsoitory
Veröffentliche deinen aktuellen Stand
```
$ git push origin master
```