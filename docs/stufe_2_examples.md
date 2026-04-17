# Stufe 2 – Drei typische Projektbeispiele für KMU

Diese Beispiele liegen genau in dem Bereich, in dem viele bestehende Tools bereits vorhanden sind und nur sauber miteinander verbunden werden müssen.  
Das Ziel ist nicht, neue Insellösungen zu bauen, sondern vorhandene Systeme so zu verknüpfen, dass ein einheitlicher Prozess entsteht.  
Darüber liegt ein klares Streamlit-Dashboard als Steuerungs- und Kontrollschicht.

---

# Beispiel 1: Buchhaltung & Finanzen – Rechnungseingang, Freigabe und Zahlungsübersicht

## Ursprüngliches Problem

In vielen KMU laufen Eingangsrechnungen über verschiedene Kanäle:

- E-Mail
- Scan-Ordner
- Lieferantenportale
- manuelle Weiterleitungen im Unternehmen

Die Folge ist meist:

- Rechnungen werden manuell geöffnet und weitergeleitet
- Beträge werden abgetippt
- Freigaben passieren per E-Mail oder Zuruf
- Buchhaltung und Fachabteilung arbeiten an unterschiedlichen Ständen
- niemand sieht sofort, wo eine Rechnung gerade hängt

## Aufgabe

Einen sauberen End-to-End-Prozess schaffen:

1. Rechnungseingang zentral erfassen  
2. Daten automatisch auslesen  
3. Freigabe automatisch anstoßen  
4. Buchhaltung oder ERP sauber versorgen  
5. Status jederzeit sichtbar machen

## Typische Systeme beim Kunden

- Outlook oder Microsoft 365
- Shared Mailbox
- SharePoint oder Netzlaufwerk
- DATEV, Lexoffice, sevDesk oder ERP
- Teams oder Slack für Benachrichtigungen
- Excel-Listen als Nebenrealität

## Wie die Stufe-2-Lösung konkret aussieht

### Eingang

Eine Rechnung kommt per E-Mail oder Upload rein.

Ein Workflow-Tool wie n8n, Make oder Power Automate erkennt:

- neue E-Mail mit Anhang
- Dateityp PDF
- Absender
- Schlüsselwörter wie Rechnung, Invoice, Faktura

### Verarbeitung

Das Dokument wird an OCR oder eine Dokumentenerkennung gegeben.

Dabei werden typischerweise ausgelesen:

- Lieferant
- Rechnungsnummer
- Datum
- Betrag
- Fälligkeit
- IBAN
- Referenznummer
- Kostenstelle, falls vorhanden

### Prüfung

Danach laufen Standardregeln:

- Dublette vorhanden?
- Betrag über Freigabegrenze?
- Lieferant bekannt?
- Pflichtfelder vollständig?
- Zahlungsziel plausibel?

### Übergabe

Je nach Ergebnis:

- Standardfall wird direkt an Buchhaltung oder ERP übergeben
- Freigabefall geht an zuständige Person
- Fehlerfall landet in einer Klärfall-Liste

### Nachverfolgung

Status wird laufend aktualisiert:

- Eingang
- Erkannt
- In Prüfung
- Freigegeben
- Verbucht
- Abgeschlossen

## Welche Tools typischerweise miteinander verbunden werden

- Outlook / Gmail
- OCR-Dienst
- SharePoint / Drive / Netzlaufwerk
- DATEV / ERP / Buchhaltungssoftware
- Teams / Slack
- Excel / Airtable als Übergangslage
- Streamlit als Überwachungsoberfläche

## Wie das Streamlit-Dashboard aussehen sollte

### Oben

- Eingänge heute
- offene Freigaben
- überfällige Rechnungen
- automatisch verarbeitete Rechnungen
- Fehlerquote

### Mitte

Eine Prozessansicht als Kette:

Eingang → OCR → Prüfung → Freigabe → Verbuchung → Archiv

Jeder Schritt bekommt:

- Anzahl Fälle
- Erfolgsrate
- durchschnittliche Laufzeit
- Fehlerstatus

### Arbeitsliste

- Rechnungen warten auf Freigabe
- OCR unsicher
- Dublette erkannt
- Bankverbindung neu
- Abweichender Betrag

### Audit-Log

- wann die Rechnung einging
- wann OCR lief
- wer freigegeben hat
- wann das ERP befüllt wurde
- was fehlgeschlagen ist

### Managementsicht

- Durchlaufzeit pro Rechnung
- Zeitersparnis pro Monat
- Anteil automatisch verarbeiteter Rechnungen
- Freigabestau nach Abteilung
- Lieferanten mit den meisten Problemen

