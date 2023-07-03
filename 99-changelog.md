# Endringslogg


Her finnes en oversikt over de viktigste endringene i funksjonalitet mellom versjonene.

## Versjon 9.1.2 (tentativt august 2023)

### Feilretting
* Superbruker: rollen superbruker vil kunne se om et forskningsobjekt er død ved ePROM-bestilling, og det er ikke mulig å bestille ePROM-skjema til døde forskningsobjekt
* ePROM: bestillingstidspunkt for skjema levert via lenke vises riktig. Bestillingstidspunkt tilsvarer tidspunktet når forskningsobjekt logget inn for å svare på skjema
* Feilmelding på startsiden  - "Denne siden finnes ikke" - vises ikke lenger ved innlogging

## Versjon 9.1 (13. april 2023)

* Dette er i hovedsak en teknisk oppgradering til .NET 6, med få funksjonelle endringer

### Feilretting
* Eksport av brevutsendinger inkluderer alle utsendinger, ikke begrenset til de 25 første

## Versjon 9.0.1 (14. februar 2023)

### Feilretting
* Forskningsobjekt: Skjemaliste viser nå alle forskningsobjektets skjema, også i tilfeller med ferdigstilt underskjema og hovedskjema i kladd på underenheter.

## Versjon 9.0 (2. februar 2023)

### Ny funksjonalitet
* Forskningsobjekt: Fra og med versjon 9.0 vil forskningsobjekter som slettes fjernes fullstendig fra eFORSK. Det vil si at forskningsobjektet kan søkes opp som en ny pasient etter at sletting er gjennomført. Dette gjelder forskningsobjekter fra Personregisteret.
* Forskningsobjekt: Mulighet for å eksportere koblingsnøkkelfil, som angir koblingen mellom fødselsnummer og forskningsobjektets unike id i eFORSK 
* Eksport av data: Filer som lastes ned kryptert og zippet lagres nå som filtype .7z (7-Zip). Det vil gjøre det enklere å pakke ut, dekryptere og åpne filene.
* Brevutsendelse: Mulighet for å opprette og fylle ut skjema basert på listen over utsendte brev (ved hjelp av "Bruk disse"-funksjonen)
* Brevutsendelse: Mulighet for å gjøre ePROM-bestilling basert på listen over utsendte brev (ved hjelp av "Bruk disse"-funksjonen)
* Skjema: Mulighet for å opprette og fylle ut nye skjema basert på listen over eksisterende skjema (ved hjelp av "Bruk disse"-funksjonen)

### Feilretting
* Skjemabygger: Skjema som inneholder kun felt av typen informasjonstekst blir nå vist i listen over samleskjema
* Skjemabygger: Formattering av tekst i felt av typen informasjonstekst er rettet slik at teksten vises riktig
* Administrasjon: Endring av databaseinnstillinger fungerer nå både ved å trykke på tekst og sjekkbokser
* Brev: Filnavn kan inneholde maksimalt 100 tegn

## Versjon 8.0 (1. desember 2022)

### Ny funksjonalitet
* Skjemabygger: Mulighet for å endre rekkefølger på variabler i skjemaet til dataeksport, basert på oppsett i skjemabygger. 
* Skjemabygger: Forbedret bygging av skjematyper via import/kopi. Bygging skjer som bakgrunnsjobb og eFORSK gir tilbakemelding til brukere når skjemaene er ferdigbygget og kan brukes.
* Skjemabygger: Import og kopi  av skjematyper tar nå med alle ePROM-innstillinger fra den opprinnelige skjematypen.
* Randomisering: Superbruker kan få se blokkstørrelser på randomiseringer som er aktive.
* ePROM: Utvidet maksimum antall dager som kan settes for en automatisk bestillingsjobb (fra 99 dager til 5 år).

### Feilretting
* Skjemabygger: Fikset problemer med import/kopi av skjematyper som kræsjet i klient og opprettet tomme skjematyper.
* Skjemabygger: Kopi av eksisterende skjematype og kopi av felter tar nå også med hjelpetekster (manglet tidligere)
* Skjema: Valgfelt med alternativ som har 0-verdi kan nå velges først

## Versjon 7.2 (25. august 2022)

### Feilretting
* Administrasjon: Endret formattering av telefonnummer til å godta landskode for å støtte sms-varsel av hendelser
* ePROM: Fjernet mulighet for å angi dager mellom og påminnelse da dette ikke lenger er støttet av helsenorge

## Versjon 7.1 

