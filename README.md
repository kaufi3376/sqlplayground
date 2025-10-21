# 🧪 SQL Playground

Ein interaktiver Web-Playground zum Schreiben, Ausführen und Speichern von SQL-Abfragen. Perfekt für Lernzwecke, Schulungen oder Prüfungen – dank integriertem Prüfungsmodus.



![image_alt](https://github.com/kaufi3376/sqlplayground/blob/5b3adc89490a5262d2240d3527f6c3435edfb927/SqlPlayground%20Screenshot.PNG)
## ✨ Features

- 🎯 Echtzeit-SQL-Ausführung
- 💡 Syntax-Highlighting mit CodeMirror
- 💾 Abfragen speichern & verwalten
- 🧱 Tabellenstruktur als visuelle Klassenkarten
- 📱 Responsives Design mit flexibler Sidebar
- 🔒 **Prüfungsmodus** – kontrolliertes Abgeben von Lösungen


## 🧪 Prüfungsmodus

Der SQL Playground verfügt über einen integrierten **Prüfungsmodus**, der es Lernenden ermöglicht, ihre SQL-Abfragen **gezielt abzugeben**. In diesem Modus:
- wird die Abgabe dokumentiert,
- sind gespeicherte Abfragen sichtbar,
- und die Benutzeridentifikation kann abgefragt werden.

Ideal für Tests, Übungen oder benotete Aufgaben.


## 📌Datenbank konfiguieren:

1. **Erstelle eine .sql Datei**  
   Trage dort dein gewünschtes Datenbankschema ein. Beispiel:

   ```sql
   CREATE TABLE students (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    grade INTEGER,
    email TEXT,
    birthdate DATE,
    address TEXT,
    enrollment_year INTEGER);
   INSERT INTO students (id, name, grade, email, birthdate, address, enrollment_year) VALUES
   (1, 'Anna Schmidt', 12, 'anna.schmidt@example.com', '2007-04-15', 'Musterstraße 1, Berlin', 2023),
   (2, 'Lukas Meier', 11, 'lukas.meier@example.com', '2008-09-22', 'Beispielweg 5, Hamburg', 2024),
   (3, 'Sofia Keller', 10, 'sofia.keller@example.com', '2009-12-03', 'Ringstraße 12, München', 2025);
   
2. **Logge dich mit deinen eigenen LogIn Daten ein**
   > Hinterlege vor dem Start deine LogIn Daten unter `intern/logInDaten.json`
   
3. **Lade die Datenbank in der Anwendung hoch**
    > Das Schema wird automatisch geladen und steht zur Auswahl bereit.
    
4. **Wähle das Schema aus**
    > Die Datenbank wird mit dem ausgewählten Schema überschrieben und steht bereit zur Nutzung im Playground.
    


    ![image](https://github.com/user-attachments/assets/d6c86b93-0ac6-40ad-a527-13a902edba5a)


## 🚀 SQL Playground starten (Windows – EXE-Version)

Für den einfachen Einsatz im Unterricht und auf Schüler-PCs gibt es eine vorkonfigurierte `sqlplayground.exe`. Damit startet der Playground ohne Installation oder Kommandozeilenkenntnisse.

1. **Doppelklicke auf die Datei `sqlplayground.exe`**  
   > Die Anwendung startet im Hintergrund einen lokalen Server.

2. **Ein schwarzes Fenster (CMD) öffnet sich**  
   > In diesem Fenster erscheint ein Link, z. B.: `Running on http://127.0.0.1:6969/`

3. **Kopiere den Link oder merke ihn dir**  
   > Das ist die Adresse, unter der der SQL Playground für dich und deine Schüler im Browser erreichbar ist.

4. **Öffne deinen Browser (z. B. Chrome oder Firefox)**

5. **Füge den Link in die Adresszeile ein und bestätige mit Enter**  
   > Jetzt öffnet sich der SQL Playground im Browser – bereit für deine SQL-Abfragen.

---

### 🖥️ Lokaler Modus vs. Server Modus

Die Anwendung unterscheidet zwei Betriebsmodi – beide sind über `sqlplayground.exe` oder `app.py` nutzbar:

#### 🔧 Lokaler Modus *(Einzelplatzanwendung)*

- Die Anwendung wird auf dem Schülergerät direkt ausgeführt.
- Sie ist **offlinefähig** und benötigt **keine Internet- oder Netzwerkverbindung**.
- Zugriff erfolgt über `http://127.0.0.1:6969` im lokalen Browser.
- 💡 **Empfohlen:** Gib deinen Schülern eine ZIP-Datei mit:
  - `sqlplayground.exe`
  - dem Ordner `intern/` (enthält Datenbank & Konfiguration)
- Ideal für Hausaufgaben, Tests oder Übungsszenarien am eigenen PC.

#### 🌐 Server Modus *(Netzwerkbetrieb im Klassenzimmer)*

- Der Lehrer startet die Anwendung im Servermodus.
- Die Anwendung erkennt automatisch die lokale IP-Adresse (z. B. `192.168.0.42`) und startet auf Port `6969`.
- Schüler greifen im selben Netzwerk über den Browser zu: `http://192.168.0.42:6969`
- Perfekt für zentral gesteuerte Übungen oder gemeinsames Arbeiten mit derselben Datenbank im Schulnetz.





