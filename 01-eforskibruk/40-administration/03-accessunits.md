# Tilgangsenheter

Tilgangsenhetene er en hierarkisk liste over enheter man kan logges inn p� i databasen. En tilgangsenhet har tilgang til data registrert p� seg selv, p� barn, og videre arvinger nedover i hierarkiet. En tilgangsenhet kan ikke se data registrert p� sin foreldre (og forfedre) oppover i hiearkiet. Tilgang h�yere opp i tilgangstreet vil si tilgang til � mer data, tilgang laverene ned vil begrense tilgangen til data.

En tilgangsenhet har ikke tilgang til � se data i kladd tilgangsenheter nedover i hiearkiet. Data m� ferdigstilles eller v�re til kontroll for at dem skal v�re synlig p� andre enn tilgangsenheten dem er opprettet p�.

En database av enkleste form vil kun ha en stykk tilgangsenhet, man trenger da ikke � ha noen kunnskap om tilganger og hierarki.