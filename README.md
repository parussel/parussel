# Frank Parussel · 153er-netz.de

Ich beschäftige mich mit FHEM, Hausautomation und Energiemanagement. Hier teile ich Lösungen, die aus dem praktischen Betrieb meiner eigenen Anlage entstanden sind.

🌐 [153er-netz.de](https://153er-netz.de) · [Entwicklung](https://153er-netz.de/seiten/entwicklung.html)

## Öffentliche Projekte

### [FHEM Style – 153er-netz.de Edition](https://github.com/parussel/fhem-style-153er-netz)

Ein eigenständig installierbarer FHEM-Style auf Grundlage der Arbeit von [Matthias Kleine (Kleinor)](https://github.com/klein0r/fhem-style-haus-automatisierung). Die Bedienung und das Layout bleiben erhalten; Erscheinungsbild und Logo wurden für 153er-netz.de angepasst.

### [PID20 Community Edition](https://github.com/parussel/PID20)

Unabhängige Community-Weiterentwicklung des FHEM-PID20-Reglers. Sie korrigiert die Wirkrichtung des D-Anteils im Reverse-Betrieb und ergänzt eine optionale Glättung über mehrere Messwerte. Automatisierte und isolierte Tests sowie ein Einsatz mit bestehenden Definitionen wurden geprüft; eine breite Erprobung in unterschiedlichen Heizungsanlagen steht noch aus.

### [Gradient](https://github.com/parussel/Gradient)

FHEM-Modul zur Erkennung dynamischer Änderungen in Messwerten mittels linearer Regression – zum Beispiel Temperaturanstieg am Zirkulationsrücklauf, schneller Temperaturabfall oder Feuchteanstieg. Automatisierte Tests und mehrere laufende Definitionen wurden geprüft; eine breite Erprobung steht noch aus.

### [TempReadingFilter](https://github.com/parussel/TempReadingFilter)

FHEM-Modul, das Temperaturwerte abhängig vom Zustand eines Aktors und einer einstellbaren Wartezeit weitergibt. Der Verzögerungsablauf, veraltete Timer und der Betrieb in einer vorhandenen FHEM-Installation wurden geprüft; eine breite Erprobung steht noch aus.

## In Vorbereitung

| Projekt | Zweck | Stand |
| --- | --- | --- |
| **TibberConnect** | Einbindung dynamischer Strompreise in FHEM | In Vorbereitung: Das frühere GitHub-Repository wurde gelöscht; die weitere Prüfung und eine neue Veröffentlichung folgen nach der FHEM-Migration. |

**Hinweis zum Entwicklungsstand:** Für diese Werkzeuge fehlt teilweise noch eine breite Erprobung in unterschiedlichen Anlagen. Wer einen veröffentlichten Stand installiert oder einsetzt, tut dies in eigener Verantwortung. Vor Änderungen an einer laufenden FHEM-Anlage sind eine Sicherung und ein Test in einer getrennten Umgebung sinnvoll. Die jeweilige Projektseite nennt den konkreten Prüfstand und die bekannten Grenzen.

## Austausch

Hinweise und nachvollziehbare Fehlermeldungen zu veröffentlichten Projekten sind in deren GitHub-Issues willkommen.
