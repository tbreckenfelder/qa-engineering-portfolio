## **Testplan & Testfalldesign**
**Testobjekt (zu testendes System):**

**Webshop: https://grocerymate.masterschool.com/**

***Ich verwende die zuvor formulierten Anforderungen als Grundlage für den Testplan.***

---
## **1. Produktanalyse**

**Zielsetzung: Was ist das Ziel des Produkts?**

- Das Hauptziel des Produkts ist die Erweiterung des bestehenden Shops um drei neue Funktionen (siehe unten) und die Gewährleistung der reibungslosen Funktion der bestehenden Funktionen.

**Zielgruppe (Stakeholder): Wer nutzt das Produkt? Wer sind die relevanten Stakeholder auf Nutzerseite?**

- Das Produkt richtet sich an neue und bestehende Nutzer der Plattform, unabhängig vom Alter, sowie an Nutzer ab 18 Jahren (für alkoholische Getränke).

**Hardware- und Software-Spezifikationen:** Es werden Geräte mit Standardkonfigurationen verwendet.


**Hardware-Anforderungen:**

- Geräte: PCs, Laptops, Smartphones, Tablets
- Mindestanforderungen: 4 GB RAM, 2-GHz-Prozessor

**Software-Anforderungen:**

- Betriebssysteme: Windows, macOS, Android, iOS
- Browser: Chrome, Firefox, Safari, Edge
- Abhängigkeiten: Backend-Dienste, Werbedienste von Drittanbietern, Zahlungsanbieter

**Bestehende Funktionen:**

Welche Funktionen bietet das Produkt – sowohl bestehende als auch geplante?

- Registrierung und Anmeldung
- Produktsuche mit Sortierfunktion (z. B. nach Preis), Produktkategorisierung
- Produkte zu Favoriten hinzufügen
- Produkte in den Warenkorb legen
- Bestellabwicklung: Rechnungs- und Lieferadresse eingeben, Zahlungsmethode auswählen, Gesamtbetrag berechnen

**Geplante Funktionen:**
- Produktbewertungssystem
- Altersverifizierung für alkoholische Getränke
- Änderungen der Versandkosten
---

## **2. Entwurf der Teststrategie**
**Testumfang: (Testumfang)**

**Im Umfang enthalten:**

- Registrierung & Anmeldung: Nein
- Altersbeschränkung für die Kontoerstellung: Ja
- Alterseingabe- und Freigabeprozess: Ja
- Produktsuche mit Sortierfunktion (z. B. nach Preis), Produktkategorisierung: Nein
- Hinzufügen von Produkten zu Favoriten: Nein
- Hinzufügen von Produkten zum Warenkorb: Ja
- Bestellabwicklung: Eingabe von Rechnungs- und Lieferadresse, Auswahl der Zahlungsmethode: Nein
- Berechnung des Gesamtbetrags: Ja
- Berechnung und Änderung der Versandkosten: Ja
- Product Rating System: Ja
- Altersverifikation für alkoholische Produkte: Ja

**Nicht im Umfang enthalten:**

- Backend-Datenbankoperationen
- UI-Funktionen
- Security Tests
- Nicht-funktionale Tests

**Geplante Testarten:**

- Funktionstests
- Regressionstests
- Usability-Tests

**Risiken, Probleme und Gegenmaßnahmen:**

**Entwicklungsverzögerungen**
- Gegenmaßnahme: Pufferzeit einplanen

**Fehlende Testdaten**
- Gegenmaßnahme: Testdaten (Mock-Daten) erstellen

**Ressourcenengpässe**

- Gegenmaßnahme: Ersatzpersonal identifizieren und einplanen

**Testlogistik (Testverantwortlichkeiten):**

- Testmanager: Thomas Breckenfelder
- QA-Ingenieur (Funktion & Regression): Thomas Breckenfelder
- QA-Ingenieur (Usability): Thomas Breckenfelder
- Endnutzer für UAT (Benutzerakzeptanztest): Student

---

## **3. Definition der Testziele**
**Ziele:**

- **Funktionalität:** Sicherstellen, dass neue und bestehende Funktionen wie vorgesehen funktionieren.


