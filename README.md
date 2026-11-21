# Frank Parussel · 153er-netz.de

Ich beschäftige mich mit FHEM, Hausautomation, Heizungsregelung und
Energiemanagement. Hier veröffentliche ich Lösungen, die aus dem praktischen
Betrieb meiner eigenen Anlage entstanden sind.

🌐 [153er-netz.de](https://153er-netz.de) ·
[FHEM-Projekte im 153er Netz](https://153er-netz.de/seiten/entwicklung/fhem.html)

## Heizungsregelung als zusammenhängender Modulverbund

Ein Schwerpunkt ist eine erweiterte FHEM-Regelkette für Fußbodenheizung,
Rücklaufmessung, dynamische Bodenerhaltung und Mischerregelung. Die sechs
Bausteine können abhängig von der jeweiligen Anlage einzeln oder gemeinsam
eingesetzt werden:

1. [OW2S0SMSGUARD](https://github.com/parussel/OW2S0SMSGUARD) liest
   OneWire-Temperatursensoren und prüft auffällige Messsprünge.
2. [TempReadingFilter](https://github.com/parussel/TempReadingFilter) gibt
   Rücklaufwerte erst nach Ventilöffnungs- und hydraulischer Transportzeit frei.
3. [PWM](https://github.com/parussel/PWM-PWMR) verteilt die zeitlichen
   Heizanforderungen der Räume.
4. [PWMR](https://github.com/parussel/PWM-PWMR) regelt Solltemperatur,
   Raumtemperatur und Ventil eines einzelnen Raums.
5. [PWMK – PWM KeepAlive](https://github.com/parussel/PWM-PWMR) ergänzt
   raumindividuelle dynamische Erhaltungspulsabstände anhand belastbarer
   Rücklaufwerte.
6. [PID20 Community Edition](https://github.com/parussel/PID20) regelt unter
   anderem die vorgelagerten Mischer und Vorlauftemperaturen.

Hydraulik, Anlegefühler, Messwertfreigabe, Sicherheits- und Rückfallebenen
sowie das Zusammenspiel der Module sind in der
**[zentralen Dokumentation der Heizungsregelkette](https://github.com/parussel/PWM-PWMR/blob/main/HEIZUNGSREGELKETTE.md)**
zusammenhängend beschrieben.

## Weitere öffentliche Projekte

### [TibberConnect und TibberLive](https://github.com/parussel/TibberConnect)

Zwei zusammenarbeitende FHEM-Module für Tibber-Viertelstundenpreise,
Preisplanung und – optional – aktuelle Tibber-Pulse-IR-Werte. Der öffentliche
Release Candidate wurde automatisiert sowie auf Raspberry Pi 3 und 4 geprüft.
Die Installationsanleitung beschreibt die sichere Reihenfolge, Diagramme,
Übersichten und einen begrenzten FHEM-Updatekanal.

### [Gradient](https://github.com/parussel/Gradient)

FHEM-Modul zur Erkennung dynamischer Änderungen in Messwerten mittels linearer
Regression – beispielsweise Temperaturanstieg, schneller Temperaturabfall oder
Feuchteanstieg.

### [FHEM Style – 153er-netz.de Edition](https://github.com/parussel/fhem-style-153er-netz)

Eigenständig installierbarer FHEM-Style auf Grundlage der Arbeit von
[Matthias Kleine (Kleinor)](https://github.com/klein0r/fhem-style-haus-automatisierung).
Bedienung und Layout bleiben erhalten; Erscheinungsbild und Logo wurden für
153er-netz.de angepasst.

### [Alexa-FHEM – lokale SSH-RSA/SHA-2-Anleitung](https://github.com/parussel/Alexa-FHEM)

Deutschsprachige Schritt-für-Schritt-Anleitung für die lokale
RSA/SHA-2-Anpassung einer bestehenden alexa-fhem-Installation 0.5.64 – mit
Prüfschritten, Sicherung und Rückweg.

> **Hinweis zum Entwicklungsstand:** Die veröffentlichten Erweiterungen sind
> keine offiziellen Bestandteile von FHEM. Teilweise fehlt noch eine breite
> Erprobung in unterschiedlichen Anlagen. Vor Änderungen an einer laufenden
> Installation sind eine Sicherung und ein Test in einer getrennten Umgebung
> sinnvoll. Die jeweilige Projektseite nennt Prüfstand und bekannte Grenzen.

## Austausch

Hinweise und nachvollziehbare Fehlermeldungen zu veröffentlichten Projekten
sind in den jeweiligen GitHub-Issues willkommen.
