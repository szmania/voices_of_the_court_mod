# Häufig gestellte Fragen

## 1. Es erscheint kein Dialogfeld
Diese Mod erfordert ein zusätzliches Backend-Programm. Laden Sie das lokalisierte Backend-Programm hier herunter: [https://github.com/szmania/Voices_of_the_Court/releases/latest](https://github.com/szmania/Voices_of_the_Court/releases/latest). Die heruntergeladene .exe-Datei installiert sich beim Öffnen automatisch.

## 2. Probleme bei der API-Konfiguration
Es wird empfohlen, die offizielle DeepSeek-API zu verwenden. Wählen Sie im Dropdown-Menü für die Verbindung zum Dialogmodell die Seite `custom(openai-compatible)` aus, um Folgendes zu konfigurieren:
- Server-URL: `https://api.deepseek.com/beta`
- API-Schlüssel: Geben Sie Ihren eigenen API-Schlüssel ein, den Sie unter [https://platform.deepseek.com](https://platform.deepseek.com) beantragen können.

OpenAI und OpenRouter sollten ebenfalls kompatibel sein.

## 3. Es erscheint kein Dialogfeld, obwohl das Backend-Programm nach der Installation läuft
**Lösung**: Sie müssen die Lokalisierungs-Mod verwenden.

Installationsmethoden (wählen Sie eine):
1. Nachdem Sie die heruntergeladenen Dateien der Lokalisierungs-Mod extrahiert haben, überschreiben Sie die ursprünglichen Mod-Dateien direkt im Steam Workshop-Verzeichnis.
2. Legen Sie den extrahierten Mod-Ordner `voices_of_the_court_mod-1.2.1-beta` in den Mod-Ordner des Spiels. Erstellen Sie dann mit Notepad eine neue Datei namens `voices_of_the_court_mod-1.2.1-beta.mod` im Ordner `Documents\Paradox Interactive\Crusader Kings III\mod` mit folgendem Inhalt:
version="1.0"
tags={
"Gameplay"
}
name="Voices of the Court mcc"
supported_version="1.13.1"
path="C:/Users/ [Ihr PC-Benutzername hier] / Documents/Paradox Interactive/Crusader Kings III/mod/voices_of_the_court_mod-1.2.1-beta"

Wenn das Dialogfeld nach der Installation und Aktivierung der Lokalisierungs-Mod immer noch nicht erscheint, ist möglicherweise der Pfad des CK3-Benutzerordners falsch eingestellt oder das Spiel befindet sich im Ironman-Modus. Diese Mod funktioniert nicht im Ironman-Modus.

## 4. Fehler "TypeError: Cannot read properties of undefined (reading 'playerID')" mit rotem Text beim Öffnen des Chat-Fensters
**Lösung**: Erstellen Sie einen Ordner namens `run` in `Documents\Paradox Interactive\Crusader Kings III`. Gehen Sie in diesen Ordner und erstellen Sie eine Textdatei namens `votc.txt`.

## 5. Kürzliche Erinnerungen werden beim Sprechen mit Charakteren nicht gelesen
**Lösung**:
1. Dies ist ein kleiner Fehler im Backend-Programm des ursprünglichen Autors; das Herunterladen des lokalisierten Backends löst dies.
2. Es kann auch an den Token-Limits für den Speicher liegen. Passen Sie die Größe der `max memory tokens` auf der Einstellungsseite des Backend-Programms an. Nach dem Anpassen der Speicher-Token sollten Sie auch die `max new tokens` erhöhen; es ist am besten, wenn `max new tokens` größer als `max memory tokens` ist.

## 6. Das Prompt-Generierungsskript wird nach dem Neustart des Backend-Programms zurückgesetzt
**Lösung**:
Speichern Sie es als separate Datei im Ordner `custom`.

Mod Name: Voices of the Court - Community Edition
License: GNU General Public License v3.0 (GPLv3)

Credits & Attribution
This project is a derivative work based on VOTC / AliChat. We would like to extend our deep gratitude to the developers who kept this project alive and pushed the boundaries of AI in Crusader Kings III:

Original Creators: The VOTC Team and community contributors.

Continued Development: Special thanks to the Chinese development community, including Lisiyuan233, zhaowendao2005, and others who provided critical updates and support.

Community Support: Thanks to Durond and MrAndroPC and the broader community for their insights and historical context regarding the project.

Licensing Information
Some of original source material for this mod was released under the Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) license.

In accordance with Section 4(b) of the CC BY-SA 4.0 license, this derivative work is being licensed under a BY-SA Compatible License: the GNU General Public License v3.0 (GPLv3).

Original License: CC BY-SA 4.0

Current License: GPLv3
