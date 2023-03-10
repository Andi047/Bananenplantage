# Einbau von RegEx in Anmeldeformular

Schritt 1:

Vorname (einzelner, lateinischer Name): ^[A-Z]{1}[a-z]{2,8}$
Nachname (schwierig bei von / zu etc., daher so): ^[\D]+?[\D]+$


Schritt 2:

Kontakt:

E-Mail: ^[\w]+\S?[\w]+@[\w]+.([a-z]{2,4})+$
Festnetz-Nummer (ohne Ländervorwahl mit +): ^(([0-9]+\s|[0-9]+)[0-9]+){4,15}$


Schritt 3:

Login-Daten:

Benutzername (muss klein anfangen): ^[a-z]+[\w]+$
Passwort (mind. 6 Zeichen, Groß/Klein + Zahl + Sonderzeichen): ^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[-#§$%&])([^\s]){6,}$