## Warum das genau Stufe 2 ist

Hier wird nicht individuell programmiert, sondern vorhandene Infrastruktur wird verbunden:

- OCR liest
- Workflow steuert
- ERP bekommt Daten
- Dashboard zeigt den Zustand

Das ist ein klassisches Integrationsprojekt mit klarer Rendite.

---

# Beispiel 2: Vertrieb, Marketing und Kundenservice – Lead-to-CRM, Follow-up und Ticket-Routing

## Ursprüngliches Problem

Leads, Anfragen und Kundenreaktionen kommen über viele Kanäle herein:

- Website-Formulare
- E-Mail
- LinkedIn
- Kontaktformulare
- Support-Mailboxen
- Chattools

Danach passiert oft:

- manuelle Übertragung ins CRM
- doppelte Datensätze
- verspätete Rückmeldung
- unklare Zuständigkeiten
- Follow-ups werden vergessen
- Support-Anfragen landen bei der falschen Person

## Aufgabe

Eingänge automatisch erfassen, zuordnen, priorisieren und an den richtigen Prozess übergeben.

## Typische Systeme beim Kunden

- HubSpot, Pipedrive, Salesforce, Zoho
- Outlook oder Gmail
- Website-Formularsysteme
- Chat-Widget
- Ticketsystem wie Zendesk oder Freshdesk
- Teams oder Slack
- Kalender und Terminbuchungstools
- Excel oder Airtable als Zwischenebene

## Wie die Stufe-2-Lösung konkret aussieht

### Lead-Eingang

Neue Leads aus Formular, Mail oder Import landen im Workflow.

### Vorprüfung

Der Workflow prüft:

- Ist das ein echter Lead oder Spam?
- Ist die Mailadresse gültig?
- Gibt es den Kontakt schon?
- Kommt die Anfrage aus einer Zielregion?
- Welche Produktkategorie ist gemeint?

### Routing

Je nach Inhalt wird automatisch entschieden:

- Vertrieb A oder Vertrieb B
- Verkauf oder Support
- hohe oder normale Priorität
- Demo oder Rückfrage
- Erstkontakt oder Bestandskunde

### Follow-up

Automatische Aktionen können sein:

- CRM-Datensatz anlegen
- Tag vergeben
- Aufgabe erzeugen
- Eingangsbestätigung senden
- Terminlink verschicken
- Erinnerung nach 2 Tagen setzen
- Ticket an Support übergeben

### Marketing-Verknüpfung

Wenn passend, wird der Lead zusätzlich in Marketing-Automationen übergeben:

- Newsletter-Liste
- Nurturing-Sequenz
- Segmenttag
- Kampagnenquelle

## Welche Tools typischerweise miteinander verbunden werden

- Webformulare
- E-Mail-Postfächer
- CRM
- Terminbuchung
- Ticket-System
- E-Mail-Automation
- Teams / Slack
- Streamlit als Steuerungs- und Transparenzschicht

## Wie das Streamlit-Dashboard aussehen sollte

### Oben

- Leads heute
- qualifizierte Leads
- offene Follow-ups
- Antwortzeit
- Conversion pro Quelle

### Mitte

Pipeline-Ansicht:

Eingang → Prüfung → Routing → CRM → Follow-up → Abschluss

Je Stufe:

- Durchsatz
- offene Vorgänge
- Fehler
- durchschnittliche Zeit

### Arbeitsliste

- neue Leads
- Dubletten
- unvollständige Anfragen
- Leads ohne Zuweisung
- Support-Tickets mit Eskalation

### Aktivitätsbereich

- neuer Lead eingegangen
- Mail bestätigt
- Aufgabe erstellt
- Termin gebucht
- Ticket verschoben
- Follow-up fällig

### Managementsicht

- Quelle mit bester Conversion
- Reaktionszeit nach Team
- Anzahl nicht bearbeiteter Leads
- Umsatzpotenzial in der Pipeline
- Supportlast pro Kategorie

## Warum das genau Stufe 2 ist

Hier werden Standardtools miteinander verkettet:

- Formular erzeugt Eingang
- Workflow prüft und routet
- CRM speichert
- Kalender oder Supportsystem reagiert
- Dashboard zeigt alles einheitlich

Das ist keine neue Softwarewelt, sondern eine saubere Orchestrierung vorhandener Systeme.

---

# Beispiel 3: Personalwesen und Recruiting – Bewerbungen, Terminierung und Onboarding

## Ursprüngliches Problem

HR-Prozesse laufen in vielen KMU noch halb manuell:

