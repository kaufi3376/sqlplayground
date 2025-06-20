# 🧪 SQL Playground

Ein interaktiver Web-Playground zum Schreiben, Ausführen und Speichern von SQL-Abfragen. Perfekt für Lernzwecke, Schulungen oder Prüfungen – dank integriertem Prüfungsmodus.



![image_alt](https://github.com/kaufi3376/sqlplayground/blob/5b3adc89490a5262d2240d3527f6c3435edfb927/SqlPlayground%20Screenshot.PNG)
## ✨ Features

- 🎯 Echtzeit-SQL-Ausführung
- 💡 Syntax-Highlighting mit CodeMirror
- 💾 Abfragen speichern & verwalten
- 🧱 Tabellenstruktur als visuelle Klassenkarten
- 👤 Benutzername-Modal für individuelle Nutzung
- 📱 Responsives Design mit flexibler Sidebar
- 🔒 **Prüfungsmodus** – kontrolliertes Abgeben von Lösungen


## 🧪 Prüfungsmodus

Der SQL Playground verfügt über einen integrierten **Prüfungsmodus**, der es Lernenden ermöglicht, ihre SQL-Abfragen **gezielt abzugeben**. In diesem Modus:
- wird die Abgabe dokumentiert,
- sind gespeicherte Abfragen sichtbar,
- und die Benutzeridentifikation kann abgefragt werden.

Ideal für Tests, Übungen oder benotete Aufgaben.


## 📌Datenbank konfiguieren:

1. **Öffne die Datei `schema.sql`**  
   Trage dort dein gewünschtes Datenbankschema ein. Beispiel:

   ```sql
   CREATE TABLE students (
       id INTEGER PRIMARY KEY,
       name TEXT,
       grade INTEGER
   );
2. **Lösche die bestehende Datenbankdatei my_database.db** 
    > Diese Datei wird beim nächsten Start automatisch neu erstellt – basierend auf deiner schema.sql.

3. **Starte die Anwendung erneut**
    > Die neue Datenbank wird automatisch geladen und steht bereit zur Nutzung im Playground.

## 🚀 SQL Playground starten (Windows – EXE-Version)

Für den einfachen Einsatz im Unterricht oder auf Schüler-PCs gibt es eine vorkonfigurierte `sqlplayground.exe`. Damit startet der Playground ohne Installation oder Kommandozeilenkenntnisse.

1. **Doppelklicke auf die Datei `sqlplayground.exe`**
   > Die Anwendung startet im Hintergrund einen lokalen Server.

2. **Ein schwarzes Fenster (CMD) öffnet sich**
   > In diesem Fenster erscheint ein Link, z. B.: Running on http://127.0.0.1:6969/

3. **Kopiere den Link oder merke ihn dir**
   > Das ist die Adresse, unter der der SQL Playground im Browser erreichbar ist.

4. **Öffne deinen Browser (z. B. Chrome oder Firefox)**

5. **Füge den Link in die Adresszeile ein und bestätige mit Enter**
   > Jetzt öffnet sich der SQL Playground im Browser – bereit für deine SQL-Abfragen.

🔒 **Hinweis:** Die Anwendung läuft nur lokal – es wird nichts ins Internet übertragen.


