# Unix/Linux Grundlagen - Übungsblatt

## Praktische Aufgaben für Studierende

---

## Vorbereitung

Öffnen Sie ein Terminal und stellen Sie sicher, dass Sie in Ihrem Home-Verzeichnis sind:

```bash
cd ~
```

---

## Aufgabe 1: Navigation und Grundkommandos

### 1.1 Verzeichnis-Navigation

1. Zeigen Sie das aktuelle Verzeichnis an
2. Wechseln Sie in das Verzeichnis `/tmp`
3. Gehen Sie zurück in Ihr Home-Verzeichnis
4. Listen Sie alle Dateien und Ordner in Ihrem Home-Verzeichnis auf (inklusive versteckte)

**Lösung dokumentieren**: Schreiben Sie die verwendeten Kommandos auf.

### 1.2 Systeminformationen

1. Zeigen Sie Ihren Benutzernamen an
2. Zeigen Sie alle aktuell angemeldeten Benutzer
3. Zeigen Sie Systeminformationen an (Kernel-Version, etc.)
4. Zeigen Sie die Festplattenbelegung in lesbarem Format an

### 1.3 Prozesse

1. Listen Sie alle Ihre laufenden Prozesse auf
2. Zeigen Sie die Prozesse in Echtzeit an (beenden Sie mit `q`)
3. Suchen Sie nach allen Prozessen, die "bash" enthalten

---

## Aufgabe 2: Arbeiten mit dem D1GB-Ordner

### 2.1 D1GB-Ordner erkunden

**Vorbereitung**: Stellen Sie sicher, dass der `D1GB`-Ordner in Ihrem Home-Verzeichnis verfügbar ist.

1. Navigieren Sie zum D1GB-Ordner: `cd ~/D1GB`
2. Zeigen Sie den vollständigen Pfad an: `pwd`
3. Listen Sie alle Textdateien auf: `ls -la *.txt`
4. Zählen Sie, wie viele Textdateien sich im Ordner befinden
5. Zeigen Sie die Größe des gesamten D1GB-Ordners an

### 2.2 Verzeichnisstruktur für Analyse erstellen

Erstellen Sie eine Arbeitsstruktur für die Datenanalyse:

```
unix_uebung/
├── d1gb_analysis/
│   ├── filtered/
│   ├── sorted/
│   └── reports/
├── scripts/
└── backups/
```

**Anforderungen**:

- Erstellen Sie alle Verzeichnisse mit einem einzigen Kommando
- Kopieren Sie 5 beliebige Textdateien aus D1GB nach `d1gb_analysis/`
- Navigieren Sie in das `d1gb_analysis`-Verzeichnis

1. Erstellen Sie in Ihrem `d1gb_analysis`-Verzeichnis eine Datei namens `analysis_notes.txt`
2. Fügen Sie folgenden Inhalt hinzu:

   ```
   D1GB Datenanalyse
   Datum: [Heutiges Datum]
   Analyst: [Ihr Name]

   Übersicht:
   - Textdateien untersuchen
   - Muster identifizieren
   - Berichte erstellen
   ```

3. Erstellen Sie ein Backup dieser Datei im `backups/`-Verzeichnis
4. Kopieren Sie 3 unterschiedliche Textdateien aus dem D1GB-Ordner in Ihr Arbeitsverzeichnis

---

## Aufgabe 3: D1GB Textanalyse

### 3.1 Dateigröße und -inhalt analysieren

1. Finden Sie die 5 größten Textdateien im D1GB-Ordner
2. Zeigen Sie die ersten 10 Zeilen der größten Datei an
3. Zeigen Sie die letzten 5 Zeilen einer beliebigen Textdatei
4. Zählen Sie Zeilen, Wörter und Zeichen in verschiedenen D1GB-Dateien

### 3.2 Textsuche im D1GB-Ordner

1. Suchen Sie in allen D1GB-Textdateien nach einem häufigen Wort (z.B. "the", "and", "data")
2. Finden Sie alle Dateien, die eine bestimmte Zeichenkette enthalten
3. Erstellen Sie eine Liste aller eindeutigen Wörter aus einer D1GB-Datei (sortiert)
4. Zählen Sie, wie oft ein bestimmtes Wort in allen Textdateien vorkommt

---

