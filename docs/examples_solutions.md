# Automatisierungslösungen mit Problem, Aufgabe und Dashboard-Darstellung

---

# 1. Sales Lead Handling

## Ursprüngliches Problem

Neue Leads kommen über mehrere Kanäle herein:

- Website-Formular
- Kontaktanfragen per E-Mail
- LinkedIn-Nachrichten
- Empfehlungen
- Telefonische Erstkontakte

In vielen kleinen und mittleren Unternehmen passiert danach Folgendes:

- Leads landen verteilt in mehreren Postfächern
- Niemand hat eine Gesamtübersicht
- Daten werden manuell übertragen
- Rückrufe erfolgen zu spät
- Zuständigkeiten sind unklar
- Manche Leads gehen verloren
- Priorisierung erfolgt nach Bauchgefühl

## Aufgabe

Ein verlässlicher, nachvollziehbarer Lead-Prozess:

1. Jeder Lead wird erfasst  
2. Kein Lead geht verloren  
3. Standardfälle laufen schnell  
4. Zuständigkeiten sind klar  
5. Vertrieb arbeitet nur an relevanten Leads  
6. Management sieht Kennzahlen live

---

# 1A – Sichtbarkeit & Kontrolle

## Ziel

Chaos beseitigen und erstmals Transparenz schaffen.

Noch keine komplexe Automatisierung.  
Erst wird der Prozess sichtbar gemacht.

## Wie die Lösung konkret aussieht

### Eingangskanäle bleiben zunächst bestehen:

- Formular bleibt Formular
- E-Mail bleibt E-Mail
- LinkedIn bleibt LinkedIn

### Lead-Erfassung erfolgt zentral

Es gibt nun **ein zentrales Lead-Board** in:

- Google Sheets
- Airtable
- Notion Database
- Excel Online

### Zwei mögliche Varianten

## Variante A – manuelle Eintragung

Mitarbeiter trägt neue Leads ein:

- Name
- Firma
- Kontaktweg
- Interesse
- Datum
- Status
- Zuständig

Diese Variante ist oft sinnvoll zum Start, weil sie extrem schnell umsetzbar ist.

## Variante B – halbautomatische Erfassung

Wenn Website-Formular vorhanden:

- Formular sendet automatisch in Sheet/Airtable

E-Mails und LinkedIn weiterhin manuell.

Das ist oft der beste Mittelweg.

## Beispiel-Prozess

1. Lead kommt per Website rein  
2. Eintrag landet automatisch im Board  
3. E-Mail-Lead wird manuell ergänzt  
4. Vertrieb sieht neue Leads sofort  
5. Lead erhält Status „Neu“

## Typische Statuswerte

- Neu
- Kontaktiert
- Termin vereinbart
- Qualifiziert
- Kein Interesse
- Gewonnen
- Verloren

## Dashboard in 1A

### KPI oben

- Leads heute
- Neue Leads offen
- Durchschnittliche Erstreaktion
- Leads diese Woche

### Hauptliste

| Name | Firma | Quelle | Status | Zuständig |
|------|------|------|------|------|

### Rechte Seite

- letzte neue Leads
- unbearbeitete Leads > 24h
- Top-Quellen

## Nutzen

- Kein Lead verschwindet
- Sofort Übersicht
- Erste Kennzahlen entstehen
- Grundlage für Phase 1B

---

# 1B – Standardisierung & Stabilität

## Ziel

Nicht nur sichtbar, sondern reproduzierbar.

Der Prozess funktioniert nun unabhängig davon, wer arbeitet.

## Wie die Lösung konkret aussieht

## Einheitliche Pflichtfelder

Jeder Lead braucht:

- Name
- Firma
- E-Mail oder Telefon
- Quelle
- Interesse
- Region
- Größe des Unternehmens
- Priorität

## Feste Regeln

### Beispiel Lead-Zuweisung

Wenn Region = Süddeutschland → Mitarbeiter A  
Wenn Region = Norddeutschland → Mitarbeiter B

### Beispiel Priorität

Wenn Firma > 50 Mitarbeiter → Hoch  
Wenn Demo-Anfrage → Hoch  
Wenn nur allgemeine Frage → Mittel

