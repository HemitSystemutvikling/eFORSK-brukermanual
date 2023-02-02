# Forskningsobjekter

Skjemaer i eFORSK tilhører det vi kaller forskningsobjekter. Forskningsobjekter tilhører en forskningsobjekttype.

Personer fra Personregisteret ligger inne som standardtype for forskningsobjekt, 
men en bruker med rollen *databaseansvarlig* kan også opprette andre typer av forskningsobjekt når data man samler inn ikke kommer fra mennesker. 
Andre typer kan for eksempel være legemidler, lab-rotter eller lignende. 
Bruker man ikke standardtypen personer fra Personregisteret kan man ikke bestille skjema til utfyllelse via ePROM.

Ved opprettelse av en skjematype låses den til en spesifikk forskningsobjekttype og kan ikke endres senere.

Under "Forskningsobjekter" kan man se de siste forskningsobjektene som er behandlet skjema på i databasen, samt søke opp eller opprette nye forskningsobjekter. 

## Samtykke

Hvordan samtykkehåndering fungerer kan leses under "Administrasjon/Skjematype/Samtykkehåndtering".

Alle forskningsobjektets samtykker vises på forskningsobjektets side. Merk at skjemaer i kladd ikke telles som samtykker.

## Sletting

Databaseansvarlige har tilgang til å slette forskningsobjekter. Dette gjøres eksempelvis hvis et forskningsobjekt trekker sitt samtykke.

Sletter man et forskningsobjekt vil alle spor av forskningsobjektet bli borte. Umiddelbart etter sletting blir forskningsobjektet markert som Slettet, og alle koblinger til fødselsnummer fjernes. Skjemadataene (svarene) og tilknyttede dokumenter vil slettes automatisk påfølgende natt etter man har slettet forskningsobjektet (årsaken er at et program med forhøyede rettigheter må kjøres for å slette historisk loggførte data).

__NB:__ Denne handlingen kan ikke reverseres! Etter sletting vil det aldri være mulig å gjenopprette koblingen mellom forskningsobjektets unike nøkkel og forskningsobjektets fødselsnummer. Dersom det er nødvendig å ivareta dette, anbefales å eksportere en kryptert koblingsnøkkelfil i forkant av slettingen. __Det er viktig å ta stilling til dette, spesielt i tilfeller hvor forskningsobjektet inngår i en randomisering.__ 