## Aufgabe 4: D1GB Datenverarbeitung mit Pipelines

### 4.1 Erweiterte D1GB-Analyse

1. Listen Sie alle D1GB-Textdateien nach Größe sortiert auf (größte zuerst)
2. Finden Sie die 10 häufigsten Wörter in einer großen D1GB-Datei
3. Zählen Sie, wie viele D1GB-Dateien einen bestimmten Begriff enthalten
4. Zählen Sie, wie viele `.txt`-Dateien sich in Ihrem `unix_uebung`-Verzeichnis befinden (rekursiv)

### 4.2 D1GB-Datenberichte mit Umleitung

1. Erstellen Sie eine Datei `d1gb_report.txt` mit folgendem Inhalt:

   - Aktuelle Uhrzeit und Datum
   - Anzahl der Textdateien im D1GB-Ordner
   - Gesamtgröße des D1GB-Ordners
   - Die 3 größten Dateien
   - Verwenden Sie Umleitung, nicht copy-paste!

2. Fügen Sie an `d1gb_report.txt` eine Liste der ersten 20 Dateien (alphabetisch sortiert) an

### 4.3 Komplexe D1GB-Pipelines

Erstellen Sie Pipelines, die:

1. Alle D1GB-Textdateien nach Größe sortieren und die 5 größten anzeigen
2. Den Gesamtinhalt aller kleinen D1GB-Dateien (< 1KB) zusammenfassen
3. Ein Wörterbuch aller eindeutigen Wörter aus 3 D1GB-Dateien erstellen
4. Das Ergebnis in eine Datei `datei_statistik.txt` schreibt

**Eine Pipeline - ein Kommando!**

---

## Aufgabe 5: Editoren

### 5.1 nano verwenden

1. Öffnen Sie `notizen.txt` mit nano
2. Fügen Sie am Ende drei neue Zeilen mit eigenen Notizen hinzu
3. Speichern Sie die Datei und beenden Sie nano
4. Erstellen Sie mit nano eine neue Datei `meine_aliase.txt` mit nützlichen Alias-Definitionen

### 5.2 vim Grundlagen

**Achtung**: Nur bearbeiten, wenn Sie sich sicher fühlen!

1. Öffnen Sie `liste.txt` mit vim
2. Fügen Sie am Ende der Datei "Feige" hinzu
3. Löschen Sie die Zeile mit "Cherry"
4. Speichern Sie und beenden Sie vim

**Tipp**: `:wq!` zum Speichern und Beenden, `:q!` zum Beenden ohne Speichern

---

## Aufgabe 6: D1GB Archivierung und erweiterte Funktionen

### 6.1 D1GB Wildcards und Dateisuche

1. Listen Sie alle D1GB-Dateien auf, die mit einem bestimmten Buchstaben beginnen
2. Finden Sie alle D1GB-Dateien, die eine bestimmte Dateiendung haben
3. Kopieren Sie alle D1GB-Dateien, die kleiner als 5KB sind, in das `filtered/`-Verzeichnis
4. Erstellen Sie eine Liste aller D1GB-Dateien mit ihren Größen (sortiert nach Größe)

### 6.2 D1GB-Daten archivieren

1. Erstellen Sie ein komprimiertes tar-Archiv Ihrer D1GB-Analyse
   - Name: `d1gb_analysis_[DATUM].tar.gz`
   - Inklusive aller erstellten Berichte und gefilterten Dateien
2. Erstellen Sie ein separates Archiv mit den 10 größten D1GB-Dateien
3. Listen Sie den Inhalt beider Archive auf, ohne sie zu extrahieren
4. Vergleichen Sie die Komprimierungsraten der verschiedenen Archive

---

## Aufgabe 7: D1GB-Daten Problemlösung und Analyse

### 7.1 Realistische D1GB-Datenanalyse

**Arbeiten Sie direkt mit echten D1GB-Textdateien:**

**Ihre Aufgaben**:

1. Finden Sie die häufigsten Fehler oder Probleme in den D1GB-Dateien (z.B. leere Zeilen, ungültige Zeichen)
2. Identifizieren Sie Dateien mit ungewöhnlich vielen/wenigen Zeilen
3. Erstellen Sie eine Liste aller D1GB-Dateien, die bestimmte Schlüsselwörter enthalten
4. Analysieren Sie die Verteilung der Dateiformate und -größen im D1GB-Ordner
5. Erstellen Sie einen umfassenden D1GB-Analysereport `d1gb_analysis_report.txt` mit:
   - Gesamtzahl und -größe aller Dateien
   - Top 10 größte und kleinste Dateien
   - Häufigste Dateierweiterungen
   - Statistiken über Zeilenzahlen
   - Identifizierte Probleme oder Anomalien

**Bonus**: Finden Sie Duplikate oder sehr ähnliche Dateien im D1GB-Ordner

**Ihre Aufgaben**:

1. Zeigen Sie nur die ERROR-Meldungen aus der Log-Datei
2. Zählen Sie, wie viele WARNING-Meldungen es gibt
3. Erstellen Sie eine Liste aller Benutzer, die sich eingeloggt haben (ohne Duplikate)
4. Finden Sie alle Log-Einträge zwischen 10:17:00 und 10:18:00
5. Erstellen Sie einen Report `log_summary.txt` mit:
   - Gesamtzahl der Log-Einträge
   - Anzahl INFO, WARNING, ERROR Meldungen
   - Liste der gefundenen Benutzer

---

## Aufgabe 8: Reflexion und Dokumentation

### 8.1 Kommando-Dokumentation

Erstellen Sie eine Datei `kommandos_cheatsheet.txt` mit:

- Den 10 wichtigsten Kommandos, die Sie gelernt haben
- Kurze Erklärung, was jedes Kommando macht
- Ein praktisches Beispiel für jedes Kommando

### 8.2 Reflexion

Erstellen Sie eine Datei `reflexion.txt` mit Antworten auf:

1. Was war die schwierigste Aufgabe und warum?
2. Welches Kommando fanden Sie am nützlichsten?
3. Wie könnte Unix/Linux in Ihrem IoT-Studium hilfreich sein?
4. Welche Bereiche möchten Sie vertiefen?

---

## Bonusaufgabe: D1GB-Automatisierung

Erstellen Sie ein Bash-Script `d1gb_analyzer.sh` das:

1. Alle D1GB-Textdateien automatisch analysiert
2. Einen täglichen Report mit Dateistatistiken erstellt
3. Problematische Dateien (z.B. leer, zu groß, ungewöhnlich) identifiziert
4. Ein Backup der wichtigsten/größten D1GB-Dateien erstellt
5. Eine Zusammenfassung ausgibt (Gesamtzahl Dateien, Gesamtgröße, gefundene Probleme)

6. Alle `.txt`-Dateien in `unix_uebung` findet
7. Ein Backup-Verzeichnis mit aktuellem Timestamp erstellt
8. Alle `.txt`-Dateien dorthin kopiert
9. Eine Zusammenfassung ausgibt (Anzahl kopierte Dateien, Zielordner)

**Hinweise**:

- Beginnen Sie das Script mit `#!/bin/bash`
- Machen Sie es ausführbar mit `chmod +x cleanup.sh`
- Testen Sie es mit `./cleanup.sh`

---

## Abgabe

### Was soll abgegeben werden:

- Keine Abgabe

### Bewertungskriterien:

- **Vollständigkeit**: Wurden alle Aufgaben bearbeitet?
- **Korrektheit**: Funktionieren die Kommandos?
- **Dokumentation**: Sind die Lösungen gut dokumentiert?

### Bewertung:

- **Sehr gut**: Alle Aufgaben vollständig und korrekt gelöst
- **Gut**: Meiste Aufgaben korrekt, kleine Fehler
- **Befriedigend**: Grundlegende Aufgaben korrekt
- **Ausreichend**: Minimale Anforderungen erfüllt
- **Nicht ausreichend**: Wesentliche Lücken

**Abgabetermin**: Keine Abgabe

**Viel Erfolg bei den Übungen!**

---

## Hilfreiche Ressourcen

- `man command` - Manualpage für jedes Kommando
- `command --help` - Schnelle Hilfe
- [Linux Command Line Cheat Sheet](https://www.linuxtrainingacademy.com/linux-commands-cheat-sheet/)
- [Vim Cheat Sheet](https://vim.rtorr.com/)

**Bei Problemen**: Fragen Sie Ihren Dozenten oder Kommilitonen!