## Kommunikationsvorlagen

- Erstkontakt-Mail
- Terminvereinbarung
- Absage
- Nachfrage nach fehlenden Infos

## Bearbeitungsstandard

Jeder neue Lead muss:

- innerhalb 24h kontaktiert werden
- vollständig bewertet werden
- dokumentiert werden

## Beispiel-Prozess

1. Neuer Lead kommt rein  
2. Pflichtfelder geprüft  
3. Priorität gesetzt  
4. Zuständigkeit festgelegt  
5. Vertrieb arbeitet nach klarer Reihenfolge

## Dashboard in 1B

### KPI

- Vollständige Leads %
- Leads ohne Bearbeitung >24h
- Hochpriorisierte Leads offen
- Reaktionszeit

### Qualitätsansicht

- fehlende Telefonnummer
- keine Zuständigkeit
- Dubletten
- veraltete Leads

### Vertriebsübersicht

- Leads pro Mitarbeiter
- Conversion pro Quelle
- Reaktionszeiten pro Person

## Nutzen

- Weniger Chaos
- Höhere Geschwindigkeit
- Gleiche Qualität
- Messbarer Vertrieb

---

# 1C – Teilautomatisierung

## Ziel

Erste echte Zeitersparnis ohne große Systemlandschaft.

## Wie die Lösung konkret aussieht

## Automatische Eingänge

### Website

Lead geht automatisch ins Board.

### E-Mail

System erkennt neue Lead-Mails anhand:

- Betreff
- Keywords
- Formulartext
- Absender

### LinkedIn

Manuell oder via Export.

## Automatische Vorverarbeitung

System befüllt:

- Name
- Firma
- Mailadresse
- Quelle
- Eingangsdatum

## Automatische Regeln

### Beispiel

Wenn Region = Bayern → Sales Süd  
Wenn Branche = Industrie → Tag setzen  
Wenn Demo gewünscht → Priorität hoch

## Automatische Aktionen

- Bestätigungs-E-Mail senden
- Aufgabe im CRM anlegen
- Slack / Teams Nachricht
- Follow-up Erinnerung

## Ausnahmefälle

Unvollständige Leads landen in:

**Klärfall-Liste**

## Beispiel-Prozess

1. Formular kommt rein  
2. Datensatz wird erstellt  
3. Priorität wird gesetzt  
4. Zuständiger Mitarbeiter wird informiert  
5. Kunde erhält Eingangsbestätigung  
6. Sonderfälle gehen in Prüfung

## Dashboard in 1C

### KPI

- Automatisch verarbeitet %
- Klärfälle offen
- Neue Leads letzte 24h
- Durchschnitt bis Erstkontakt

### Arbeitsliste

- Auto-Zugewiesen
- Wartet auf Bearbeitung
- Klärfall
- Erledigt

### Prozessanzeige

Eingang → Bewertung → Zuweisung → Kontakt

## Nutzen

- Weniger Admin-Arbeit
- Schnellere Reaktion
- Mehr Leads bearbeitet
- Mitarbeiter arbeiten nur noch an echten Fällen

---

# Phase 2 – Workflow-Automation mit Standardtools

## Ziel

Komplette Lead-Strecken automatisieren.

## Tools

- n8n
- Make
- Zapier
- Power Automate

## Wie die Lösung konkret aussieht

## Beispiel-Ablauf

1. Lead kommt via Formular oder Mail  
2. Workflow startet automatisch  
3. Dublettenprüfung  
4. Datenanreicherung (Website / Branche / Größe)  
5. CRM-Eintrag erzeugen  
6. Sales Owner zuweisen  
7. Sequenz-Mail senden  
8. Reminder erzeugen  
9. Dashboard aktualisieren

## Erweiterungen

- Kalenderlink senden
- Terminbuchung automatisch
- Lead Scoring
- CRM Tags setzen
- Follow-up nach 3 Tagen

## Dashboard in Phase 2

### KPI

- Conversion nach Quelle
- Leads pro Kampagne
- Automationsquote
- SLA eingehalten %
- Termine gebucht

### Funnel

Neu → Qualifiziert → Termin → Angebot → Kunde

### Fehlercenter

