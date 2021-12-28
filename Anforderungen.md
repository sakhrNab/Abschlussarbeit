# funktionale Anforderungen
## 1. Anforderung
---
- Funktion: 
    1. Einloggen

- Eingaben: 
    1. Email-adresse
    2. Passwort

- Verarbeitungsschritt:
    1. prüfe, ob der Emailadresse richtig ist
    2. prüfe, ob das Passwort richtig ist.

- Ausgaben: Die Hauptseite wird angezeigt oder ein Fehler wird gemeldet. 

## 2. Anforderung
--- 
- Funktion: 
    1. Registerieren
- Eingaben:
    1. Vorname
    2. Nachname
    3. Geschlecht
    4. Email-Adresse
    5. Ort
    6. PLZ
    7. Spieler-stärke
    8. Passwort
    9. Passwort-Wiederholung
    10. 
- Verarbeitungsschritte:
    1. prüfe, ob die Emailadresse vergeben ist.
    2. prüfe, ob das PW die Anforderungen erfüllt.
    3. prüfe, ob den Namen kein falsches Zeichen enthält. 
- Ausgaben:
    1. Ein Status zur Überprüfung der Richtigkeit der Emailadresse.
    2. Eine Email mit einem Link zur Hauptseite für angemeldeten wird zugeschickt. 

## 3. Anforderung
---
- Funktion: Ausloggen
- Eingaben: Keine - Vorgegebenes Token während der Sitzung für angemeldeten.
- Verarbeitungsschritte: 
    1. Wenn Benutzer eingeloggt sind, dann können sie ausloggen und das Token wird entsprechend gelöscht.
- Ausgaben:
    1. Hauptseite für nicht angemeldeten

## 4. Anforderung
---
- Funktion: Suche
- Eingaben: 
    1. Benutzername
    2. Filter nach:
        - Region
        - Geschlecht
        - Alter
        - Stärke
- Verarbeitungsschritte: 
    1. prüfe, ob der Name richtig ist

- Ausgabe:
    - gesuchte Benutzer(n).
    - NOT-FOUND Meldestatus

## 5. Anforderung
---
- Funktion: Sendung der Anfrage
- Eingaben: 
    1. Titel
    2. Text - Email

- Verarbeitungsschritte:
    1. 
- Ausgabe:
    1. Meldestatus "Email erfolgreich zugesendet worden"
    2. Meldestatus "Versand fehlgeschlagen"
    3. 

## 6. Anforderung
--- 
- Funktion: Profilbearbeitung
- Eingaben: 
    1. Profilbild hinzufügen
    2. Profilseinstellung
        - Email ändern
        - passwort zurücksetzen
        - Profilbearbeiten
            1. Stärke ändern
            2. Verfügbarkeit
            3. Name 
            4. Ort
- Verarbeitungsschritte:
    1. 
- Ausgabe: -- PUT ANFRAGEN --
    1. HTTPSTATUS 
        - 200 - (OK)
        - 204- (No Content) "resource updated successfully"
    2. HTTPSTATUS - Fehlermeldungen
## 7. Anforderung
---
- Funktion: Profil löschen
- Eingaben: 
    1. Button klicken, um Profil zu löschen
- Verabrieungsschritte:
    1. prüfe, ob den Benutzer den Button nicht aus Versehen geklickt hat- Meldung "Klicken Sie auf Bestätigen, um das Profil zu löschen"
        - HTTPSTATUS: 202 (Accepted)

- Ausgabe:
    1. Hauptseite für nicht angemeldeten, oder
    2. Abschiedsmeldestatus
## 8. Anforderung
--- 
- Funktion: Authenticate
- Eingaben: to be found - or external library
- Verarbeitungsschritte
- Ausgabe: 

## 9. Anforderung
---
- Funktion: clickOnUser
- Eingaben:
    1. FindUserThrough SearchField
    2. FindUser on MainPage
    3. FindUser through Filtering page
- Verarbeitugsschritte
    1. prüfe, ob UserExistiert

- Ausgabe:
    1. Benutzersprofil
    2. Meldestatus: Bentuzer existiert nicht mehr. Nur wenn danach expliziert gesucht wird. 
## 10. Anforderung
---
- Funktion: Benutzer bewerten
- Eingaben: 
    Bedingung: 
    Man darf nur bewerten, wenn man bereits mit dem Benutzer gespielt hat. 
    1. Sternen Zahl eingeben. Min: 0 Sternen und Max: 5
    2. Benutzer bewerten im Text Form. Max. Zeichen ist 200. 
- Verabeitungsschritte:
    1. prüfe, ob den Benutzer bereits mit dem zu bewertenden gespielt hat.
    
- Ausgabe:
    1. Benutzersprofil mit der aktuelisierten Bewertung.

## 11. Anforderung:
- Funktion: Eigene Verfügbarkeit adden/bearbeiten/auschalten.
- Eingaben: 
    1. Daten der Verfügbarkeit eingeben-
    2. Uhrzeiten der Verfügbarkeit eingeben. 
    3. 
- Verabeitungsschritte:
    1. prüfe, ob die Eingabe nicht mit anderen Terminen überschneidet. 
- Ausgabe:
    1. Kalender mit Verfügbarkeitsübersicht.
    2. Meldestatus: Success

## 12. Anforderung
---
- Funktion: Benutzer in/von der Favoritenliste adden/löschen.
- Eingaben: 
    1. Button zum Hinzufügen
- Verarbeitungsschritte:
    1. prüfe, ob Benutzer existiert. 
- Ausgabe: Favoritenliste der angemeldeten Benutzer

## 13. Anfoderung
---
- Funktion: Stornierung einer Anfrage bzw. eines Termins.
- Eingabe: 
    1. Button zur Stornierung
    2. Texteingabe, wenn man noch eine Nachricht beifügen will. 
- Verarbeitugsschritte:
    1. prüfe, ob eine Anfrage bereits existiert.

- Ausgabe: 
    1. Meldestatus: "Ihre Spieltermin mit Benutzername wurde storniert"
    2. der andere Benutzer erhält eine Email und die Buchung von seinem/ihrem Kalender wird gelöscht.

## 14. Anforderung
---
- Funktion: 

There are two main requirements, which are going to be acquired and explained on the following section. There are the functional and non-functional requirements. 
Es gibt zwei Hauptanforderungen, die im folgenden Abschnitt behandelt und erläutert werden sollen. Es sind die funktionalen und die nicht-funktionalen Anforderungen.