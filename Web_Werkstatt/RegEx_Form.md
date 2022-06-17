# Einbau von RegEx in Anmeldeformular

Schritt 1:

Vorname: ^[\D]+$
Nachname: ^[\D]+?[\D]+$


Schritt 2:

Kontakt:

E-Mail: ^[\w]+?[\w]@[\w]+\W[\w].[\w]+$
Festnetz-Nummer: ^(+[0-9]+|[0-9]+)[0-9]+$


Schritt 3:

Login-Daten:

Benutzername: ^[\w]+$
Passwort: ^[\w]+$
