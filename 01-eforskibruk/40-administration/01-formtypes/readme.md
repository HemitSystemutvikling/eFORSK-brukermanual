# Skjematype

En skjematype er oppsettet og egenskaper av felter og regler det skal registreres på. 
Man kan velge å opprette en ny skjematype, kopiere en allerede eksisterende skjematype eller bruke standardskjematyper.

## Arkitektur

Man må tenke grundig igjennom hvilke skjematyper man skal ha før man oppretter dem. 

Alle spørsmål som skal besvare samtidig bør/må plasseres i en og samme skjematype. La oss si at man skal la forsningsobjekter besvare EQ5D, HeartQol og et egendefinert sett med spørsmål. Da bygger man ny skjematype med utgangspunkt i standardskjematyper, der man velger EQ5D og HeartQol. Deretter legger man i skjematypen til en ny gruppe hvor man plasserer alle de egendefinerte spørsmålene. Man kan nå bestille skjemautfyllelse en gang for alle spørsmålene, og forskningsobjektet får kun ett skjema (en skjemapakke) tilsendt.

Har man avhengigheter mellom skjematyper, eksempelvis at et inklusjonsskjema har informasjon om forskningobjektet som fører til bestilling av et PROM skjema med relasjon tilbake til inklusjonsskjemaet. Se "Skjematypen skal være underskjematype av" nedenfor.

## Bygg ny skjematype

Når man skal bygge ny skjematype må man gjøre noen valg som ikke kan gjøres om på senere. Unntaket er skjematypens navn, dette kan når som helst endres etter opprettelse.

### Utgangspunkt

Her har man følgende valg:

#### Ny skjematype
Her får man et tomt utgangspunkt, kun med noen foreslåtte systemutfylte felter

#### Kopi av eksisterende skjematype
Her kan man velge en eksisterende versjon av en skjematype, og få gjenskapt en kopi av denne

#### Importer fra fil
Her kan man laste opp fil som tidligere er eksportert fra en eksisterende skjematype, under valget "Eksporter skjemadefinisjon". Dette gjør at man kan flytte skjematyper mellom databaser.

### Skjematypen skal være underskjematype av

Hvis man har avhengigheter i mellom skjematyper, kan man velge at en skjematype er underskjematype av en annen. Da får man et ekstra systemutfylt felt som har den unike nøkkelen til foreldreskjemaet, som kan nyttes for å koble data. 

Et typisk eksempel er at skjematypen "Spørreskjema 30 dager etter utskrivelse" er en tilknyttet skjematype til "Inklusjonsskjema". Her kan man for eksempel sette opp automatisk utsendelse av spørreskjemaet 30 dager etter at inklusjonsskjemaet er opprettet.

### Type forskningsobjekt

Skjemaer som fylles ut av skjematypen må være tilknyttet en forskningsobjekttype. Forskningsobjekttyper settes opp under "Administrasjon". Skal man samle inn data på medisiner, må man opprette en forskningsobjekttype som heter "Medisiner", og deretter velge denne ved opprettelse av skjematypen. 

Skal man bruke ePROM er man nødt til å velge "Personer fra personregisteret". "Personer fra personregisteret" gir også en del ekstra muligheter for data med systemutfylte felter, for eksempel kjønn og adresse.

## Bygg ny skjematype fra regneark

En alternativ måte å raskt komme i gang med å bygge en skjematype er å lage seg et regneark med variabler og eksempeldata.

| Spoersmal1 |	EtTall |	EtAnnetTall |	FriTekst |	Skala |	BesoksDato |
| -- |	-- |	-- |	-- |	-- |	-- |
| 1: Ja	| -5	| 1.01 | Tekst| 	1: Veldig bra| 	22.10.2019 |
| 2: Nei	| 10	| | 	|	2: Ganske bra	| |
| 9: Ukjent  | | | 	|		3: Middels	
| | | | | 			4: Ganske dårlig	| |
| | | | | 				5: Veldig dårlig	| |

Regnearket importerer man så under "Verktøy" og "Importer data". Der velger man "Opprett ny skjematype fra importdata". Variablene anaylseres, og man må gå over og velge riktig felttype før man går videre til skjemabyggeren.

Systemutfylte felter (fødselsnummer, kjønn osv), samtykkefelter og randomiserte felter skal ikke tas med i regnearket, men opprettes i skjemabyggeren etterpå.
