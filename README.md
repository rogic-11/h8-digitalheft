# Nur ein Spaß? · digitales Heft (Ethik 8)

Gehostete Fassung des digitalen Hefts für eine Klasse: https://ethik8-gbs.github.io/heft/

Der gesamte Inhalt in `index.html` ist mit dem Klassenpasswort verschlüsselt (AES-256-GCM, Schlüssel aus dem Passwort über PBKDF2); ohne Passwort zeigt die Seite nur die Tür. Die Seite speichert Antworten nur im Browser des Geräts und sendet nichts. Die Content Security Policy erlaubt Verbindungen nur zum eigenen Ursprung (`connect-src 'self'`), damit das Heft die verschlüsselten Videos laden kann.

| Datei | Inhalt |
|---|---|
| `index.html` | das Heft, Inhalt verschlüsselt; im Klartext nur Tür, Schriften und Code |
| `manifest.webmanifest`, `icon-180.png`, `icon-512.png` | „Zum Home-Bildschirm“ auf dem iPad |
| `medien/*.bin` | neun Videos für die Klasse, einzeln mit dem Klassenpasswort verschlüsselt (AES-256-GCM); ohne Passwort nur Datenrauschen |
| `probe/` | Probeumgebung: `index.html`, `manifest.webmanifest`, Symbole; Adresse `…/probe/` (die Beispieldateien bleiben lokal) |
| `medien/LIZENZ.md` | Lizenz und Löschfrist (19.05.2027) |

Quelle und Werkzeuge liegen in einem privaten Repository. Diese Seite wird von dort gebaut und veröffentlicht.