- Dublette erkannt
- CRM Fehler
- Fehlende Mailadresse
- API Fehler

## Nutzen

- Skalierbarer Vertrieb
- Weniger manuelle Übergaben
- Schnelleres Follow-up
- Bessere Conversion

---

# Phase 3 – Lokale Speziallösung

## Ziel

Wenn Standardtools nicht reichen.

## Wann nötig

- Chaotische Lead-Quellen
- Alte Systeme ohne API
- Komplexe Angebotslogik
- Eigene Matching-Regeln
- Datenschutz intern erforderlich

## Wie die Lösung konkret aussieht

## Beispiel

Lokaler Python-Service liest:

- Outlook Postfach
- CSV Uploads
- Website Exporte
- Excel-Dateien

Dann:

1. Erkennt Leads intelligent  
2. Extrahiert Daten  
3. Prüft Dubletten  
4. Bewertet Potenzial  
5. Erstellt Importdatei fürs CRM  
6. Schreibt Logs

## Erweiterte Funktionen

- Eigener Lead Score
- Branchenklassifizierung
- Umsatzschätzung
- Matching nach Vertriebsstärke
- Region + Produkt + Sprache Routing

## Dashboard in Phase 3

### KPI

- Parser-Erfolgsrate
- Import erfolgreich
- Sonderfälle
- Verarbeitungszeit

### Technische Ansicht

- letzte Jobs
- erkannte Fehler
- Dateiformatprobleme
- Quelle mit meisten Problemen

### Managementsicht

- Beste Lead-Quellen
- Umsatzpotenzial offen
- Team-Auslastung
- Abschlusswahrscheinlichkeit

## Nutzen

- Maximale Kontrolle
- Verarbeitung schwieriger Inputs
- Interne Daten bleiben intern
- Maßgeschneiderter Vertriebsmotor

---

# Empfohlener Kundenweg

## Kleine Firma / Start

1A → 1B → 1C

## Wachsender Vertrieb

1C → Phase 2

## Komplexes Unternehmen

Phase 2 + Phase 3

---

# Wichtiger Verkaufsansatz

Nicht verkaufen:

„Wir bauen Automationen.“

Sondern verkaufen:

- Kein Lead geht verloren
- Schnellere Reaktion
- Mehr Termine
- Bessere Conversion
- Klare Vertriebssteuerung
- Weniger Admin-Aufwand

# 2. Supplier Invoice Intake

## Ursprüngliches Problem

Rechnungen kommen über viele Wege ins Unternehmen:

- per E-Mail als PDF
- als Scan
- per Post eingescannt
- als Sammelanhänge
- von verschiedenen Lieferanten mit unterschiedlichen Layouts

Danach passiert häufig:

- Mitarbeiter öffnen jede Mail manuell
- Anhänge werden heruntergeladen
- Dateien werden umbenannt
- Rechnungsdaten werden abgetippt
- Beträge werden kontrolliert
- Lieferanten werden geprüft
- Rechnungen werden ins ERP / Buchhaltungssystem übertragen
- Freigaben laufen per Zuruf oder Mail

Das kostet Zeit, erzeugt Fehler und ist schlecht skalierbar.

---

## Aufgabe

Ein zuverlässiger Rechnungseingangsprozess:

1. Jede Rechnung wird erfasst  
2. Nichts geht verloren  
3. Standardfälle laufen schnell  
4. Fehler werden früh erkannt  
5. Freigaben sind nachvollziehbar  
6. Management sieht Status und Volumen live

---

# 1A – Sichtbarkeit & Kontrolle

## Ziel

Zuerst Übersicht schaffen.  
Nicht sofort automatisieren.

## Wie die Lösung konkret aussieht

## Eingang bleibt zunächst wie bisher

- E-Mail bleibt E-Mail
- Scan bleibt Scan
- Postscan bleibt Postscan

## Zentrale Sammelstelle

Alle Rechnungen laufen an einen zentralen Ort:

- rechnung@firma.de
- Shared Mailbox
- Netzwerkordner
- SharePoint-Ordner

## Erfassung in Übersichtsliste

Google Sheets / Airtable / Excel Online:

