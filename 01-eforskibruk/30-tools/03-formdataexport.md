# Eksporter data

Når man eksporterer data blir hvert felt i skjematypen en egen kolonne med variabelnavnet som overskrift. Rekkefølgen på feltene kan bestemmes av databaseansvarlig ved redigering av skjematypen. Eksport gjøres via **Verktøy** - **Eksporter data**. Alternativt finnes dataeksport-valget også under valget **Bruk disse** som du finner under fanene **ePROM bestillinger** eller **Skjema** i hovedmenyen.  

## Redigere rekkefølge i dataeksport

* Åpne den aktuelle skjematypen
* Velg fanen Felter. Her vises alle felter skjematypen inneholder, inkludert metadatafelt
* Trykk på **Rediger rekkefølge** øverst til høyre, dette gir to alternativer:
    * Flytt felt manuelt opp eller ned med pilene til høyre for hvert felt
    * Sorter felter etter skjemaversjon, som velges øverst. Da vil feltene i eksporten sorteres i samme rekkefølge som de vises i den aktuelle skjemaversjonen
* Velg **Lagre rekkefølge**

## Filformat

Ved eksport av data får man en kryptert zip-fil. For å pakke ut denne filen trenger man:
* Et program som kan pakke ut zip-filer som er kryptert med AES 256-standarden, for eksempel 7-Zip
* Passordet som genereres. Dette blir kun presentert én gang og kan ikke gjenhentes i etterkant. For å sikre korrekt og trygg håndtering anbefales det at passordet lagres på en sikker måte. Passordet bør aldri lagres i klartekst, deles ukryptert eller oppbevares på steder som kan være tilgjengelig for uvedkommende. Dersom passordet går tapt, må eksporten gjennomføres på nytt for å generere et nytt passord.

Innholdet i zip-fila velges ved eksport, csv og xlsx støttes.

## Samtykkeeksport

For eksport av samtykker til dokumentasjonsformål, gå til **Verktøy** - **Eksporter data** og velg aktuelle skjematype du ønsker å eksportere samtykker for. Beskriv formålet med eksporten, ønsket format, ta stilling til om du trenger personidentifiserbare data og metadata og huk av valget **Eksporter som samtykkedata** for å inkludere en PDF-fil med alle samtykker for aktuelle skjematype. 

## Ansvar

Eksportfilene og innholdet i disse må behandles i henhold til personopplysningsloven og tilhørende forskrifter. 
Opplysningene kan bare behandles i tråd med det formålet de er innsamlet for, og bruken må være forankret i gjeldende godkjenninger fra regionaletisk komite (REK) eller andre relevante myndigheter.

All lagring og behandling av filene må skje i henhold til virksomhetens sikkerhetskrav for håndtering av personpplysninger og forskningsdata. Dette innebærer at:  
* Krypterte eksportfiler skal lagres sikkert og utilgjengelig for uvedkommende. 
* Dekrypterte filer skal kun lagres i mapper eller på lagringrområder som er godkjent av informasjonssikkerhetsansvarlig/personvernombudet, og som oppfyller kravene til sikkerhet, tilgangsstyring og dataminimering. 
* For forskningsprosjekter skal all behandling av data være i tråd med godkjenning fra REK, eventuelle interne forskningsetiske komiteer, samt forskningsprotokollen som regulerer formål, metode og lagringrrutiner. Dette inkluderer også krav om at kun personer med tjenstlig behov og godkjent tilgang kan behandle filene. 

Når formålet med datauttrekket er oppfylt eller når opplysningene ikke lenger er nødvendige for forskningsprosjektet skal eksportfilen slettes på en sikker og etterprøvbar måte. Sletting skal gjennomføres i samsvar med virksomhetens rutiner for datasletting og i tråd med krav fra personvernregelverket, REK-godkjenningen og gjeldende forskningsprotokoll. 
