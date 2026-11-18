# Leuchtfeuer

Ein **3D-Koop-Escape** für zwei Handys. Sturmnacht auf Hallig Möwensand: Das Leuchtfeuer ist aus,
der Dampfer *Elise* hält auf die Klippen zu. 15 Minuten.

- **Laternenraum** (oben): Rundum Glas, draußen Regen, Blitze und die Lichter des Schiffs.
  Linse, Kontrolltafel, Kennungsgeber, Messingplatte, Logbuch.
- **Maschinenraum** (unten): Generator, Sicherungskasten, Telegraf, Bücherregal mit dem
  Leuchtfeuerverzeichnis.

Jeder sieht nur seinen Raum. Was man braucht, liegt immer beim anderen. Also redet ihr,
am selben Tisch oder per Telefon („Sprachrohr“).

## Ablauf

1. **Strom:** Oben hängt der Sicherungsplan, unten der Sicherungskasten. Danach geht der Freigabecode nach oben.
2. **Linse:** Unten kommt per Telegraf die Peilung zum Schiff, oben wird die Linse ausgerichtet.
3. **Kennung:** Oben steht die Feuer-Nr. am Linsenfuß, unten steht die Kennung im Verzeichnis. Oben wird sie eingestellt.
4. **Bestätigung:** Oben erscheint ein Code, unten wird er per Telegraf gesendet.

Fehler kosten 30 Sekunden. Beide geben denselben Einsatzcode ein. Daraus entstehen auf beiden
Handys dieselben Rätsel, ganz ohne Server.

## Bedienung

Wischen zum Umsehen, auf leuchtende Punkte tippen zum Untersuchen. Am Rechner gehen auch
Pfeiltasten und Enter. „Was tun?“ gibt einen Tipp passend zum Fortschritt.

## Technik

Eine einzige `index.html` mit [Three.js](https://threejs.org) r128 vom CDN. Die Räume, Texturen
(Planken, Mauerwerk, Messingplatte) und Geräusche (Regen, Donner, Generator, Nebelhorn) werden
im Code erzeugt, es gibt keine Asset-Dateien.

Ein Push auf `main` veröffentlicht das Spiel über GitHub Pages
(Pages-Quelle in den Einstellungen auf „GitHub Actions“ stellen).
