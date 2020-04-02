#### Übung 1

1. *Wie beschreibt man eine technische Schnittstelle vollständig?*

   API steht für „Application Programming Interface“. Grundsätzlich handelt es sich dabei um eine Schnittstelle, die die Kommunikation und Interaktion zwischen zwei Systemen ermöglicht. Das heisst mit dieser Schnittstelle wird anderen Programmen ein Tool zur Verfügung gestellt, über welches sie sich an das Software System anbinden können. 

   - Performanz
   - Datensicherheit/ Datenschutz
   - System-System-Schnittstelle

2. *Wie beschreibt man eine Benutzerschnittstelle?*

   - Statisches Verhalten
   - Dynamisches Verhalten

   Eine Benutzerschnittstelle bietet Benutzern die Möglichkeit, mit einem Programm oder Rechner einen Datenaustausch durchzuführen. Eine Benutzerschnittstelle kann zum Beispiel ein Web-Formular oder eine Eingabemaske sein. Das am meisten benutzte Interaktions-Level ist derzeit das GUI.

3. *Welche weiteren Aspekte sollte eine vollständige Systemanforderung beschreiben?*

   - Software Requirements Specification
   - Pflichtenheft
   - Beschreibung des Systems aus Blackbox Sicht

4. *Was sollte eine Systemanforderung beschreiben?*

   Die **Systemanforderungen** sind Anforderungen an das System.

   - UI, Nutzer-System-Schnittstelle
   - Schnittstelle  zur Laufzeitumgebung
   - Datenschnittstelle Technische Schnittstellen

5. *Wie nennt man Systemanforderungen noch? Wie unterscheiden sie sich von Stakeholder-Anforderungen?*

   Stakeholder-Anforderungen beinhalten Systemanforderungen. Unter Systemanforderungen versteht man die Anforderung an die effiziente Erbringung eines Ergebnisses mit einem interaktiven System (z.B. Software). Man kann sie nach Kernaufgaben, Teilaufgaben und Nutzungsanforderungen gruppieren. Sie werden auch SRS (System Requirements Specification) genannt obwohl hiermit eigentlich Systemanforderungen zusammen mit der Systemspezifikation gemeint ist. 

#### Übung 2

1. *Identifizieren Sie die Nutzer Gruppen.*
   Mitarbeiter und Kunde
2. *Identifizieren Sie die Erfordernisse*

- Die Firma muss die Kundendaten verfügbar haben, um das System erneuern zu können.
- Der Kunde muss wissen, welche Daten er eingeben muss, um sich für den Newsletter zu registrieren.
- Der interne Mitarbeiter muss die Daten der Kunden kennen, um diese verwalten zu können. 
- Die Mitarbeiter müssen die Kundendaten verwalten können, um ihren Kunden Nachrichten schicken zu können. 

3. *Erheben Sie die Kernaufgaben.*
   Vorbedingung: Wissen welche Kundendaten ein Hängeregister beinhaltet
   Kernaufgabe: Hängeregister digitalisieren
   Nachbedingung: das Hängeregister wurde digitalisiert

   Vorbedingung: Die Mitarbeiter müssen die Kundendaten kennen
   Kernaufgabe: Mitarbeiter können Kundendaten verwalten/ verändern
   Nachbedingung: Änderungen an den Kundendaten wurden vorgenommen

4. *Leiten Sie die Teilaufgaben ab.*

   Kernaufgabe: Hängeregister digitalisieren

   - physische Kundendaten in Datenbank eintragen

   - eindeutige Benennung des Kundendossiers

   Kernaufgabe: Mitarbeiter können Kundendaten verwalten/ verändern

   - eindeutige Identifikatoren für einen jew. Kunden
   - Möglichkeit Daten verändern zu können

5. *Notieren Sie die Nutzungsanforderungen.*

   NA1: Der Nutzer muss am System die Daten eines neuen Kunden eingeben können.

   NA2: Der Nutzer muss am System die Kundendaten ändern können.

   NA3: Der Nutzer muss am System die Kunden eindeutig unterscheiden können.

   NA4: Der Nutzer muss am System einen Kunden auswählen können.

   NA5: Der Nutzer muss am System neue Attribute zu einem Kunden hinzufügen können. 

   NA6: Der Nutzer muss am System eine Nachricht für den Kunden eingeben können. 

   