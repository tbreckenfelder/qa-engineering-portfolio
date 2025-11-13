## **Die Software**

--- 
Webshop: https://grocerymate.masterschool.com/

Mit folgenden Basisfunktionen:

- Registrierung und Anmeldung
- Produktsuche mit Sortierfunktion (z. B. nach Preis), Produktkategorisierung
- Produkte zu Favoriten hinzufügen
- Produkte in den Warenkorb legen
- Bestellabwicklung: Rechnungs- und Lieferadresse eingeben, Zahlungsart auswählen, Gesamtbetrag berechnen

## **Neue Funktionen**

---

## **1. Product Rating System**

Nutzer sollen Produkte anhand eines 5-Sterne-Systems bewerten.

**Vage formulierte** Anforderung:
* **Frage 1:** Nach welchem Status (wann) darf der Nutzer eine Bewertung abgeben?
* **Frage 2:** Zu welchem Zeitpunkt soll die Bewertung angezeigt werden?
* **Frage 3:** Darf der Nutzer eine abgegebene Bewertung löschen oder ändern?


Nutzer sollen zusätzlich ein schriftliches Feedback hinterlassen können.

**Vage formulierte** Anforderung:
* **Frage 4:** Soll das Feedbackfeld ein Pflichtfeld sein?
* **Frage 5:** Soll das Feedback vor der Veröffentlichung durch einen Filter geprüft werden?
* **Frage 6:** Soll die Anzahl der Zeichen begrenzt werden?

Besser:

**Konkret formulierte** Anforderung:
* **Frage 1:** Erst wenn der Kauf des Produkts abgeschlossen ist können Bewertungen abgegeben werden.
* **Frage 2:** Die abgegebene Bewertung soll angezeigt werden, wenn der Artikel im Shop erneut angezeigt wird.
* **Frage 3:** Der Nutzer darf eine abgegebene Bewertung nicht löschen oder ändern.

* **Frage 4:** Das Feedbackfeld soll ein Pflichtfeld sein.
* **Frage 5:** Das Feedback soll vor der Veröffentlichung durch einen Filter (z.B. Schimpfwort- oder Profanity) geprüft werden.
* **Frage 6:** Die Anzahl der Zeichen soll auf 50 Zeichen begrenzt sein.

---

## **2. Altersverifikation für alkoholische Produkte**

Alkoholische Produkte erfordern eine Altersverifikation. 

**Vage formulierte** Anforderung:
* **Frage 1:** Wird nach Eingabe des Geburtsjahres das Alter automatisch berechnet?
* **Frage 2:** Muss ein einmal registrierter Nutzer immer wieder das Modal ausfüllen?
* **Frage 3:** Wie reduziere ich versehentliche Falscheingaben?

Beim Aufrufen der Kategorie soll ein Modal erscheinen, in dem Nutzer ihr Alter angeben müssen (18+), bevor sie Zugriff erhalten.

**Vage formulierte** Anforderung:
* **Frage 4:** Was passiert, wenn der Geburtstagsinput nicht erfolgt?
* **Frage 5:** In welchem Format soll das Geburtsdatum angegeben werden? 
* **Frage 6:** Was passiert bei der Bestätigung des Nutzers < 18J? 

Besser:

**Konkret formulierte** Anforderung:
* **Frage 1:** Nach Eingabe des Geburtstages erfolgt die Altersberechnung. Nur wenn das errechnete Alter ≥ 18 Jahre ist, darf der Zugriff auf alkoholische Produkte erlaubt werden. Sonst Nachricht JuSchG und Funktion Sperrung Plausibilitätsprüfung).
* **Frage 2:** Das System speichert die Bestätigung („18+“) lokal im Browser (z. B. Cookie) für eine definierte Dauer (z. B. 24 Std.), sodass das Modal nicht bei jedem Aufruf erneut erscheint. Danach erscheint das Modal erneut.
* **Frage 3:** Nach Eingabe des Geburtstages erfolgt ein weiterer Schritt. "Ich bestätige, dass das eingegebene Geburtsjahr korrekt ist und ich über 18 Jahre alt bin".

* **Frage 4:** Das Modal soll den Seiteninhalt so lange blockieren, bis ein Geburtstag eingegeben wurde.
* **Frage 5:** Das Geburtsdatum soll im Format {TT-MM-JJJJ} angegeben werden.
* **Frage 6:** Bei der Bestätigung („< 18“) wird der Nutzer auf eine Seite ohne alkoholische Inhalte weitergeleitet (z. B. Startseite) oder zurück zu seinem Warenkorb (ohne Alc.).

---

## **3. Änderungen der Versandkosten**

Für Bestellungen über einem bestimmten Wert entfallen die Versandkosten. Für Bestellungen unter diesem Wert fallen Versandkosten an.

**Vage formulierte** Anforderung:
* **Frage 1:** Ab welchem Bestellwert entfallen die Versandkosten? 
* **Frage 2:** Werden die Versandkosten pro Bestellung oder pro Artikel berechnet, bevor geprüft wird, ob der Schwellenwert erreicht wurde?
* **Frage 3:** Was passiert, wenn ein Nutzer Produkte entfernt oder hinzufügt – werden die Versandkosten sofort neu berechnet und angezeigt?

**Konkret formulierte** Anforderung:
* **Frage 1:** Die Versandkosten entfallen ab einem Bestellwert von >= 20€.
* **Frage 2:** Die Versandkosten pro Bestellung oder pro Artikel werden berechnet, bevor geprüft wird, ob der Schwellenwert erreicht ist.
* **Frage 3:** Fügt ein Nutzer Produkte hinzu oder löscht – werden die Versandkosten sofort neu berechnet und angezeigt,