## Branching
Benennen von Commit-Serien und Zusammenfassen erledigter Tasks


Listet alle lokalen Branches im aktuellen Repository auf
```
$ git branch
```

Erzeugt einen neuen Branch
```
$ git branch [branch-name]
```


Wechselt auf den angegebenen Branch und aktualisiert das Arbeitsverzeichnis
```
$ git checkout [branch-name]
```


Fasst die Historie des angegeben Branches mit der des aktuell ausgecheckten Branches zusammen
```
$ git merge [branch-name]
```


Löscht den angegebenen Branch
```
$ git branch -d [branch-name]
```


## Verschieben und Löschen versionierter Dateien


Löscht die Datei aus dem Arbeitsverzeichnis und indiziert diese Löschung
```
$ git rm [file]
```



Entfernt die Datei aus der Versionskontrolle, behält sie jedoch lokal
```
$ git rm --cached [file]
```


Ändert den Namen der Datei und bereitet diese für den Commit vor
```
$ git mv [file-original] [file-renamed]
```


## Tracking
Temporäre Dateien und Pfade ausschließen


Eine Textdatei namens `.gitignore` verhindert das versehentliche Committen von Dateien und Pfaden mit den spezifizierten Patterns
```
*.log
build/
temp-*
```


Listet alle innerhalb dieses Projekts ignorierten Dateien auf
```
$ git ls-files --others --ignored --exclude-standard
```


