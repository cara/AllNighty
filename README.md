# AllNighty

**Dein Backlog, über Nacht abgearbeitet.** · [English below](#english)

AllNighty ist eine kleine App für die Menüleiste deines Macs. Du schreibst
Aufgaben auf, und ein KI-Agent arbeitet sie selbstständig in deinen eigenen
GitHub-Projekten ab, zum Beispiel über Nacht. Das Ergebnis bekommst du als
Branch oder Pull Request. Morgens schaust du nur noch drüber und entscheidest,
was du übernimmst.

- **Aufgaben:** Die eingebaute Aufgabenliste reicht. Wer mag, verbindet
  stattdessen Things 3, Todoist, Notion, Google Tasks oder GitHub Issues.
- **KI-Anbieter:** Claude Code (empfohlen), OpenAI Codex, OpenRouter (über den
  Pi-Agenten) oder Pi. Experimentell: OpenCode, Cursor, GitHub Copilot, Grok
  und Antigravity. Du brauchst dafür ein eigenes Konto, Abo oder einen
  API-Schlüssel beim Anbieter. Die KI-Kosten trägst du selbst.
- **iPhone (optional):** Eine Begleit-App für iOS gibt es als TestFlight-Beta.
  Sie verbindet sich über dein privates iCloud.

Website: **[allnighty.com](https://allnighty.com)**

## Download

Die aktuelle Version findest du unter
**[Releases → neueste Version](https://github.com/cara/AllNighty/releases/latest)**.

- `AllNighty-X.Y.Z.dmg`: **empfohlen.** Öffnen und AllNighty in den Ordner
  *Programme* ziehen.
- `AllNighty-X.Y.Z.app.zip`: dieselbe App als ZIP, falls du lieber selbst
  entpackst.

AllNighty gibt es nur für den Mac.

## Voraussetzungen

- Mac mit Apple-Chip (M1 oder neuer)
- macOS 13 oder neuer
- ein GitHub-Konto
- ein Konto, Abo oder API-Schlüssel bei einem der KI-Anbieter

## Erster Start

1. DMG öffnen und **AllNighty** in den Ordner **Programme** ziehen. Dann die
   App von dort starten.
2. Die Checkliste **„Bereit?“** führt dich durch alles Weitere. Jede Zeile
   zeigt, ob etwas fehlt, und hat einen Knopf, der es einrichtet:
   - die Xcode Command Line Tools (Apples Entwickler-Grundwerkzeuge)
   - die GitHub CLI (`gh`) und die Anmeldung bei GitHub
   - das Programm deines KI-Anbieters und die Anmeldung dort
3. Wenn alles grün ist, auf **„Loslegen“** klicken.

Besondere Rechte in den Systemeinstellungen brauchst du dafür nicht. Nur wenn
du **Things 3** als Aufgabenquelle nutzt, fragt macOS nach *Festplattenvollzugriff*
(damit AllNighty deine Things-Aufgaben lesen kann) und nach der Erlaubnis,
Things zu steuern.

Solange Aufgaben laufen, hält AllNighty deinen Mac wach. Über Nacht am besten
ans Netzteil hängen.

## Bitte lesen: Sicherheit

AllNighty lässt den KI-Agenten **ohne Rückfragen** arbeiten, mit deinen
Benutzerrechten und in den Projekten, die du eingerichtet hast. Der Agent
kann dort alles tun, was du selbst am Mac tun könntest: Dateien ändern,
Programme ausführen, Daten ins Internet schicken.

- Richte **nur eigene oder vertrauenswürdige Projekte** ein.
- Text aus Aufgaben und Projekten kann versteckte Anweisungen an die KI
  enthalten („Prompt-Injection“). Nutze keine geteilten Listen oder fremden
  Inhalte als Aufgabenquelle.
- Schau dir jedes Ergebnis an, **bevor** du es übernimmst (mergst).

Mehr dazu im [Haftungsausschluss](https://allnighty.com/disclaimer.html).

## Updates

AllNighty sucht einmal am Tag nach einer neuen Version und installiert sie
auf Wunsch direkt in der App. Updates sind signiert und von Apple
notarisiert. Die automatische Suche kannst du in den Einstellungen
ausschalten.

## Preis

Während der Beta ist AllNighty **kostenlos**. Kosten bei deinem KI-Anbieter
zahlst du direkt dort.

## Hilfe und Support

Schreib an **[support@allnighty.com](mailto:support@allnighty.com)**. Bitte
hänge den **Diagnosebericht** an (in der App unter **Hilfe →
Diagnosebericht erstellen…**). Du kannst dir vorher ansehen, was drinsteht.

Issues und Pull Requests werden in diesem Repository nicht bearbeitet.

## Rechtliches

- [Impressum](https://allnighty.com/impressum.html)
- [Datenschutz](https://allnighty.com/datenschutz.html)
- [Nutzungsbedingungen](https://allnighty.com/nutzungsbedingungen.html)
- [Haftungsausschluss](https://allnighty.com/disclaimer.html)

Dieses Repository enthält nur die Release-Dateien; der Quellcode ist nicht
öffentlich. Proprietäre Software – siehe
[Nutzungsbedingungen](https://allnighty.com/nutzungsbedingungen.html).

---

<a id="english"></a>

## English

**Your backlog, worked through overnight.**

AllNighty is a small app for your Mac's menu bar. You write down tasks, and
an AI coding agent works on them on its own in your own GitHub projects, for
example overnight. Results arrive as a branch or pull request. In the morning
you review them and decide what to keep.

- **Tasks:** the built-in task list is all you need. You can connect Things 3,
  Todoist, Notion, Google Tasks or GitHub Issues instead.
- **AI providers:** Claude Code (recommended), OpenAI Codex, OpenRouter (via
  the Pi agent) or Pi. Experimental: OpenCode, Cursor, GitHub Copilot, Grok and
  Antigravity. You need your own account, subscription or API key with the
  provider. AI costs are yours.
- **iPhone (optional):** an iOS companion app is available as a TestFlight
  beta. It connects through your private iCloud.

Website: **[allnighty.com](https://allnighty.com)**

### Download

Get the current version from
**[Releases → latest](https://github.com/cara/AllNighty/releases/latest)**.

- `AllNighty-X.Y.Z.dmg`: **recommended.** Open it and drag AllNighty into
  *Applications*.
- `AllNighty-X.Y.Z.app.zip`: the same app as a ZIP, if you prefer to unpack it
  yourself.

AllNighty is available for Mac only.

### Requirements

- Mac with Apple silicon (M1 or newer)
- macOS 13 or newer
- a GitHub account
- an account, subscription or API key with one of the AI providers

### First start

1. Open the DMG, drag **AllNighty** into **Applications** and start it from
   there.
2. The **"Bereit?" (Ready?)** checklist guides you through the rest. Each line
   shows what is missing and has a button that sets it up:
   - Xcode Command Line Tools (Apple's basic developer tools)
   - GitHub CLI (`gh`) and signing in to GitHub
   - your AI provider's program and signing in to it
3. When everything is green, click **"Loslegen" (Get started)**.

No special permissions in System Settings are needed. Only if you use
**Things 3** as your task source will macOS ask for *Full Disk Access* (so
AllNighty can read your Things tasks) and for permission to control Things.

While tasks are running, AllNighty keeps your Mac awake. Plug it in overnight.

### Please read: security

AllNighty lets the AI agent work **without asking for permission**, with your
user rights, in the projects you set up. There the agent can do anything you
could do on your Mac: change files, run programs, send data to the internet.

- Only set up **your own or trusted projects**.
- Text in tasks and projects can contain hidden instructions to the AI
  ("prompt injection"). Don't use shared lists or other people's content as a
  task source.
- Review every result **before** you merge it.

More in the [disclaimer](https://allnighty.com/en/disclaimer.html).

### Updates

AllNighty checks for a new version once a day and can install it right in
the app. Updates are signed and notarised by Apple. You can switch off the
automatic check in the settings.

### Price

AllNighty is **free during the beta**. You pay your AI provider directly.

### Help and support

Email **[support@allnighty.com](mailto:support@allnighty.com)**. Please attach
the **diagnostic report** (in the app: **Hilfe → Diagnosebericht
erstellen…**). You can look at what it contains first.

Issues and pull requests are not handled in this repository.

### Legal

- [Imprint](https://allnighty.com/en/imprint.html)
- [Privacy](https://allnighty.com/en/privacy.html)
- [Terms of use](https://allnighty.com/en/terms.html)
- [Disclaimer](https://allnighty.com/en/disclaimer.html)

This repository contains only the release files; the source code is not
public. Proprietary software – see the
[terms of use](https://allnighty.com/en/terms.html).