### Ny funksjonalitet
* Randomisering: Ny innstilling for databaser - Mulig å tillate eksponering av aktive randomiseringsresultater i dataeksport for alle aktuelle roller. 



## Versjon 7.0 (13. juni 2022)

### Ny funksjonalitet
* Skjemabygger: Mulighet for å legge til Standardskjema inne i skjemabygger, også på en opprettet skjematype.
* Skjemabygger: Ny standard-mal for skjemabygging - tilrettelagt for bruk av "Hovedgrupper" på øverste nivå i skjemaet. Bygger videre på ytelsesforbedring gjort i skjemabygger i versjon 6.0, muligheten for ePROM skjemaoppdeling, og muligheten for å legge til standardskjema i skjemabygger.
* Skjemabygger: Tilbyr skjemaoppdeling i ePROM-skjema som et valg i skjemabygger (aktivert som en standard). Hver "Hovedgruppe" i skjemaet blir da et eget underskjema i ePROM-utsendingen som sendes ut som ett samleskjema. Kan leses mer om i brukermanual under "ePROM aktivering". Krav i oppbygning av skjema for å kunne benyttes.
* Skjemabygger: Forbedret visning i skjemabygger for å framheve "Hovedgrupper", og forbedret visningen av validerings-tilbakemeldinger inne i lukkede grupper.
* Skjemabygger: Utlistet navn over elementer under "Flytt"-valget er utvidet for å lettere lese og skille mellom elementer i skjemaet.
* Import: Import av skjemadefinisjon nå samtykkehåndtering for det nye skjemaet hvis skjemadefinisjon inneholder samtykkefelt. Aktiverer også ePROM for skjemaet hvis skjemadefinisjonen hadde ePROM aktivert.
* ePROM: Mulighet for oppdeling i flere ePROM-skjema i ePROM-utsending, basert på hovedgrupper i eFORSK-skjema.
* ePROM: Mulighet for ePROM-utsendinger til mottakere mellom 16-18 år som har Helsenorge-bruker.
* Randomisering: Konfigurering av randomiseringer kan nå bare utføres av rollen Superbruker.
* Randomisering: Mulighet for å legge til randomiseringsfelt i skjema kan nå bare utføres av rollen Superbruker. 
* Randomisering: Andre roller enn superbruker har mulighet til å se informasjon om randomiseringer og randomiseringsfelter, men ikke redigere eller konfigurere randomiseringer.
* Randomisering: I eksport av skjemadefinisjon er randomiseringsfelt inkludert. Importering av skjemadefinisjon ignorerer randomiseringsfelt. Kopiering av skjemadefinisjon ignorerer randomiseringsfelt.
* Randomisering: Eksport av skjemadata sensurerer randomiseringsfelt med randomiseringer som fortsatt er aktiv, for alle andre roller enn Superbruker.

### Feilretting
* ePROM: Fikset feil med randomiseringsfelt som ikke fungerte i ePROM-skjema 
* Import: Fjernet muligheten for superbruker til å importere skjemadata (fortsatt mulig i andre aktuelle roller)
* Administrasjon: Rettinger i visning over databaser
* Administrasjon: Fjernet mulighet for å godkjenne ePROM-skjema på deaktiverte databaser
* Administrasjon: Superbruker får ikke mulighet til å se oversikt over alle aktive databaser når den er innlogget på en spesifikk database.
* Administrasjon: Fjernet flere visningsmuligheter over databaser som er deaktivert.



## Versjon 6.0 (7. april 2022)

### Ny funksjonalitet
* Skjemabygger: Forbedret ytelse i skjemabygger. Begrenset til at bare en gruppe på toppnivå kan være åpen om gangen, for å redusere treghet/problemer med større skjema. Alle grupper på toppnivå er nå automatisk lukket ved åpning av en skjematype i skjemabygger.
* Roller: Lagt til nye roller Databaseansvarlig Avidentifisert og Superbruker (Ikke tilgjengelig enda)
* Roller: Superbrukere får oversikt over databaser personen er superbruker for (Ikke tilgjengelig enda)
* Roller: Superbrukere får mulighet til å godkjenne digitale ePROM-skjema for databaser personen er superbruker for (Ikke tilgjengelig enda)
* Roller: Leser Anonymisert rollen heter nå Leser Avidentifisert. (Ikke tilgjengelig enda)
* Brukerdetaljer: Oppdatert utlisting av brukerinformasjon.
* ePROM: Økt antallet automatisk bestillingsjobber med ePROM som kan opprettes (fra 10 til 30)
* ePROM: ePROM-bestillinger som evt. feiler underveis i utsending vil pause utsending, og gi bruker mulighetene for å fortsette utsending.
* Skjema: Mulighet for å inkludere metadata av skjematype sammen med eksport av skjemadata.

