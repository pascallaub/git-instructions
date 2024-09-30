# Anleitung zur Einrichtung von Github

## 1. Wie installiere ich die Software?

Es gibt mehrere Möglichkeiten Git lokal auf dem Rechner zu installieren. Die gängigste Variante ist der Download der Installationsdatei und dessen ausführung.
Diese findet man auf der offiziellen Webseite. [Git-Website](https://git-scm.com/)

Eine andere Option ist Git direkt über den Terminal zu installieren. Dafür verwendet man den Befehl "choco install git".

## 2. Konfigurieren von Git

Danach muss mit der Git Bash die config festgelegt werden, damit uns Github auch zuordnen kann. Das wird mit dem Befehl 'git config --global user.name "Hans Wurst"' 
und 'git config --global user.email "wurst@wasser.de".
Um zu überprüfen ob die Konfigurationsdatei richtig gesetzt wurde, kann man den befehl 'git config --list' ausführen.

## 3. Erstellen eines Git-Repositorys

Wenn man sich nun mit der installierten Git-Bash in dem Verzeichnis für seine Projekte befindet, kann man ein neues Git-Repository starten, indem man den Befehl
'git init' verwendet.

## 4. Erstellen einer README.md

Durch den Befehl 'echo "# Das ist eine README-Datei" > README.md' kann eine README-Datei erstellt werden. 
Mit 'git status' lässt sich überprüfen, ob die Datei hinzugefügt wurde. 
Danach wird durch den Befehl 'git add README.md' die Datei vorbereit und mit 'git commit -m "README.md added"' dem Repository hinzugefügt. 

## 5. Verbindung zum Remote-Repository herstellen

Um eine Verbindung mit dem Remote-Repository herzustellen, wird ein SSH-Key benötigt, wie dieser eingerichtet werden kann. Kann man [hier](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) nachlesen. 
Wenn dieser Vorhanden und richtig eingerichtet ist, kann man mit dem Befehl 'git remote add origin git@github.com:test.git' die Remote-Verbindung herstellen.
Nachdem die Verbindung hergestellt wurde, kann man mit 'git clone' 
