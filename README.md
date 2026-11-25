# Reha, Gym & Handstand Tracker

Ein responsiver Fitness- und Reha-Tracker als reine HTML-Datei. Die Anwendung unterstützt die Planung und Dokumentation von Knie-Reha, Oberkörpertraining und Handstand-Sessions.

## Funktionen

- **Übersicht:** aktuelle Trainingsphase, wöchentliche Ziele und anstehende Physiotherapie-Termine
- **Training:** Protokollierung von Knie-Reha, Oberkörper-Gym, Kombi-Einheiten und Handstand-Sessions
- **Übungen:** vorbereitete Trainingspläne, Sätze, Wiederholungen, Gewicht, RIR und eigene Übungen
- **Knie-Check:** Trainingsschmerz, 24-Stunden-Reaktion und Verlauf
- **Handstand:** Stoppuhr, Countdown, Versuche, Qualität, persönliche Bestzeit und vier Progressionsstufen
- **Kalender:** Terminübersicht, Trainingshistorie und feste Physiotherapie-Termine
- **Statistik:** Diagramme zu Training, Handstand und Kniebelastung
- **Datensicherung:** Import und Export als JSON sowie CSV-Bericht
- **Demo-Daten:** Beispielverlauf zum Kennenlernen der Anwendung

## Starten

Die Anwendung benötigt keine Installation oder Build-Umgebung.

### Live-Version

Der Tracker ist als GitHub Pages Website verfügbar:

**https://vladbux.github.io/Fitness-Reha-Tracker/**

### Lokal starten

1. Das Projekt- oder Downloadverzeichnis öffnen.
2. Die Datei `index.html` in einem modernen Browser starten.

Alternativ kann ein einfacher lokaler Webserver verwendet werden, zum Beispiel:

```powershell
python -m http.server 8000
```

Danach `http://localhost:8000` im Browser öffnen.

## Verwendung

1. Über die Navigation zwischen Übersicht, Training, Handstand, Kalender und Statistik wechseln.
2. Neue Einheiten mit Datum und Trainingsart erfassen.
3. Sätze, Wiederholungen, Gewichte und Schmerzwerte eintragen.
4. Handstand-Versuche mit der Stoppuhr erfassen oder manuell eintragen.
5. Unter **Daten & Demo** Demo-Daten laden, ein Backup erstellen oder vorhandene Daten zurücksetzen.

Die Anwendung funktioniert ohne Backend. Alle erfassten Daten werden ausschließlich im Browser über `localStorage` gespeichert. Ein Browserprofil oder privater Modus kann Daten deshalb getrennt verwalten oder beim Löschen der Browserdaten entfernen.

## Datensicherung

Über **Daten & Demo** sind folgende Funktionen verfügbar:

- JSON-Backup herunterladen
- JSON-Backup importieren
- CSV-Bericht mit Trainings- und Physiotherapiedaten herunterladen
- Demo-Daten laden
- Alle gespeicherten Daten zurücksetzen

Vor einem Browserwechsel oder größeren Wartungsarbeiten wird ein JSON-Backup empfohlen.

## Technik

- HTML5
- CSS mit Tailwind CSS über CDN
- Vanilla JavaScript
- Chart.js über CDN
- Browser `localStorage`

Für Tailwind CSS, Chart.js und Google Fonts wird eine Internetverbindung benötigt. Die Anwendungslogik selbst benötigt keinen Server oder Account.

## Projektstruktur

```text
Fitness-Reha-Tracker/
├── index.html
└── README.md
```
