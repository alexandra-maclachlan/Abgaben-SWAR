# Übung 1 - Software-Systemanforderungen 

Beantworten Sie folgende Fragen:

1. Wie beschreibt man eine technische Schnittstelle vollständig?

   API steht für „Application Programming Interface“. Grundsätzlich handelt es sich dabei um eine Schnittstelle, die die Kommunikation und Interaktion zwischen zwei Systemen ermöglicht. Das heisst mit dieser Schnittstelle wird anderen Programmen ein Tool zur Verfügung gestellt, über welches sie sich an das Software System anbinden können. 

   - Performanz
   - Datensicherheit/ Datenschutz
   - System-System-Schnittstelle

2. **Wie beschreibt man eine Benutzerschnittstelle?**

   - Statisches Verhalten
   - Dynamisches Verhalten

   Eine Benutzerschnittstelle bietet Benutzern die Möglichkeit, mit einem Programm oder Rechner einen Datenaustausch durchzuführen. Eine Benutzerschnittstelle kann zum Beispiel ein Web-Formular oder eine Eingabemaske sein. Das am meisten benutzte Interaktions-Level ist derzeit das GUI.

3. **Welche weiteren Aspekte sollte eine vollständige Systemanforderung beschreiben?**

   - Software Requirements Specification
   - Pflichtenheft
   - Beschreibung des Systems aus Blackbox Sicht

4. **Was sollte eine Systemanforderung beschreiben?**

   Die **Systemanforderungen** sind Anforderungen an das System.

   - UI, Nutzer-System-Schnittstelle
   - Schnittstelle  zur Laufzeitumgebung
   - Datenschnittstelle Technische Schnittstellen

5. Wie nennt man Systemanforderungen noch? Wie unterscheiden sie sich von Stakeholder-Anforderungen?

   Sie werden auch SRS (System Requirements Specification) genannt obwohl hiermit eigentlich Systemanforderungen zusammen mit der Systemspezifikation gemeint ist. 

   Systemanforderungen sind viel spezifischer.
   Stakeholder-Anforderungen gruppiert man nach Kernaufgaben, Teilaufgaben, Nutzungsanforderungen.

# Übung 2 - Software-Systemanforderungen 

Fall Beispiel für das Erheben von Anforderungen. 

Situation:

Die Nicht Moderne Firma in Konstanz pflegt ihre Abonnenten / Kunden und Interessenten nach wie vor in einem Hängeregister. Sie als Requirements Engineer werden engagiert, um dieses veraltete System zu digitalisieren.

Das System soll sowohl Intern für die Mitarbeiter dieser Firma als auch für die Kunden zugänglich sein. Es soll die Möglichkeit bieten sich als neuer Abonnent eines bezahlten Newsletters ähnlich einer Tageszeitung zu registrieren. Die Kunden sollen Ihre News online abrufen können. 

Die Mitarbeiter der Firma sollen Ihre Kunden verwalten können und diesen Nachrichten zu schicken können.

Aufgaben:

1. **Identifizieren Sie die Nutzer Gruppen.**

   - Kunden/Abonnent, Mitarbeiter

2. **Identifizieren Sie die Erfordernisse**

   - Die Mitarbeiter müssen einen Computer verfügbar haben, um das System pflegen zu können.

   - Die Nutzer müssen eine Internet verfügbar haben um online-News abrufen zu können.

   - Der Kunde muss wissen, welche Daten er eingeben muss, um sich für den Newsletter registrieren zu können.

   - Der Mitarbeiter muss die Daten des Kunden kennen, um diese verwalten zu können.

     

3. **Erheben Sie die Kernaufgaben.** 

   | Vorbedingung                             | Kernaufgabe                                              | Nachbedingung                                    |
   | ---------------------------------------- | -------------------------------------------------------- | ------------------------------------------------ |
   | Gültige Anmeldedaten                     | Administrator anlegen                                    | Administrator angelegt                           |
   | Administrator angelegt                   | Administratoren verwalten/ verändern                     | Änderungen an den Daten wurden vorgenommen       |
   | Administrator wurde zuvor registriert    | Administratoren können sich anmelden                     | Administrator angemeldet                         |
   | Administrator angemeldet                 | Mitarbeiter/ Administratoren können Newsletter schreiben | Newsletter angelegt                              |
   | Newsletter wurde angelegt                | Newsletter kann bearbeitet/ verändert werden             | Newsletter Änderungen wurden vorgenommen         |
   | Newsletter wurde angelegt/ erstellt      | Mitarbeiten können Newsletter versenden                  | Newsletter wurde versendet                       |
   | Gültige Anmeldedaten                     | Kunde kann sich registrieren                             | Kunde wurde angelegt                             |
   | Kunde ist registriert                    | Kunde kann sich anmelden                                 | Kunde ist angemeldet                             |
   | Kunde muss registriert sein              | Kundendaten verwalten/verändern                          | Änderungen an den Kundendaten wurden vorgenommen |
   | Kunde muss registriert sein              | Zahlungsdaten anlegen                                    | Zahlungsdaten hinterlegt                         |
   | Newsletter angelegt und Kunde angemeldet | Newsletter abonnieren                                    | Newsletter wurde abonniert                       |
   | Newsletter per Email empfangen           | Newsletter einsehen (Email)                              | Newsletter- Vorschau wird angezeigt              |
   | Newsletter aufrufen                      | Newsletter einsehen (online)                             | Newsletter wird angezeigt                        |
   | Als Nutzer angemeldet sein               | Nachricht  verfassen                                     | Nachricht wurde erstellt                         |
   | Nachricht wurde erstellt                 | Nachricht versenden                                      | Nachricht versendet                              |

   

