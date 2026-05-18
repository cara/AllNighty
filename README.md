# Nightshift — Releases & Download

Dieses Repo hostet ausschließlich die **fertigen Release-Artefakte** von
Nightshift (macOS-DMG / Windows-Installer). Der **Quellcode liegt in einem
separaten, privaten Repo** und ist hier bewusst nicht enthalten.

## Download

Die jeweils aktuelle Version gibt es unter
**[Releases](https://github.com/cara/Nightshift/releases/latest)**:

- `Nightshift-X.Y.Z.dmg` — macOS, notarisierter Drag-and-drop-Installer (empfohlen)
- `Nightshift-X.Y.Z.app.zip` — macOS, entpacken und nach *Programme* ziehen
- `Nightshift-Setup-X.Y.Z.exe` — Windows-Installer (bringt eigene Python-Runtime mit)

Die macOS-App aktualisiert sich danach selbst über genau diese Releases
(Menübar → *Nach Updates suchen…*).

## Installation (macOS, Kurzfassung)

1. DMG öffnen, **Nightshift.app** nach **Programme** ziehen.
2. App einmal starten. macOS verlangt *Full Disk Access* (Lesezugriff auf die
   Things-Datenbank) und *Automation: Things 3* (AppleScript-Steuerung) —
   beides in den Systemeinstellungen erlauben.
3. Über das Menübar-Icon (Mond) **Start** klicken.

## ⚠️ Sicherheits-Hinweis

Nightshift startet `claude` mit `--dangerously-skip-permissions` in den im
Watcher konfigurierten Repos — die App kann darin alles tun, was auch der
Nutzer in einem Terminal könnte. **Nur eigene, vertraute Repos einrichten.**

## Hinweis

Die Releases in diesem Repo werden **automatisch** von der CI-Pipeline des
privaten Quell-Repos erzeugt, signiert und notarisiert. Issues und Pull
Requests werden hier nicht bearbeitet.
