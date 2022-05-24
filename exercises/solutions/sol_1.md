# Aufgabe 1.1
Loggen sie sich in den Administrator-Account ein, ohne sql-injection zu nutzen oder das Passwort vorher zu ändern.
## Mögliche Lösung
Die Email-Adresse des Admin kann man raten oder in den Reviews zu den einzelnen Produkten wiederfinden. Das Passwort kann man ebenfalls raten oder in der rockyoumini.txt wiederfinden und z.B. mit der Burp-Suite rausfinden.

# Aufgabe 1.2
Loggen sie sich in Jims Account über die "forgot your password" Funktion ein.
## Mögliche Lösung
Über die Reviews herausfinden, wer Jim ist und dann bei Wikipedia nachschauen. Mit dem Hinweis "Star Trek" sollte das machbar sein. 

# Aufgabe 1.3
Burp-Suite und die rockyoumini.txt nutzen, um sich in den Administrator-Account einzuloggen.
## Mögliche Lösung
- Proxy-tab -> intercept-tab -> Browser öffnen.
- zum Login navigieren
- Login-Versuch starten mit richtiger Admin-Email und irgendein Passwort
- In der HTTP history den "POST" Eintrag finden zum Loginversuch, Rechtsclick auf den Eintrag und "send to intruder"
- Intruder-tab öffnen und einmal den Button "clear" klicken. Dann ins Passwort-feld doppelklicken und dann den Button "add" clicken. Es erscheint innerhalb des password-Strings zwei "§" zeichen und es wird markiert.
- Dann zu "payloads" gehen und die rockyoumini.txt reinladen
- Angriff starten und gucken, welches genutzte Passwort ein Status 200 zurückgibt
- "results" öffnen für bessere Übersicht