- Eingangsdatum
- Lieferant
- Rechnungsnummer
- Betrag
- Status
- Zuständig
- Fälligkeitsdatum

## Wie erfolgt die Datenerfassung?

### Variante A – manuell

Mitarbeiter öffnet Rechnung und trägt Werte ein.

Sinnvoll bei geringem Volumen.

### Variante B – halbmanuell

Datei landet automatisch im Ordner, Mitarbeiter ergänzt nur Daten.

Sehr realistischer Start.

## Beispiel-Prozess

1. Rechnung kommt per Mail  
2. Datei landet im zentralen Postfach  
3. Mitarbeiter trägt Daten ein  
4. Status = Neu  
5. Buchhaltung arbeitet Liste ab

## Dashboard in 1A

### KPI

- Rechnungen heute
- Offene Rechnungen
- Überfällige Freigaben
- Eingänge diese Woche

### Hauptliste

- Lieferant
- Betrag
- Eingang
- Status
- Zuständig

### Warnungen

- Rechnung > 7 Tage offen
- fehlender Betrag
- keine Zuständigkeit

## Nutzen

- Keine verlorenen Rechnungen
- Übersicht statt Postfach-Chaos
- Basisdaten verfügbar
- Grundlage für Standardisierung

---

# 1B – Standardisierung & Stabilität

## Ziel

Rechnungseingang funktioniert sauber und einheitlich.

## Wie die Lösung konkret aussieht

## Pflichtfelder

Jede Rechnung braucht:

- Lieferant
- Rechnungsnummer
- Datum
- Betrag
- Kostenstelle
- Freigabe nötig ja/nein
- Fälligkeitsdatum

## Klare Regeln

### Beispiel

Wenn Betrag < 500 € → direkte Buchhaltung  
Wenn Betrag > 500 € → Freigabe Teamleiter

Wenn Lieferant unbekannt → Prüfung

Wenn doppelte Rechnungsnummer → Sperre

## Einheitliche Ablage

Dateinamen:

YYYY-MM-DD_Lieferant_Rechnungsnummer.pdf

## Checklisten

Mitarbeiter prüft:

- Ist Rechnung lesbar?
- Betrag plausibel?
- Lieferant bekannt?
- USt enthalten?
- Dublette?

## Beispiel-Prozess

1. Rechnung kommt rein  
2. Daten werden eingetragen  
3. Regeln geprüft  
4. Freigabe wenn nötig  
5. Übergabe an Buchhaltung

## Dashboard in 1B

### KPI

- Vollständige Rechnungen %
- Rechnungen ohne Kostenstelle
- Dubletten erkannt
- Freigaben offen

### Qualitätsübersicht

- unbekannte Lieferanten
- fehlende Rechnungsnummern
- fehlende Fälligkeit
- fehlerhafte Dateien

## Nutzen

- Weniger Rückfragen
- Weniger Fehler
- Saubere Prozesse
- Revisionsnäher

---

# 1C – Teilautomatisierung ohne Systembruch

## Ziel

Erste Zeitersparnis ohne großes ERP-Projekt.

---

## Wie die Lösung konkret aussieht

## Automatische Vorsortierung

Neue E-Mails mit:

- PDF-Anhang
- Begriffen wie Rechnung, Invoice, Faktura
- bekannten Lieferanten-Absendern

werden automatisch markiert oder verschoben.

## Wie werden Patterns erkannt ohne Programmierung?

Mit No-Code / Low-Code Regeln:

### Beispiel in Power Automate / Make / n8n

Wenn:

- Betreff enthält „Rechnung“
- Anhang endet auf .pdf
- Absenderdomain = lieferant.de

Dann:

→ In Rechnungseingang verschieben

### Weitere einfache Muster

Wenn Lieferant Müller GmbH:

→ immer Kostenstelle Einkauf

Wenn Betrag im Betreff enthalten:

→ markieren

Wenn PDF mehr als 10 Seiten:

→ Sonderfall

Das ist regelbasiert, keine klassische Programmierung.

---

## Wie werden Beträge erkannt?

## Variante A – OCR + Texterkennung

Tools lesen Text aus PDF:

- Microsoft AI Builder
- Google OCR
- PDF Parser
- Make OCR Module
- n8n OCR Integrationen

