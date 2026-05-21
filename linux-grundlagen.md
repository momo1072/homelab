# 🐧 Linux Grundlagen

Gelernt während der FISI-Ausbildung — direkt auf dem Raspberry Pi 400 geübt.

## 📁 Navigation

| Befehl | Funktion | Beispiel |
|---|---|---|
| `pwd` | Aktuellen Ordner anzeigen | `pwd` → `/home/homeles82` |
| `ls` | Dateien anzeigen | `ls` |
| `ls -la` | Detaillierte Ansicht mit Berechtigungen | `ls -la` |
| `cd` | Ordner wechseln | `cd monitoring` |
| `cd ~` | Zurück zum Home-Ordner | `cd ~` |

## 📄 Dateien verwalten

| Befehl | Funktion | Beispiel |
|---|---|---|
| `mkdir` | Ordner erstellen | `mkdir projekte` |
| `cat` | Datei lesen | `cat docker-compose.yml` |
| `echo` | Text in Datei schreiben | `echo "Hallo" > datei.txt` |
| `cp` | Datei kopieren | `cp datei.txt projekte/` |
| `mv` | Verschieben/Umbenennen | `mv alt.txt neu.txt` |
| `rm` | Löschen (kein Papierkorb!) | `rm datei.txt` |

## 🔐 Berechtigungen

| Befehl | Funktion | Beispiel |
|---|---|---|
| `chmod` | Berechtigungen ändern | `chmod 644 datei.txt` |
| `chown` | Besitzer ändern | `chown homeles82 datei.txt` |



### Berechtigungen verstehen

|     |      |
|----|--------|
|  d- | Datei, Ordner |
| rw- | Besitzer (rw=lesen+schreiben) |
| r-- | Andere (r=lesen) |
| r-- | Gruppe (r=lesen) |





### Wichtige chmod Werte

| Zahl | Buchstaben | Wann benutzen |
|---|---|---|
| 777 | rwxrwxrwx | Nie! Unsicher |
| 755 | rwxr-xr-x | Ordner |
| 644 | rw-r--r-- | Normale Dateien |
| 600 | rw------- | Private Dateien (SSH-Keys) |

## 💻 System überwachen

| Befehl | Funktion |
|---|---|
| `df -h` | Speicherplatz anzeigen |
| `free -h` | RAM anzeigen |
| `sudo systemctl status dienst` | Dienst-Status prüfen |
| `sudo systemctl start dienst` | Dienst starten |
| `sudo systemctl stop dienst` | Dienst stoppen |
| `sudo systemctl restart dienst` | Dienst neu starten |

## 📝 Heute geübt auf dem Pi

- Pi-hole Status geprüft mit `systemctl`
- SD-Karte: 26GB total, 18GB frei
- RAM: 3.7GB total, nur 604MB benutzt
- Docker Container laufen alle stabil
