# Git Konfigurieren
---
### Fragen:
* Wie muss ich Git konfigurieren um arbeiten zu können?
  
### Übungsziele:
* Konfiguriere Git zum ersten Mal auf deinem Computer
* Verstehe die Bedeutung von `--global` beim Konfigurieren

---

Wenn wir Git zum ersten Mal auf einem neuen Computer verwenden, müssen wir ein paar Dinge konfigurieren. Nachfolgend findest Du einige Beispiele für Konfigurationen, die wir beim Start mit Git festlegen müssen, bevor es losgeht:

* unseren Namen und unsere E-Mail-Adresse
* welches unser preferierte Editor ist
* und diese Einstellungen möchten wir gerne für jedes Projekt hinterlegen

Git Kommandos sind wie folgt aufgebaut:
`git <verb> <optionen>`




## Git konfigurieren

### Benutzerinformationen
Konfigurieren von Benutzerinformationen für alle lokalen Repositories

```
$ git config --global user.name "[name]"
```

Setzt den Namen, den du an deine Commit-Transaktionen hängen willst


```
$ git config --global user.email "[email address]"
```

Setzt die Emailadresse, die du an deine Commit-Transaktionen hängen willst

### Line Endings

Du kannst die Art und Weise, wie Git Zeilenenden erkennt und kodiert, mit dem Befehl `core.autocrlf` in der Git-Konfiguration ändern. Die folgenden Einstellungen werden empfohlen:

##### Linux/MacOS
```
$ git config --global core.autocrlf input
```


##### Windows
```
$ git config --global core.autocrlf true
```


### Editors


|Editor         |                           Kommando                                  |
|---------------|---------------------------------------------------------------------|
|Atom           |	`$ git config --global core.editor "atom --wait"`                 |
|nano           |	`$ git config --global core.editor "nano -w"`                     |
|VS Code        |	`$ git config --global core.editor "code --wait"`                 |



### Proxy

In einigen Netzwerken kann es sein, dass Du einen Proxy verwenden musst. Wenn dies der Fall ist, musst Du Git möglicherweise auch Infos über den Proxy mitteilen:

##### Proxy aktivieren
```
$ git config --global http.proxy proxy-url
$ git config --global https.proxy proxy-url
```

##### Proxy deaktvieren
```
$ git config --global --unset http.proxy
$ git config --global --unset https.proxy
```

### Konfiguration prüfen

Die Befehle, die wir gerade oben ausgeführt haben, müssen nur einmal ausgeführt werden: Das Flag '--global' weist Git an, die Einstellungen für jedes Projekt, in deinem Benutzerkonto, auf diesem Computer zu verwenden!

Du kannst deine Einstellungen jederzeit überprüfen indem Du folgenden Befehl aufrufst:

```
$ git config --list
```