Dann wird nach Mustern gesucht:

- Gesamtbetrag
- Summe
- Total
- EUR
- €

## Beispiel

Im PDF steht:

Gesamtbetrag: 1.245,00 €

Tool erkennt:

1.245,00

## Variante B – feste Lieferantenlayouts

Wenn Lieferant immer dieselbe Rechnung nutzt:

Betrag steht z.B. rechts unten.

Dann kann gezielt gelesen werden.

## Variante C – halbautomatisch

System schlägt Betrag vor, Mensch bestätigt.

---

## Welche Felder lassen sich oft automatisch erkennen?

- Lieferant
- Rechnungsnummer
- Datum
- Nettobetrag
- Bruttobetrag
- USt
- IBAN
- Zahlungsziel

---

## Automatische Aktionen

- Datei umbenennen
- In richtigen Ordner verschieben
- Datensatz anlegen
- Freigabe an Verantwortlichen senden
- Buchhaltung informieren

## Ausnahmefälle

Gehen in:

**Klärfall-Liste**

z.B.:

- Betrag nicht erkannt
- Dublette vermutet
- Unbekannter Lieferant
- Schlechter Scan

---

## Beispiel-Prozess

1. Rechnung kommt per Mail  
2. PDF erkannt  
3. Betrag + Datum extrahiert  
4. Lieferant erkannt  
5. Datensatz angelegt  
6. Standardfall geht weiter  
7. Sonderfall landet in Prüfung

---

## Dashboard in 1C

### KPI

- Automatisch vorbereitet %
- Manuelle Klärfälle
- Durchschnittliche Bearbeitungszeit
- Heute verarbeitet

### Arbeitsliste

- Wartet auf Freigabe
- OCR prüfen
- Dublette prüfen
- Fertig

### Prozessanzeige

Eingang → Erkennung → Prüfung → Freigabe

## Nutzen

- Weniger Tipparbeit
- Schnellere Verarbeitung
- Weniger Fehler
- Mitarbeiter prüfen nur Ausnahmen

---

# Phase 2 – Workflow-Automation mit Standardtools

## Ziel

Komplette digitale Rechnungseingangsstrecke.

## Tools

- n8n
- Make
- Zapier
- Power Automate
- DATEV / ERP Connectoren

---

## Beispiel-Ablauf

1. Rechnung kommt per Mail  
2. Workflow startet  
3. OCR liest PDF  
4. Dublettenprüfung  
5. Lieferant validieren  
6. Freigabe an Zuständigen  
7. Nach Freigabe Übergabe an ERP  
8. Dashboard aktualisieren

---

## Erweiterungen

- Erinnerungen bei Freigabeverzug
- Eskalation nach 3 Tagen
- Kostenstellenvorschläge
- Zahlungsziel überwachen
- Frühzahlerrabatt-Hinweise

---

## Dashboard in Phase 2

### KPI

- Durchsatz pro Tag
- Freigabezeit
- Automationsquote
- Überfällige Rechnungen
- Fehlerquote

### Pipeline

Eingang → OCR → Validierung → Freigabe → ERP → Archiv

### Fehlercenter

- OCR unsicher
- API Fehler
- Dublette
- Freigabe fehlt
- Lieferant unbekannt

## Nutzen

- Skalierbar
- Schnellere Freigaben
- Weniger Medienbrüche
- Transparenz

---

# Phase 3 – Lokale Speziallösung

## Ziel

Wenn Standardtools nicht reichen.

## Wann nötig?

- Viele Sonderformate
- Schlechte Scans
- Alte ERP-Systeme
- Kein Cloud-Wunsch
- Sehr individuelle Freigabelogik

---

## Wie die Lösung konkret aussieht

Lokaler Python-Service oder interner Dienst:

liest:

- Outlook Postfach
- Scan-Ordner
- CSV Uploads
- PDF Archive

Dann:

1. OCR + Parsing  
2. Lieferantenabgleich  
3. Betragsprüfung  
4. Dublettenprüfung  
5. Regelprüfung  
6. Importdatei erzeugen  
7. Audit-Log schreiben

---

## Erweiterte Speziallogik