### Feilretting
* Brukerdetaljer: Optimalisert utlisting av brukerinformasjon så siden ikke skaper problemer.
* Forskningsobjekter: Søk på forskningsobjekter fungerer nå med fødselsdato og navn.
* Eksport av alle skjemabestillinger fungerer nå hvis noen av skjemaene tidligere er slettet.
* ePROM: Verdiintervall på slider i skjemafelt fungerer nå i utsendt ePROM-skjema.
* ePROM: Systemutfylt felt "EPromBestiltTidspunkt" vil kunne legges til og vises i følgebrev
* ePROM: Fikset feil med ePROM-bestillinger som ble avbrutt ved for stort antall bestillinger.
* Oppdatert tekst for felter det ikke er mulig å legge til regler på.



## Versjon 5.0 (11. november 2021)

### Merk:
* Anbefalt antall forskningsobjekter per ePROM-utsending er justert til 500 (tidligere 1000). Dette er en midlertidig løsning for å unngå problemer med ePROM-bestilling, permanent løsning er under arbeid.
* Randomisering må aktiveres igjen for allerede eksisterende databaser ved produksjonssetting av versjon 5.0
* Det legges nå til en tom side på alle brev som blir sendt på papir, så det er lenger ikke nødvendig å sette av plass på første side for addresseinformasjon i brevutsending. Digitale utsendinger og papirutsending vil være like.

### Ny funksjonalitet
* Randomisering: Randomisering er lagt til som en feature som kan velges på databasenivå, som nå kan velges bort for databaser som ikke trenger randomisering. (NB! Må aktiveres igjen for allerede eksisterende databaser ved produksjonssetting av versjon 5.0)
* Randomisering: Tilbakemelding i skjema hvis manuell randomisering ikke gir noe resultat.
* Randomisering: Mulighet for å sette spesifikk størrelse på første randomiseringsblokk.
* Brevutsendelse: Mulighet for å søke i listen over brevutsendinger
* Brevutsendelse: Lagt til informasjon om størrelsesbregrensninger og prissteg for utsending.
* Skjemabygger: Nytt valideringssystem for feilmeldinger og advarsler i skjemabyggeren.
* Skjemabygger: Mulighet for å slette grupper inkludert innholdet i de.
* ePROM: Mulighet for å ikke ikke sende ut purring på ePROM-bestillinger og automatisk bestillingsjobber.
* ePROM: Utsending til personer under 18 år godtar bare "Jeg vil varsle mottaker selv", da andre kanaler ikke kan brukes.
* ePROM: Nytt symbol for valgte mottakere som er under 18 år i ePROM bestillinger.

### Feilretting
* Import av skjemadefinisjon med samtykkefelt feilet.
* Skjemabygger: Randomsering som "Utføres ved skjemaopprettelse" forårsaket kræsj i "Test regler og beregninger" i forhåndsvisning.
* Skjemabygger: "Slett skjematype" bekreftelses-knapp fungerte ikke optimalt.
* Skjemabygger: Man kunne tidligere redigere felter i skjemabygger utenfor redigerings-modus.
* Skjemabygger: ePROM-oppsett hadde påkrevde felter som man kunne omgå.
* Skjemabygger: Grupper og informasjonstekster i skjulte elementer var tidligere synlig i ePROM-skjemaet
* ePROM: Eksport av ePROM-bestillinger feilet ved et stort nok antall bestillinger.
* ePROM: ePROM-bestillingsjobber feilet hvis tillagte regler ble fjernet.
* ePROM: ePROM-bestillingsjobber krevde ikke valg av hvilken skjemastatus som skull trigge bestilling.

## Versjon 4.0 (19. september 2021)
* Mulighet for å skifte rolle eller enhet direkte i header
* Ekstra advarsel ved bekreftelse av brevutsendelse
* Mulighet for å eksportere liste over utsendte brev til excel
* Mulighet for å filtrere på tilgangsenhet i skjemasøk
* Mulighet for å aksessere ePROM bestillingsjobberfra Verktøy-menyen
* ePROM: Tydeliggjort informasjon i ePROM-oppsett og samstemt variabelnavn med forhåndsvisning av skjema i ePROM
* ePROM: Fjernet mulighet for å "ikke sende kopi av besvart skjema til utfyller" hvis man har valgt innhenting av samtykke-signatur i ePROM-besvarelse