- Bewerbungen kommen per E-Mail
- Lebensläufe werden manuell gesichtet
- Termine werden per Mail hin- und hergeschrieben
- Zusagen und Absagen werden einzeln verschickt
- Onboarding-Unterlagen liegen verstreut
- IT, HR und Fachabteilung arbeiten nicht synchron

## Aufgabe

Bewerbungs- und Onboarding-Prozesse standardisieren, beschleunigen und nachvollziehbar machen.

## Typische Systeme beim Kunden

- Outlook oder Gmail
- Bewerbermanagement-System
- Kalender
- SharePoint oder Drive
- HR-Software
- Teams oder Slack
- Formularsysteme für interne Anträge
- E-Signatur-Lösungen

## Wie die Stufe-2-Lösung konkret aussieht

### Bewerbungseingang

Neue Bewerbungen werden automatisch aus Mail oder Formular gelesen.

### Erste Verarbeitung

Der Workflow erkennt:

- Name
- Position
- E-Mail
- Lebenslauf-Anhang
- gewünschte Stelle
- Eingangsdatum

### Sortierung

Danach wird automatisch entschieden:

- welche Position betroffen ist
- ob Unterlagen vollständig sind
- ob eine Antwort sofort verschickt werden kann
- ob jemand aus HR manuell prüfen muss

### Terminierung

Wenn die Bewerbung passt:

- Kalenderlink senden
- Interviewtermin vorschlagen
- Erinnerungen setzen
- Bestätigung versenden

### Onboarding

Nach Zusage werden automatisch angestoßen:

- Willkommensmail
- Onboarding-Checkliste
- IT-Anforderung
- Zugriffsanfrage
- Vertrags- oder Signaturworkflow
- interne Benachrichtigung an Fachbereich

## Welche Tools typischerweise miteinander verbunden werden

- E-Mail
- Bewerbermanagement-System
- Kalender
- HR-Ordner / Dokumentenablage
- E-Signatur
- Teams / Slack
- Onboarding-Checklisten
- Streamlit-Dashboard

## Wie das Streamlit-Dashboard aussehen sollte

### Oben

- Bewerbungen eingegangen
- offene Rückmeldungen
- Termine geplant
- Onboarding offen
- durchschnittliche Reaktionszeit

### Mitte

Prozesskette:

Bewerbung → Prüfung → Terminierung → Entscheidung → Onboarding

Mit Kennzahlen pro Schritt:

- Anzahl Vorgänge
- Zeit bis Antwort
- offene Fälle
- Fehlerquote

### Arbeitsliste

- unvollständige Bewerbungen
- Interview offen
- Absage offen
- Onboarding nicht gestartet
- Signatur fehlt

### HR-Sicht

- Bewerbungen pro Stelle
- Zeit bis zum Erstkontakt
- Interviewquote
- Zusagequote
- offene Onboarding-Schritte

### Audit-Log

- wann Bewerbung kam
- wann sie geprüft wurde
- wann der Termin versendet wurde
- wann die Zusage oder Absage erfolgte
- wann Onboarding ausgelöst wurde

## Warum das genau Stufe 2 ist

Auch hier gilt:

- vorhandene Tools bleiben bestehen
- Prozesse werden verbunden
- manuelle Übergaben werden reduziert
- das Dashboard macht die Strecke sichtbar

Das ist genau die Art von Projekt, bei der ein schlankes Integrations- und Steuerungsmodell den größten Hebel bringt.

---

# Gemeinsames Muster aller drei Projekte

## Was du faktisch verkaufst

Nicht nur Automation.

Sondern:

- Systemverbindung
- Prozesssicht
- Fehlerkontrolle
- einheitliche Steuerung
- ein zentrales Dashboard

## Was das Dashboard immer können sollte

- Live-Status anzeigen
- Klärfälle sichtbar machen
- Prozessschritte messen
- Ausnahmen auflisten
- Audit-Logs zeigen
- Einsparungen grob beziffern

## Typische Kennzahlen

- Durchsatz
- offene Fälle
- Laufzeit pro Vorgang
- Fehlerquote
- manuelle Eingriffe
- Automationsgrad
- Status je Quelle oder Kanal

## Die passende Positionierung

Das ist kein klassisches Softwareprojekt.

Es ist ein Integrationsprojekt mit Steuerungsebene.

Genau dort liegt der Sweet Spot:

- vorhandene Tools bleiben
- Prozesse werden verbunden
- Management bekommt Übersicht
- operative Arbeit sinkt
- Kunden sehen schnell messbaren Nutzen