- Prüfe ob Betrag stark vom Durchschnitt abweicht
- Prüfe ob Bankverbindung neu ist
- Prüfe ob gleiche Rechnung schon existiert
- Erkenne typische Betrugsmuster
- Routing nach Abteilung

---

## Dashboard in Phase 3

### KPI

- Parser-Erfolgsrate
- Import erfolgreich
- Sonderfälle offen
- Durchschnittliche Laufzeit

### Technische Ansicht

- Letzte Jobs
- OCR Qualität
- Fehlerhafte PDFs
- Lieferanten mit Problemen

### Managementsicht

- Volumen pro Lieferant
- Bearbeitungszeit
- Freigabestau
- Zahlungsfristen

## Nutzen

- Maximale Kontrolle
- Interne Daten bleiben intern
- Verarbeitung schwieriger Fälle
- Maßgeschneiderte Logik

---

# Empfohlener Kundenweg

## Kleine Firma

1A → 1B → 1C

## Wachsendes Unternehmen

1C → Phase 2

## Komplexe Buchhaltung

Phase 2 + Phase 3

---

# Wichtiger Verkaufsansatz

Nicht verkaufen:

„Wir automatisieren Rechnungen.“

Sondern verkaufen:

- Keine verlorenen Rechnungen
- Schnellere Freigaben
- Weniger Tippfehler
- Transparente Zahlungsprozesse
- Weniger Stress im Monatsabschluss

# 3. Reporting for Management

## Ursprüngliches Problem

Management-Berichte entstehen in vielen Unternehmen manuell aus mehreren Quellen:

- CRM
- ERP
- Buchhaltung
- Excel-Dateien
- CSV-Exporte
- Marketing-Tools
- manuelle Listen

Danach passiert oft:

- Daten werden exportiert
- Tabellen kopiert
- Zahlen zusammengeführt
- Fehler manuell korrigiert
- Charts neu gebaut
- Versionen per Mail verschickt
- Zahlen widersprechen sich
- Reports kommen verspätet

Zusätzlich entsteht Abhängigkeit:

- Nur eine Person weiß, wie der Bericht gebaut wird
- Bei Urlaub steht alles still
- Niemand vertraut den Zahlen vollständig

---

## Aufgabe

Ein zuverlässiger Reporting-Prozess:

1. Zahlen kommen aus klaren Quellen  
2. Kennzahlen sind einheitlich definiert  
3. Reports entstehen regelmäßig  
4. Fehler werden sichtbar  
5. Management hat Live-Übersicht  
6. Weniger Excel-Handarbeit

---

# 1A – Sichtbarkeit & Kontrolle

## Ziel

Zuerst Transparenz schaffen:

- Welche Reports gibt es?
- Wer erstellt sie?
- Welche Quellen werden genutzt?
- Wie lange dauert es?
- Wo treten Fehler auf?

Noch keine große Automatisierung.

---

## Wie die Lösung konkret aussieht

## Zentrales Reporting-Board

In:

- Google Sheets
- Airtable
- Excel Online
- Notion

werden alle Reports erfasst.

## Pro Report werden dokumentiert:

- Reportname
- Empfänger
- Rhythmus (wöchentlich / monatlich)
- Verantwortlich
- Datenquellen
- Letzter Versand
- Nächster Termin
- Status

## Beispiel

| Report | Turnus | Status |
|-------|-------|-------|
| Vertriebsreport | wöchentlich | offen |
| Monatszahlen | monatlich | in Arbeit |
| Marketing KPI | wöchentlich | fertig |

## Wie läuft der Prozess konkret?

1. Bestehende Reports werden gesammelt  
2. Quellen werden dokumentiert  
3. Ersteller festgelegt  
4. Deadlines sichtbar gemacht  
5. Fehlende Reports auffällig gemacht

## Dashboard in 1A

### KPI

- Reports diese Woche
- Überfällige Reports
- Datenquellen aktiv
- Reports in Arbeit

### Hauptliste

- Reportname
- Verantwortlich
- Nächster Termin
- Status

### Rechte Seite

- Letzte Updates
- Nächste Fälligkeiten
- Engpässe

## Nutzen