## Versjon 3.1.1 (21. januar 2021)
### Feilretting
* Kopiering av grupper i skjemabygger skapte problemer når fjernede regler eller fjernede felter var involvert
* Skjemabygger: Forhåndsvisning av formler (systemutfylt felt) ble ikke beregnet

## Versjon 3.1 (15. desember 2020)
* Skjemabygger: Mulighet for å kopiere grupper
* Brevutsendelse: Mulighet for farger
* Mulighet for å opprette skjema på flere forskningsobjekter samtidig, for videre utfylling i massevisningsmodus
* Randomisering: Randomiseringsresulateter vil nå vises ved eksport av skjemadata selv om randomiseringen ikke er avsluttet, mens blokkstørrelsene vil skjules isteden
### Feilretting
* Rettet feil ved eksportering av skjemadata der datofelter kunne komme i feil tidsone 

## Versjon 3.0.1 (5. november 2020)
* Hvis en person starter utfylling av ePROM via lenke, men ikke fullfører/leverer, vil dette dukke opp som en utløpt ePROM bestilling i eFORSK to dager etterpå
### Feilretting
* Rettet feil ved bruk av LeserAnonymisert rollen

## Versjon 3.0 (26. oktober 2020)

* Mulighet for å slette forskningsobjekter
* Mulighet for å deaktivere og slette tilgangsenheter
* Forbedringer rundt visning av tilgangsenhet
* Bedre funksjonalitet for å styre hvilke funksjoner som er tilgjengelig på ulike tilgangsenheter innad en database
* ePROM: Nytt valg i skjemabygger for å ikke sende kopi av besvart skjema til utfyller sin Helsenorge-konto eller digitale postkasse
* ePROM: når papirskjema i posten ikke kommer frem til mottaker og blir returneret (grunnet feil adresse f.eks.) blir status på bestillingen nå "Feilet" istedenfor tidligere "Utgått", da status "Utgått" kun burde brukes for digitale bestillinger der mottaker har hatt en mulighet til å svare.
* ePROM: flere muligheter for å spesifisere tekst i melding som går til Digipost og Helsenorge
* ePROM: mulighet ved bestilling å forhindre bestilling hvis forskningsobjektet allerede har et skjema eller en aktiv (status: planlagt eller bestilt) bestilling av valgt skjematype
* Skjemabygger: mulighet for  å flytte til topp eller bunn av gruppe
* Separat applikasjon for å lese brukermanualen
* Forbedret grensesnitt rundt redigering av rekkefølge på felter. Fikset feil ved lagring av ny rekkefølge
* Forbedret grensesnitt på skjemasiden (statusendring)
* Mulighet for å legge inn kommentarer på forskningsobjekter og i skjemaer
* Massevisningsmodus for skjema, nytt valg under "bruk disse" i skjemautlistinger
* Støtte for enkel monitorering av skjema
* Nye systemutfylte felter: Monitoreringsstatus og samtykkestatus
* Wysiwig tekstredigering på enkelte steder
#### Feilretting
* Rettet feil der dataansvarlig ikke kunne se hendelser
* Rettet feil ved lagring av sortering av felter inne på en skjematype
#### Kjente feil
* Kan oppleve feil ved bruk av LeserAnonymisert rollen

## Versjon 2.0.1 (mars 2020)
* Rettet feil der eksport av ePROM bestillinger eksporterte maksimum 25 stk

## Versjon 2.0 (16. desember 2019)

