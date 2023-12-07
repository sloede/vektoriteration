# Vektoriteration und inverse Iteration

Die Vektoriteration bzw. die inverse Iteration sind numerische Verfahren zur Bestimmung von
Eigenwerten und Eigenvektoren. Dieses Repository enthält ein interaktives Pluto-Notebook mit
Anwendungsbeispielen zu den beiden Verfahren:

* [Link zum Pluto-Notebook (zum Starten in Pluto)](https://raw.githubusercontent.com/sloede/vektoriteration/main/vektoriteration.jl)
* [HTML-Vorschau im Browser](https://vektoriteration.lakemper.eu/vektoriteration.jl.html)

Das Notebook wurde als interaktives Skriptum zur Begleitung einer Vorlesung konzipiert, in der die
beiden Verfahren vorgestellt werden. Zielgruppe ist eine Vorlesung für Bachelorstudierende im 3.
Semester in einem Studium mit Mathematik-Schwerpunkt, wie z.B. Mathematik, Mathematik und
Informatik oder Computational Engineering Science.

Neueinsteiger in Julia und Pluto können im folgenden Abschnitt den Anweisungen zur Installation von
[Julia](https://julialang.org) und [Pluto](https://github.com/fonsp/Pluto.jl) folgen.

## Erste Schritte mit Julia und Pluto
Die folgende Beschreibung basiert auf
[dieser](https://computationalthinking.mit.edu/Spring21/installation/) hervorragenden Anleitung (auf
Englisch).

### Julia installieren
Um Julia zu installieren, sollte die *aktuelle stabile Version* von
[https://julialang.org/downloads/](https://julialang.org/downloads/)
heruntergeladen werden (nicht die LTS-Version, keine Vorabversionen usw.). Bei Fragen zum
Installationsprozess können die plattformspezifischen Anweisungen genutzt werden, z.B. für
[Windows](https://julialang.org/downloads/platform/#windows),
[macOS](https://julialang.org/downloads/platform/#macos) oder
[Linux](https://julialang.org/downloads/platform/#linux_and_freebsd).


### Pluto installieren
Sobald Julia installiert ist, kann die ausführbare Datei von Julia (`julia` unter Linux/macOS,
`julia.exe` unter Windows) aufgerufen werden, um die Julia-REPL zu starten. Anschließend müssen die
folgenden Befehle ausgeführt werden:
```julia
using Pkg
Pkg.add("Pluto")
```
Damit wird das Pluto-Paket installiert. Dieser Schritt ist nur einmal erforderlich, d.h., wenn
Pluto ein zweites Mal verwendet wird, kann direkt [Pluto ausgeführt werden](#pluto-ausführen).

### Pluto ausführen
Nach der Installation von Julia und Pluto kann Pluto gestartet werden, indem die Julia-REPL geöffnet
und die folgenden Befehle ausgeführt werden:
```julia
using Pluto
Pluto.run()
```
Dadurch sollte Pluto automatisch im Standardbrowser geöffnet werden. Sollte dies nicht der Fall
sein, kann der Link in der Julia-REPL, der etwa wie `http://localhost:1234/?secret=1234abcd`
aussieht, manuell im Browser geöffnet werden.

Auf der Startseite von Pluto findet sich ein Abschnitt mit dem Titel "Open a notebook". Hier kann
der Link zum Pluto-Notebook (siehe Anfang dieser Datei) hineinkopiert und durch Klicken auf "Open"
das Notebook gestartet werden.

Hinweis: Beim Öffnen eines Notebooks muss aus Sicherheitsgründen einmal oben rechts "Run notebook
code" ausgewählt werden, woraufhin der Julia-Code ausgeführt wird. Abhängig vom Notebook
kann dies einige Sekunden in Anspruch nehmen. Nachdem das Notebook vollständig geladen wurde, sollte
alles reibungslos funktionieren. Beim erstmaligen Öffnen eines Notebooks kann diese Verzögerung noch
länger sein (bis zu ca. einer Minute), da Pluto ggf. zusätzliche Julia-Pakete installieren muss.

## Autor
Dieses Repository wurde von [Michael Schlottke-Lakemper](https://lakemper.eu) initiiert.

## Lizenz
Die Inhalte dieses Repositories sind unter der MIT-Lizenz lizenziert (siehe
[LICENSE.md](LICENSE.md)).