- Erstmals Übersicht
- Kein vergessener Report
- Verantwortlichkeiten klar
- Basis für Standardisierung

---

# 1B – Standardisierung & Stabilität

## Ziel

Reports sollen reproduzierbar werden.

Nicht jede Woche neue Zahlenlogik.

---

## Wie die Lösung konkret aussieht

## Einheitliche KPI-Definitionen

Beispiele:

### Umsatz

Immer netto?  
Immer brutto?  
Mit Retouren oder ohne?

### Leads

Nur neue Leads?  
Oder alle Kontakte?

### Conversion Rate

Welche Formel genau?

Das wird einmal definiert.

---

## Standardisierte Templates

Jeder Report erhält feste Struktur:

1. Executive Summary  
2. KPI-Block  
3. Trends  
4. Risiken  
5. Maßnahmen

## Feste Exportregeln

Beispiel:

CRM Export immer:

- letzter voller Monat
- gleiche Filter
- gleiche Regionen
- gleiche Spalten

## Verantwortlichkeiten

- Wer liefert Daten?
- Wer prüft?
- Wer versendet?

## Beispiel-Prozess

1. Datenquellen werden nach Standard exportiert  
2. Template wird genutzt  
3. Zahlen geprüft  
4. Versand

## Dashboard in 1B

### KPI

- Reports vollständig %
- Datenfehler
- Fehlende Quellen
- Pünktlich geliefert %

### Qualitätsansicht

- Quelle fehlt
- KPI unplausibel
- Datei verspätet
- Format falsch

### Managementansicht

- Alle Reports im Status
- Zuverlässigkeit je Bereich

## Nutzen

- Vergleichbare Zahlen
- Weniger Diskussionen
- Schnellere Erstellung
- Höheres Vertrauen

---

# 1C – Teilautomatisierung

## Ziel

Wiederkehrende Berichtsteile automatisch erzeugen.

---

## Wie die Lösung konkret aussieht

## Automatische Datenimporte

Beispiele:

- CSV wird automatisch eingelesen
- CRM Export wird importiert
- Buchhaltungsdatei wird übernommen
- Sheet aktualisiert sich

## Wie funktioniert das ohne große Programmierung?

Mit:

- Power Query in Excel
- Google Sheets Import-Funktionen
- Airtable Sync
- Make / Zapier / n8n
- Geplante CSV Imports

## Beispiel

Jeden Montag 07:00 Uhr:

- CRM CSV importieren
- Sheet aktualisieren
- Charts neu berechnen

---

## Automatische Berechnungen

- Umsatz vs Vorwoche
- Conversion Rate
- Offene Angebote
- Pipeline-Wert
- Kampagnenkosten

## Automatische Visualisierung

- Balkendiagramme
- Trendlinien
- Ampelstatus
- Top 5 Kunden
- Warnfelder

## Halbautomatisch

Management-Kommentar wird manuell ergänzt.

---

## Beispiel-Prozess

1. Quellen werden geladen  
2. Kennzahlen berechnet  
3. Charts aktualisiert  
4. Report steht bereit  
5. Mitarbeiter prüft kurz  
6. Versand

---

## Dashboard in 1C

### KPI

- Daten automatisch aktualisiert
- Reports bereit
- Fehlerhafte Quellen
- Letzte Aktualisierung

### Arbeitsliste

- Wartet auf Freigabe
- Kommentar fehlt
- Versand bereit
- Sonderfall prüfen

### Prozessanzeige

Import → Berechnung → Visualisierung → Freigabe

## Nutzen

- Stunden statt Minuten
- Weniger Excel-Arbeit
- Schnellere Reports
- Weniger Fehler

---

# Phase 2 – Workflow-Automation mit Standardtools

## Ziel

Komplette Reporting-Strecken automatisieren.

## Tools

- Power BI
- Looker Studio
- Google Sheets
- Excel Power Query
- Make
- n8n
- Power Automate

---

## Beispiel-Ablauf

1. CRM liefert Daten automatisch  
2. ERP liefert Daten automatisch  
3. Buchhaltung liefert Daten automatisch  
4. Workflow prüft Vollständigkeit  
5. Dashboard aktualisiert sich  
6. PDF Report wird erzeugt  
7. Automatischer Versand an Management

