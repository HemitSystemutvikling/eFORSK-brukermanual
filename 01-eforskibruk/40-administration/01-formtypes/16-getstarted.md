# Skjemabygger 1-2-3

Du kan opprette et skjema i eFORSK ved å:
- Lage en helt ny skjematype
- Kopiere en eksisterende skjematype
- Importere skjematype fra en fil du laster opp


Uansett valg kommer du videre til **skjemabyggeren** når du skal designe skjemaet ditt i eFORSK. 

På øverste nivå i skjemabyggeren under «Legg til element», kan du legge til to typer elementer:
- Hovedgrupper
- Standardskjema


## Hovedgrupper

Hovedgrupper er grupper som ligger på øverste hierarkinivå i et skjema. Det er bare mulig å ha *en* slik hovedgruppe åpen til enhver tid i skjemabyggeren. Hovedgrupper kan flyttes inn i andre grupper, og grupper som ligger inne i hovedgrupper kan flyttes til øverste nivå.


Dersom «Vis hovedgrupper som egne skjema i ePROM» er aktivert er det ikke mulig å ha regler på hovedgrupper, eller mellom felter som ligger i ulike hovedgrupper. Du vil få opp en advarsel dersom dette skjer. 

Det er anbefalt å opprette egne hovedgrupper for en tematisk inndeling, for eksempel en hovedgruppe for samtykke, en for bakgrunnsinformasjon, studiespesifikke spørsmål, oppfølgingsspørsmål og lignende. Inne i en hovedgruppe kan man legge til felter av alle typer, inkludert nye undergrupper, og regler tilhørende disse feltene: 
- Gruppe
- Informasjonstekst
- Valgfelt
- Avkrysningsfelt
- Tallfelt
- Datofelt
- Tekstfelt
- Systemutfylte felt
- Samtykkefelt 


**Gruppe:** Tillater gruppering av innhold i skjemabyggeren. 

**Informasjonstekst:** Brukes etter behov. Kan inneholde informasjon som er relevant for hvordan studiedeltaker skal fylle ut skjematypen. 

**Samtykkefelt:** Digital samtykkehåndtering kan aktiveres for hver enkelt skjematype. Dette gjøres som et eget valg i høyre kolonne og må kombineres med et samtykkefelt i selve skjemabyggeren. Samtykke gir to svaralternativer: *Jeg samtykker/Jeg samtykker ikke*. Dette genererer et samtykkesymbol på skjemasvaret og gir oversikt over hvilke forskningsobjekter som har samtykket (grønt symbol) og ikke (rødt symbol). Det er også mulighet for å sette opp delvis samtykke ved flere innad i samme prosjekt.

**Valgfelt:** Med dette valget kan studiepasient bare svare ett svaralternativ til tilhørende spørsmål i feltet. Visningstekst i valgfelt er teksten som vises i skjemaet (typisk et spørsmål). Variabelnavn er teksten som blir stående i dataeksporten og kan inneholde maks 50 tegn (A-Z, tall og _). Hjelpetekst kan benyttes supplerende dersom det er behov for å utdype spørsmålet ytterligere. Det er mulig å legge til, fjerne og revidere svaralternativene for spørsmålet under «Alternativer» for å få ønsket format på datasettet i en senere eksport. Dersom du ønsker at spørsmålet skal være obligatorisk å svare på, krysses det av "Feltet må besvares". Studiepasient får ikke levert skjemaet dersom dette er huket av og aktuelle spørsmål ikke er besvart. 

**Avkrysningsfelt:** Benyttes dersom utfyller skal kunne velge flere enn ett alternativ. For å bygge et spørsmål med flervalgsfelt velger man «gruppe» og skriver spørsmålet. For hvert mulige svaralternativ velger man et nytt «Avkrysningsfelt» og skriver inn passende visningstekst og variabelnavn for alternativet. 

**Tallfelt:** Benyttes dersom studiedeltaker skal svare på spørsmålet i tallformat. Her er det blant annet mulig å sette minimums- og maksimumsverdi, velge enhet og desimaler, samt velge om det skal besvares med siffer eller langs en slider. 

**Datofelt:** Velges dersom studiepasient skal svare i datoformat. 

**Tekstfelt:** Med dette valget kan man be studiepasienten svare i form av fritekst. 

**Systemutfylte felt:** Her velger man data om studiepasienten som man ønsker skal være tilgjengelig i en senere dataeksport. Disse valgene vil ikke være synlige for studiedeltaker som fyller ut skjematypen via ePROM selv om de er synlige for den som bygger skjemaet i eFORSK-forhåndsvisningen. Enkelte av feltene hentes fra Folkeregisteret. Hvilke systemutfylte felt man ønsker velges under skjemabygging under «Skjulte elementer». **Merk at dette må tas stilling til under skjemabygging og før utsending og at det er for sent å legge på systemutfylte felter etter at skjemaet er besvart.**

**Skjemaregler:** Det er mulig å legge på andre skjemaregler enn obligatoriske felt, som for eksempel «vis hvis». Dette gjør at et forhåndsbestemt svar utløser eller fjerner et annet spørsmål i tråd med valgt oppsett under «vis hvis». Det er viktig å teste at alle slike regler fungerer. Dette gjør man under fanen «Forhåndsvisning» i eFORSK. 


## Standardskjema
Et utvalg standardskjemaer er tilgjengelige i eFORSK. Dette er ferdig, kvalitetssikrede spørreskjema som brukes slik det er — uten at forskeren selv designer spørsmålene. Dette sikrer kvalitet, reliabilitet og sammenlignbarhet i forskningen. Et standardskjema er låst og kan ikke endres. Husk at ved bruk av standardskjematyper er man selv ansvarlig for å overholde eventuelle lisenser disse måtte ha.

Ved bruk av flere standardskjematyper som skal besvares samtidig, eksempelvis EQ5D og RAND12, er det i eFORSK anbefalt å samle disse i en skjematype. Ved bestilling av utfyllelse (via ePROM) kan mottaker da besvare alt samtidig, istedenfor å motta flere separate skjemaer som øker terskelen for å fullføre utfyllelsen.


