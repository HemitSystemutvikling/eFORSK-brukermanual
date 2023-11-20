# Randomisering

Det er kun Superbruker som har tilgang til å administrere randomiseringer.

Randomisering kan gjøres på to måter i eFORSK:
- ved å legge inn randomiseringsfelt i skjematyper
- ved å utføre en hurtigrandomisering på et utvalg forskningsobjekter 

Hurtigrandomisering kan brukes for randomisere en gitt liste med forskningsobjekter umiddelbart uten å gå veien via skjemaer. Dette brukes gjerne når man skal bruke randomiseringsresultatet videre i andre applikasjoner enn eFORSK.

En avluttet randomisering kan ikke "startes" igjen (bortsett fra i testmodus).

## Randomiseringsmetoder

Valg av riktig randomiseringsmetode er et ansvar som ligger hos hvert enkelt prosjekt. Det er viktig å gjøre en vurdering av behovet, da randomiseringsmetode kan komplisere analysen av data i ettertid. Under følger en kort forklaring av de ulike randomiseringsmetodene som er tilgjengelig i eFORSK:

### Enkel randomisering
Enkel randomisering innebærer at hvert forskningsobjekt tildeles en gruppe etter "mynt og kron"-prinsippet. Det vil si at tildelingen ikke påvirkes av tidligere tildelinger eller påvirker framtidige tildelinger. Det betyr at rekkefølgen blir tilfeldig, men kan ha uheldige effekter spesielt når antall forskningsobjekter er lite.

### Blokkrandomisering
Blokkrandomisering sikrer at at det på et hvilket som helst tidspunkt i inklusjonsperioden er omtrent like mange forskningsobjekter som er tildelt til de ulike gruppene (randomiseringsmulighetene). Det er mest hensiktsmessig å benytte mange mindre blokker for å unngåe systematiske forskjeller i fordelingen mellom blokkene i inklusjonsperioden. Med to ulike grupper (randomiseringsmuligheter) A og B som er vektet likt, og en blokkstørrelse på 8, vil blokkrandomisering sørge for at 4 forskningsobjekter tildeles gruppe A og 4 tildeles gruppe B.

### Stratifisert blokkrandomisering
Stratifisert randomisering innebærer at randomiseringen skjer basert på egenskaper hos forskningsobjektet. Det kan f.eks. være alder eller kjønn eller behandlingssted. Imidlertid er det viktig å bruke stratifisering kun på egenskaper som vil kunne påvirke utfallet. I eFORSK benyttes stratifisert randomisering sammen med blokkrandomisering. Stratifiseringen skjer da på grunnlag av felter, synlige eller skjulte, som ligger på det aktuelle skjemaet.

### Utførelse av randomsering
For randomiseringsfelt i skjema er det mulig å konfigurere når randomiseringen skal utføres, gitt noen unntak ved bruk av ePROM*. Valgene forskjellige valgene for utførelse er:
- Manuelt ved klikk på knapp i skjema
- Automatisk ved skjemaopprettelse
- Automatisk ved første ferdigstillelse

**ePROM-unntak:**

*For skjema som sendes i ePROM-bestilling vil både valget for "Manuelt ved klikk" og "Automatisk ved skjemaopprettelse" begge føre til at randomisering utføres ved bestillingstidspunktet.

*Stratifisert blokkrandomisering kan **ikke** utføres ved skjemaopprettelse i ePROM-bestillinger. For stratifisert blokkrandomsering i ePROM-bestillinger vil randomiseringen utføres etter at skjema er levert **uavhengig** av hva som er konfigurert på feltet.

## Eksport av randomiseringsdata
Eksportering av data som inneholder felter med aktive randomiseringer (ikke avsluttet) vil i utgangspunktet sensureres i eksporten for alle andre roller enn Superbruker. 
Det er mulig å konfigurere hver enkelt database til å vise aktive randomiseringsdata i eksport for alle aktuelle roller. Dette styres av adminstrator, og kan spesifiseres i brukeravtalen når det opprettes en ny database.