---

## Erweiterungen

- Slack / Teams Reportversand
- Montagmorgen Auto-Mail
- Abweichungswarnungen
- Zielerreichungsampel
- Forecast-Berechnung

---

## Dashboard in Phase 2

### KPI

- Datenquellen online
- Erfolgreiche Syncs
- Reports automatisch versendet
- Fehlerquote
- Aktualität in Minuten

### Pipeline

Quelle → Import → Prüfung → Dashboard → Versand

### Fehlercenter

- Quelle nicht erreichbar
- API Fehler
- Datei fehlt
- Unplausible Werte
- Sync abgebrochen

## Nutzen

- Management hat Live-Zahlen
- Kein manuelles Zusammenbauen
- Schnellere Entscheidungen
- Hohe Skalierbarkeit

---

# Phase 3 – Lokale Speziallösung

## Ziel

Wenn Standardtools nicht reichen.

---

## Wann nötig?

- Alte ERP-Systeme ohne API
- Lokale Datenbanken
- Viele Excel-Inseln
- Hohe Datenschutzanforderungen
- Sehr spezielle KPI-Logik
- Komplexe Forecastmodelle

---

## Wie die Lösung konkret aussieht

Lokaler Python-Service oder interner Datenprozess:

liest:

- SQL Datenbanken
- Excel-Dateien
- CSV Ordner
- ERP Exporte
- lokale Systeme

Dann:

1. Daten zusammenführen  
2. Dubletten entfernen  
3. KPI berechnen  
4. Forecast rechnen  
5. Dashboard aktualisieren  
6. PDF / Excel exportieren  
7. Logs schreiben

---

## Erweiterte Speziallogik

- Deckungsbeitrag pro Kunde
- Forecast auf Basis Historie
- Churn-Risiko
- Umsatzwarnsystem
- Pipeline-Wahrscheinlichkeiten
- Vertriebsranking

---

## Dashboard in Phase 3

### KPI

- Datenjobs erfolgreich
- Quellen synchronisiert
- Forecast aktualisiert
- Anomalien erkannt

### Technische Ansicht

- Letzte Jobs
- Laufzeiten
- Fehlerquellen
- Datenkonflikte

### Managementsicht

- Umsatztrend
- Forecast Monatsende
- Risiko-Kunden
- Zielerreichung
- Performance nach Team

## Nutzen

- Maßgeschneiderte Steuerung
- Interne Daten bleiben intern
- Komplexe Logik möglich
- Starke Entscheidungsbasis

---

# Empfohlener Kundenweg

## Kleines Unternehmen

1A → 1B → 1C

## Wachsendes Unternehmen

1C → Phase 2

## Komplexe Organisation

Phase 2 + Phase 3

---

# Wichtiger Verkaufsansatz

Nicht verkaufen:

„Wir bauen Reports.“

Sondern verkaufen:

- Schnellere Entscheidungen
- Verlässliche Zahlen
- Weniger Excel-Chaos
- Live-Übersicht fürs Management
- Früher Risiken erkennen
- Zeit sparen im Reporting

# Einheitliche Dashboard-Struktur für alle Kunden

## Kopfbereich

- Kundenname
- Systemname
- Live-Status
- Letzte Synchronisierung

## KPI-Reihe

- Eingänge heute
- Offene Klärfälle
- Automationsrate
- Fehlerquote
- Bearbeitungszeit

## Prozessübersicht

Eingang → Prüfung → Verarbeitung → Ausnahme → Fertig

## Arbeitsliste

- Neue Fälle
- In Bearbeitung
- Klärfälle
- Historie

## Aktivität / Audit-Log

- Was ist passiert
- Wann ist es passiert
- Wer hat ausgelöst
- Fehlerursache

## ROI-Bereich

- Zeit gespart pro Woche
- Weniger Fehler
- Schnellere Durchlaufzeit
- Entlastete Mitarbeiterstunden

---

# Verkaufslogik

Nicht verkaufen:

„Wir bauen Automatisierung.“

Sondern verkaufen:

1. Transparenz schaffen  
2. Prozess stabilisieren  
3. Erst dann automatisieren  
4. Ergebnisse messbar machen

---