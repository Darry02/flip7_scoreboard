FLIP 7 SCOREBOARD – PWA

INHALT
- index.html             App
- manifest.webmanifest   Installationsdaten
- sw.js                  Offline-Cache
- icon-192.png           App-Icon
- icon-512.png           App-Icon

FUNKTIONEN
- 2–20 aktive Mitspieler
- Punkte je Runde eintragen und automatisch addieren
- Sieger automatisch bei mindestens 200 Punkten + eindeutiger Führung
- Undo der letzten Runde
- Sieg-/Langzeitstatistik über abgeschlossene Partien
- Rangliste, Siegquote, Durchschnittspunkte, Direktvergleich
- Partiehistorie
- IndexedDB als dauerhafter lokaler Datenspeicher
- JSON Backup Export/Import
- Offline-Nutzung nach Installation

WICHTIG ZUR INSTALLATION
Eine PWA kann aus Sicherheitsgründen nicht direkt über file:// als App installiert werden.
Sie muss einmal über HTTPS (oder localhost) geöffnet werden.

Einfachste dauerhafte Variante:
1. Den kompletten Ordner auf einen statischen Webhost laden, z.B. GitHub Pages.
2. Die HTTPS-Seite auf dem Handy öffnen.
3. Android/Chrome: Browser-Menü -> "App installieren" oder "Zum Startbildschirm hinzufügen".
   iPhone/Safari: Teilen -> "Zum Home-Bildschirm".
4. Danach läuft die App offline und wie eine normale App.

DATENSPEICHER
Die Statistiken liegen lokal in IndexedDB des Browsers/PWA-Profils.
Sie werden nicht an einen Server gesendet.
Für Handywechsel, Browserwechsel oder zusätzliche Sicherung regelmäßig
unter "Spieler" -> "Backup exportieren" eine JSON-Datei speichern.
