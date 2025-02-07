# Systemutfylte felt

Et systemutfylt felt vil automatisk fylles ut ved opprettelse, endring eller ferdigstillelse.
Vedkommende som fyller ut skjema har ikke muligheten til å fylle ut eller endre disse feltene. 
Dette er typisk brukt for metadata som skjemaets unike nøkkel, alder, kjønn og lignende. Det er viktig å tenke nøye gjennom hvilke systemutfylte felter som er nødvendige for hver enkelt studie og velge de aktuelle før man starter skjemabygging og datainnsamling. 

### Brukeren som opprettet skjemaet sin unike ID 

En unik ID generert av FALK som tilhører personen som har opprettet skjemaet i eFORSK. 

### Brukeren som opprettet skjemaet sitt navn 

Navnet til brukeren som opprettet skjemaet i eFORSK.

### Formel

I formler kan man hente inn verdier fra andre felter. Hvis man har et tallfelt med variabelnavn Tall, skriver man \[\_Tall\_\] i formelen for å få feltets verdi. Har ikke feltet en verdi (ubesvart/tomt), vil den beregnes med verdien 0 i formelen.

Datoer vil transformeres til antall sekunder siden 1970 slik at dem kan brukes i formler, se eksempel under.

Lager man en formel (B) som skal hente verdien fra en annen formel (A), er det viktig at feltet med formel (A) opprettes før formel (B).

<a href="https://github.com/pieterderycke/Jace/wiki" target="_blank">Detaljert informasjon om bygging av formler</a>

#### Eksempel 1: enkel formel
`([_Tall1_] + [_Tall2_]) / [_Tall3_]`

OBS: deling på 0 gir feil (ubesvarte felter gir verdi 0 i formler). En løsning kan være;

`([_Tall1_] + [_Tall2_]) / if([_Tall3_]==0, 1, [_Tall3_])`

#### Eksempel 2: bruk av funksjoner
`max([_Tall1_], [_Tall2_], [_Tall3_])`

Gir høyeste verdi av de tre feltene

#### Eksempel 3: avansert formel
`2 * median([_Tall1_], [_Tall2_], [_Tall3_]) / 2E-3`

#### Eksempel 4: bruk av datoer
`([_Datofelt2_] - [_Datofelt1_]) / 86400`

Antall dager mellom datoene Datofelt1 og Datofelt2

`([_Datofelt2_] - [_Datofelt1_]) / 32000000`

Antall år mellom datoene Datofelt1 og Datofelt2. Obs: beregning av alder er utfordrende grunnet skuddår.

#### Begrensninger

Systemutfylte felter med formel kan ikke brukes til å sammenligne med i regler i skjematypen. Dette kommer av hvordan formlene blir beregnes av systemet.

I et ePROM skjema vil ikke formlene beregnes før skjemaet er levert og ankommet eFORSK.

### Forskningsobjektets alder ved skjemaopprettelse

Alderen til forskningsobjektet på tidspunktet for skjemaopprettelse. 

### Forskningsobjektets bostedsgate ved skjemaopprettelse

Bostedsgaten til forskningsobjektet på tidspunktet for skjemaopprettelse. 

### Forskningsobjektets distriktskode ved skjemaopprettelse 

Distriktskoden til forskningsobjektet på tidspunktet for skjemaopprettelse. Distriktskode gjelder bare forskningsobjekter bosatt i Trondheim, Oslo eller Bergen. 

### Forskningsobjektets dødsdato

Datoen for eventuelt dødsfall til forskningsobjektet. 

### Forskningsobjektets fødselsdato 

Fødselsdatoen til forskningsobjektet. 

### Forskningsobjektets id/fødselsnummer

Forskningsobjektets fødselsnummer, eller eventuelt ID. Dette systemutfylte feltet er valgt by default.

### Forskningsobjektets kjønn 

Kjønnet til forskningsobjektet. 

### Forskningsobjektets kommunenummer ved skjemaopprettelse 

Kommunenummeret til forskningsobjektet på tidspunktet for skjemaopprettelse. 

### Forskningsobjektets navn

Navnet til forskningsobjektet. 

### Forskningsobjektets postnummer ved skjemaopprettelse 

Postnummeret til forskningsobjektet på tidspunktet for skjemaopprettelse. 

### Forskningsobjektets poststed ved skjemaopprettelse 

Poststedet til forskningsobjektet på tidspunktet for skjemaopprettelse. 

### Forskningsobjektets unike nøkkel 

En systemgenerert nøkkel som er unik for forskningsobjektet. Dette systemutfylte feltet er valgt by default. 

### Registrerende tilgangenhets id/navn

Navnet eller ID-en til tilgangsenheten. Anbefales å brukes dersom man har flere tilgangsenheter. Denne vil da sørge for at man kan se hvilken enhet skjemaer er registrert på.

### Skjemaet sin monitoreringsstatus

Monitoreringsstatusen til skjemaet. Statusen kan være "Ikke vurdert", "til monitorering" eller "godkjent". Les mer under "Skjema" i brukermanualen. 

### Skjemaet sin samtykkestatus 

Viser samtykkestatusen til skjemaet. 

### Skjemaet sin status 

Dette systemutfylte feltet er valgt by default. 

### Skjemaet sin unike nøkkel 

Dette systemutfylte feltet er valgt by default. 

### Skjemaets foreldreskjema sin unike guid 



### Skjematypens navn 

Navnet til aktuelle skjematype.

### Skjematypens unike id

Skjematypene har unike ID-er. Dette systemutfylte feltet er valgt by default. 

### Skjematypens versjonsnummer 

Dette systemutfylte feltet er valgt by default. 

### Tidspunktet skjemaet ble ferdigstilt første gang 

Dette systemutfylte feltet er valgt by default. 

### Tidspunktet skjemaet ble opprettet 

Dette systemutfylte feltet er valgt by default. 

### Tidspunktet skjemaet sist ble oppdatert

Dette systemutfylte feltet er valgt by default. 

### ePROM bestillingstidspunkt 

Dersom skjematypen har aktivert ePROM anbefales det å legge til relevante systemutfylte felter, som feltet ePROM bestillingstidspunkt. Dette må vurderes for hver enkelt skjematype. 

### ePROM brukernavnet til bestiller 

Dersom skjematypen har aktivert ePROM anbefales det å legge til relevante systemutfylte felter, som feltet ePROM brukernavnet til bestiller. Dette må vurderes for hver enkelt skjematype. 

### ePROM svartidspunkt

Dersom skjematypen har aktivert ePROM anbefales det å legge til relevante systemutfylte felter, som feltet ePROM svartidspunkt. Dette må vurderes for hver enkelt skjematype. 

### ePROM varslingskanal

Dersom skjematypen har aktivert ePROM anbefales det å legge til relevante systemutfylte felter, som feltet ePROM varslingskanal. Dette må vurderes for hver enkelt skjematype. 