**Erwartete Ergebnisse:**

- Alle bestehenden und neuen Funktionen verhalten sich gemäß der Spezifikation.

- Fehlerhafte Benutzereingaben werden entsprechend angezeigt.

---

## **4. Definition der Testkriterien**
**Abbruchkriterien:**

- **Alle geplanten Tests** wurden ausgeführt.

- **Ausführungsrate**: 100 % aller Testfälle wurden ausgeführt.

- **Erfolgsrate**: Mindestens 90 % der ausgeführten Testfälle wurden bestanden.

- Alle kritischen und hoch priorisierten Fehler wurden behoben.

- Der Benutzerakzeptanztest (UAT) wurde abgeschlossen und freigegeben.

**Abbruchkriterien:**

- Kritische Fehler, die die Fortsetzung der Tests verhindern (Schweregrad 1).

- Ausfall der Testumgebung (Server, Datenbankzugriff).

- Fehlende Ressourcen (Tools, Hardware, Personal).

**Fortsetzungskriterien:**

- Freigabe erteilt.
- Die benötigten Tools und das Personal sind wieder verfügbar.

- Die erforderlichen Testdaten wurden erstellt, korrigiert oder aktualisiert.

---

## **5. Ressourcenplanung**

- **Personal**: QA-Team, Entwicklungsteam, Endbenutzer für UAT
- **Hardware:** PCs, Laptops, Tablets, Smartphones
- **Software:** Gängige Browser (Chrome, Firefox, Safari, Edge), Betriebssysteme (Windows, macOS, Android, iOS)

- **Infrastruktur:** Testumgebungen, Automatisierungstools
---

## **6. Testumgebung planen**
**Testgeräte**: Realgeräte mit echten Betriebssystemen und Browsern zur realitätsnahen Simulation
- **Hardware1:** MacBook Air 13“/16GB/256GB
- Betriebssystem: Sequoia 15.6.1
- Browser: Chrome für Mac


- **Hardware2:** Lenovo P52/15"/64GB/256GB
- Betriebssystem: Windows 11 Pro
- Browser: Opera für Windows


- **Hardware3:** iPad mini 7.9"/1GB/128GB
- Betriebssystem: iOS 9
- Browser: Safari

**Umgebungen:**
- Entwicklung (DEV)
- TEST (Test)
- Abnahme (ACC - Acceptance)

---

## **7. Zeitplan und Aufwandsschätzung**


| Aktivität                                        | Startdatum | Enddatum  | Umgebung | Verantwortlich | Geplanter Aufwand |
|--------------------------------------------------|------------|-----------| -------- |----------------|-------------------|
| Testplanung                                      | 06.11.2025 | 11.11.2025 | Alle     | TB             | 7 Stunden         |
| Testfalldesign                                   | 12.11.2025 | 12.11.2025 | Alle     | TB             | 7 Stunden         |
| Unittest (nur Erweiterungen)                     | 13.11.2025 | 13.11.2025 | TEST     | TB             | 7 Stunden         |
| Integrationstest (Zusammenspiel der neuen Module) | 14.11.2025 | 14.11.2025| TEST     | TB             | 5 Stunden         |
| Systemtest                                       | 17.11.2025 | 17.11.2025 | TEST     | TB             | 7 Stunden         |
| Teil-Regressions-Test (von Änderungen betroffen) | 18.11.2025 | 18.11.2025 | ACC      | TB             | 3 Stunden         |
| Abnahmetest (UAT)                                | 18.11.2025 | 18.11.2025 | TEST     | PB             | 2 Stunden         |
| Dokumentation                                    | 19.11.2025 | 19.11.2025 | ACC      | TB             | 2 Stunden         |

------------------------------------

## **8. Testergebnisse festlegen**

Dokumente/Tools, die zur Unterstützung der Testaktivitäten im Projekt erstellt werden müssen:

- Testplan / test plan (GitHub)
- Testfälle und Testskripte / test case design (GitHub)
- Testdaten / functional test execution (GitHub)
- Testberichte / test reporting (GitHub)
- Fehlerberichte (GitHub)
- Abnahmedokument für Benutzertests (GitHub)