* Mulighet for å sende ut brev (PDF) til personer i personregisteret (helsenorge, sikker digital postkasse eller i posten)
* Nytt system for samtykkehåndtering
* System for hendelsesovervåking
* Mulighet for å skjule fjernede felter i skjemabygger
* Mulighet for å styre muligheten for å bestille skjemautfyllelse (ePROM) per tilgangsenhet
* Stratifisert blokkrandomisering: utvidet mulig felter som kan brukes som stratifiseringskategorier til også å gjelde avkryssningsfelt, samtykkefelt og det systemutfylte feltet "registrerende tilgangenhets ID"
* Ny hendelseslogg på forskningsobjekter, vist som tidslinje
* Mulighet for å ha registrering av klokkeslett på datofelt
* Mulighet for å sammenligne med tallfelt på "Vis hvis" regler
* Nytt systemutfylt felt: Formel
* ePROM: Bedre mulighet for å styre tekster i Helsenorge og sikker digital postkasse i skjemabyggeren
* ePROM: Mulighet for å skjule fremdriftindikator i ePROM skjema
* ePROM: Ny regel for å kunne skjule utfyllingshjelp på papirskjema
* ePROM: Mulighet for å bestille ePROM utfylling via E-post og SMS hentet fra kontaktregisteret. 
* ePROM: Forbedret valg av varlingskanaler ved ePROM bestilling
* ePROM: Forbedret funksjonalitet for automatiske ePROM bestillinger
* ePROM: Forbedret søkefiltre for bestillinger
* Nye regler på datofelt: fortid, mindre enn (verdi), mindre enn annet felt, mindre enn eller lik (verdi), mindre enn eller lik annet felt, større enn (verdi), større enn annet felt, større enn eller lik (verdi), større enn eller lik annet felt, lik (verdi), ulik  (verdi)
* Nye regler på tallfelt: mindre enn (verdi), mindre enn annet felt, mindre enn eller lik (verdi), mindre enn eller lik annet felt, større enn (verdi), større enn annet felt, større enn eller lik (verdi), større enn eller lik annet felt, lik (verdi), ulik (verdi)
* Ny regel på avkryssningfelt: påkrevd svar
* Nye kommunenummer for 2020 ved personsøk
#### Kjente feil
* Eksport av ePROM bestillinger eksporterer maksimum 25 stk
* Kan ikke se hendelser med rollen dataansvarlig
* Feil ved lagring av sortering av felter inne på en skjematype
* Lang avsendernavn på brevutsendelse vil skape feil ved utsendelse i ePROM, bør holde seg innenfor 21 tegn inntil videre (løses sansynligvis med ny versjon av ePROM 14. mai)

## Versjon 1.2 (8. oktober 2019)

* Forbedringer i "Finn forskningsobjekt" funksjon. Kan nå laste opp fil med IDer. Antall samtidige i visning er satt til 1 000.
* Nye systemutfylte felter: Forskningsobjektets navn, Forskningsobjektets poststed ved skjemaopprettelse, Forskningsobjektets bostedsgate ved skjemaopprettelse, Brukeren som opprettet skjemaet sitt navn
* Mulighet for stikkordsøk i brukermanual
* Tekstlig visning av skjemadata, kopierbar til andre systemer
* Forbedringer ved validering av variabelnavn
* Forbedringer i skjemabygger rundt forhåndsvisning og tillegging av systemutfylte felter

## Versjon 1.1 (26. august 2019)

eFORSK lanseres, pilotperiode avsluttes.

* Mulighet for identifiserbar eksport av ePROM bestillinger
* Mulighet for å låse skjemaversjoner, slik at skjemaer utfylt i versjonen ikke kan endres
* Mulighet for å se verdien til skjulte elementer på et skjema inne i eFORSK
* Bedre støtte for varsler: Databaseansvarlig kan opprette varsler som vises for alle brukere av databasen. Brukes også for å varsle oppgradering av eFORSK.
* ePROM Personinitiert utfyllelse tilgjengelig for alle med ePROM aktivert
* Mulighet for verdier fra felter inn i informasjonstekst til mottaker ved ePROM bestilling
* Kan nå slå opp forskningsobjektet med dens unike nøkkel

#### Feilretting

* Rettet feil med funksjonen "Slå opp unik nøkkel" på skjema-siden
* Rettet feil der skjemastatus og sist oppdaterttidspunkt ikke ble oppdatert ved status "til kontroll" på skjema.
* Rettet feil med funksjonen "last ned skjematype metadata" under verktøy

## Versjon 1.0 (17. juni 2019)

* Løsning for flervalgsfelt
* Mulighet for å legge ePROM bestillinger frem i tid
* Mulighet for eksport av ePROM bestillinger til regneark
* ePROM Personinitiert utfyllelse (tilgjengelig kun ved forespørsel)
* Automatiserte ePROM bestillinger (tilgjengelig kun ved forespørsel)
* Mulighet for å etterspørre samtykke ved ePROM bestilling selv om samtykke allerede foreligger
* Import av skjemadata (tilgjengelig kun ved forespørsel)
* Diverse rettelser for nettleseren Edge
* Rettet visning av tidspunkter i systemutfylte felter til å ha korrekt tidssone
* Roller i Falk på plass
* Samtykketekst konfigureres nå per skjematypeversjon, og ikke felles for hele databasen

## Versjon 0.9 (mars 2019)

Dette er første versjon av eFORSK, til bruk for piloteringsprosjekter.
