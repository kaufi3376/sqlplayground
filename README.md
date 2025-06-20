# 🧪 SQL Playground

Ein interaktiver Web-Playground zum Schreiben, Ausführen und Speichern von SQL-Abfragen. Perfekt für Lernzwecke, Schulungen oder Prüfungen – dank integriertem Prüfungsmodus.



![image_alt]()
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


### 📌 Schritt-für-Schritt-Anleitung:

1. **Öffne die Datei `schema.sql`**  
   Trage dort dein gewünschtes Datenbankschema ein. Beispiel:

   ```sql
   CREATE TABLE students (
       id INTEGER PRIMARY KEY,
       name TEXT,
       grade INTEGER
   );
2. **Lösche die bestehende Datenbankdatei my_database.db**
    Diese Datei wird beim nächsten Start automatisch neu erstellt – basierend auf deiner schema.sql.

3. **Starte die Anwendung erneut**
     Die neue Datenbank wird automatisch geladen und steht bereit zur Nutzung im Playground.
