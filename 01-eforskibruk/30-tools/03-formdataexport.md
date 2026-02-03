# Eksporter data

Når man eksporterer data blir hvert felt i skjematypen en egen kolonne med variabelnavnet som overskrift. Rekkefølgen på feltene kan bestemmes av databaseansvarlig ved redigering av skjematypen. Eksport gjøres via **Verktøy** - **Eksporter data**, alternativt under valget **Bruk disse** under fanene "ePROM bestillinger" eller "Skjema" i hovedmenyen.  

## Redigere rekkefølge i dataeksport

* Åpne den aktuelle skjematypen
* Velg fanen Felter. Her vises alle felter skjematypen inneholder, inkludert metadatafelt
* Trykk på **Rediger rekkefølge** øverst til høyre, dette gir to alternativer:
   - Flytt felt manuelt opp eller ned med pilene til høyre for hvert felt
   - Sorter felter etter skjemaversjon, som velges øverst. Da vil feltene i eksporten sorteres i samme rekkefølge som de vises i den aktuelle skjemaversjonen
* Velg **Lagre rekkefølge**

## Filformat

Ved eksport av data får man en kryptert zip-fil. For å pakke ut denne filen trenger man:
* Et program som kan pakke ut zip-filer som er kryptert med AES 256-standarden, for eksempel 7-Zip
* Passordet som oppgis ved eksportering av data, denne får man bare en gang

Innholdet i zip-fila velges ved eksport, csv og xlsx støttes.

## Samtykkeeksport

For eksport av samtykker til dokumentasjonsformål, gå til **Verktøy** - **Eksporter data** og velg aktuelle skjematype du ønsker å eksportere samtykker for. Beskriv formålet med eksporten, ønsket format, ta stilling til om du trenger personidentifiserbare data og metadata og huk av valget **Eksporter som samtykkedata**for å inkludere en PDF-fil med alle samtykker for aktuelle skjematype. 

## Ansvar

Eksportfilene og innholdet i disse må behandles i henhold til personopplysningsloven. 
Opplysningene kan bare behandles i henhold til det formål opplysningene er innsamlet for.

Lagring av filen må være i henhold til de sikkerhetskrav som gjelder for slike opplysninger i virksomheten. 
Filen i dekryptert form må kun lagres i sikre mapper godkjent av informasjonssikkerhetsansvarlig/personvernombudet og i tråd med forskningsprotokoll.

Når formålet med uttak av filen er oppfylt skal den slettes i henhold til krav til sletting.