4. **Leiten Sie die Teilaufgaben ab.**

   - Kernaufgabe:  Administrator anlegen
     - Anmeldedaten festlegen
     - Passwort festlegen
     - Email eingeben
     - Rolle festlegen 
   - Kernaufgabe: Administratoren verwalten/ verändern
     - Daten ändern
     - Zugriffsrechte ändern
     - Passwort ändern 
     - Änderungen speichern
   - Kernaufgabe: Administratoren können sich anmelden
     - Anmeldedaten eingeben

   - Kernaufgabe: Mitarbeiter/ Administratoren können Newsletter schreiben
     - Administrator anmelden
     - Newsletter verfassen
     - Newsletter speichern
   - Kernaufgabe: Newsletter kann bearbeitet/ verändert werden
     - Administrator anmelden
     - Newsletter suchen
     - Newsletter verändern
     - Newsletter speichern
   - Kernaufgabe: Mitarbeiter können Newsletter versenden
     - Administrator anmelden
     - Kunde suchen 
     - Kunde auswählen
     - Newsletter versenden

   - Kernaufgabe: Kunde kann sich registrieren
     - Anmeldedaten festlegen
     - Passwort festlegen
     - Email eingeben
   - Kernaufgabe:   Kunde kann sich anmelden
     - Anmeldedaten eingeben
   - Kernaufgabe:   Kundendaten verwalten/verändern
     - Daten ändern
     - Zugriffsrechte ändern
     - Passwort ändern 
     - Änderungen speichern
   - Kernaufgabe: Zahlungsdaten anlegen
     - Kunde anmelden
     - Zahlungsdaten hinterlegen
     - Änderung speichern
   - Kernaufgabe: Newsletter abonnieren
     - Kunde anmelden
     - Newsletter abonnieren
   - Kernaufgabe: Newsletter einsehen (Email)
     - Kundenemail hinterlegt
     - Newsletter abonniert
     - Newsletter empfangen
     - Email Konto einsehen
   - Kernaufgabe:   Newsletter einsehen (online)
     - Newsletter einsehen (Email)
     - Kunde anmelden
     - Link abrufen

5. **Notieren Sie die Nutzungsanforderungen.**

   - Der Nutzer muss am System seinen Vor- und Nachnamen eingeben können.
   - Der Nutzer muss am System seine E-Mail-Adresse eingeben können.
   - Der Nutzer muss am System sein Passwort eingeben können.
   - Der Nutzer muss am System den Button zum Registrieren auswählen können. 

   - Der Nutzer muss am System seine Rolle auswählen können.
   - Der Nutzer muss am System seine Benutzerdaten zum Anmelden eingeben können.
   - Der Nutzer muss am System den Button zum Anmelden auswählen können.
   - Der Nutzer muss am System die aktuellen Daten erkennen können.
   - Der Nutzer muss am System die neuen Daten eingeben können.
   - Der Nutzer muss am System den Button zum speichern auswählen können.
   - Der Nutzer muss am System die Kunden eindeutig unterscheiden können.
   - Der Nutzer muss am System einen Kunden auswählen können.
   - Der Nutzer muss am System erkennen können wie er sich ausloggen kann.
   - Der Nutzer muss am System den Butten zum Ausloggen auswählen können.
   - Der Nutzer muss am System eine Nachricht eingeben können. 
   - Der Nutzer muss am System den Button zum Versenden der Nachricht auswählen können. 
   - Der Nutzer muss am System einen Button zum Abonnieren des Newsletters erkennen können.
   - Der Nutzer muss am System einen Button zum Abonnieren des Newsletters auswählen können.
   - Der Nutzer muss am System einen neuen Newsletter eingeben können.
   - Der Nutzer muss am System den Button zum Bearbeiten des Newsletters auswählen können. 
   - Der Nutzer muss am System den Button zum Speichern der Änderung auswählen können.
   - Der Nutzer muss am System den Button zum Versenden des Newsletters an den Kunden auswählen können.
   - Der Nutzer muss am System den aktuellen Newsletter online erkennen können.
   - Der Nutzer muss am System den Button zum löschen von Kundendaten auswählen können.
   - Der Nutzer muss am System den Button zum Abmelden des Newsletters auswählen können.

   
