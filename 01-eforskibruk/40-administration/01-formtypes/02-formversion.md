# Versjoner

Man kan lage nye versjoner av en skjematype og innføre endringer som ikke vil forstyrre tidligere versjoner som allerede er tatt i bruk.

Ved opprettelse av en ny versjon starter man med en kopi av den forrige versjonen til skjematypen. Man kan kun opprette ny versjon av den siste eksisterende versjonen.

Flere versjoner kan være publisert samtidig, men kun en versjon kan være i kladd om gangen. Grunnen til dette er at versjonene er kronologiske, en ny versjon opprettes som en kopi av den forrige versjonen. Kunne man endret versjoner tilbake i rekken, ville dette påvirket alle etterkommende versjoner.

Versjonene får navn V*X*, der *X* er versjonsnummeret. Det anbefales å i tillegg gi versjonen et navn for å enklere skille den fra andre versjoner. Dette gjøres i skjemabyggeren på høyre side.

## Versjonsstatus

En versjon har en av følgende statuser:

### Kladd

Det er kun i status kladd at innholdet i en versjon kan endres. Når en versjon har forlatt status kladd kan den **aldri** returnere tilbake til denne statusen, versjonen blir altså låst for endringer.

### Publisert

Når en skjematype er publisert, kan man fylle ut skjemaer av denne typen. Om ePROM er aktivert for skjematypen, kan man også bestille skjemautfyllelse fra personer i Personregisteret. I testmodus kan man gjøre dette umiddelbart, mens for ikke-test modus må versjonen godkjennes av en administrator først.

Versjoner som er publisert, avpublisert eller låst kan ikke endres; man er nødt til å opprette en ny versjon for å overholde korrekt versjonering av felter og regler.

En publisert versjon kan avpubliseres eller låses.

#### Felter i publiserte versjoner

Det er ikke mulig å endre på feltinformasjon til et felt som finnes i en tidligere publisert versjon av et skjema. Det inkluderer:
- Visningstekst
- Variabelnavn
- Hjelpetekst
- Alternativer for visning
- Om feltet inneholder personopplysninger

Følgende egenskaper kan likevel endres på et felt som finnes i en tidligere publisert versjon av et skjema:
- regler på feltet kan legges til og fjernes
- feltets plassering kan endres i skjemaet
- feltet kan slettes

### Avpublisert

Når en verjson er avpublisert kan det ikke opprettes nye skjemaer eller bestilles utfyllelse av versjonen. Allerede opprettede skjemaer kan man fortsatt endre på, og eventuelle svar på skjemabestillinger vil fortsette å komme inn. Bruker man personinitiert ePROM, vil lenken til skjemaet ikke fungere lenger. 

Avpubliserte versjoner kan publiseres på nytt eller låses.

### Låst

Når en versjon er låst, kan man verken opprette nye skjemaer, bestille utfyllelse eller endre på eksisterende skjemaer. Tilstanden er låst. Eventuelle svar på skjemabestillinger vil fortsatt komme inn, ønsker man ikke dette må man sørge for at alle ubesvarte bestillinger har løpt ut på tid. Merk at bestillinger som har blitt sendt som papirskjema i posten ikke har en utløpstid. Bruker man personinitiert ePROM, vil lenken til skjemaet ikke fungere lenger. 

Låste versjoner kan publiseres på nytt eller avpubliseres.
