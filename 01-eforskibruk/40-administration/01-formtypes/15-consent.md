# Samtykkehåndtering

Ønsker man å innhente samtykke gjøres dette med skjemaer. Man kan lage egen skjematype for samtykke, som kun har som oppgave å etterspørre samtykke. Man kan også inkludere samtykkeinnhenting i skjematyper med andre spørsmål som skal besvares for å minimere antall utsendelser.

For å komme i gang må man huke av for "Aktiver samtykkehåndtering" på skjemaversjonen man ønsker forespørsel om samtykke på.

## Ulike krav til samtykkeinnhentelse

Krav til samtykke avhenger av prosjektets innretning og tillatelser/hjemmel for behandling av data.  For eksempel vil behandling i REK omhandle dette. 

I noen tilfeller vil besvarelsen av et skjema anses som godkjent som et samtykke. Man trenger da ikke gjøre noe annet enn å aktivere samtykkehåndtering, men man må informere med tekst et sted at man samtykker ved å besvare skjema.

I noen tilfeller kreves  man aktivt må besvare et spørsmål om man samtykker. Dette løses med å legge til elementet "Samtykkefelt" i skjemabyggeren (dette dukker opp når man aktiverer samtykkehåndtering). Man kan legge til flere "Samtykkefelt", slik at man kan innhente flere ulike samtykker på ett og samme skjema. Videre kan man for eksempel legge på "vis hvis" regler som viser frem spørsmålene kun hvis man velger at man samtykker.

I noen tilfeller kreves ekte elektronisk signatur, da må man krysse av for "Innhent signatur ved ePROM besvarelse". For digital besvarelse må man signere med BankID (medfører en kostnad), for papirskjema vil det komme et felt for signering på slutten av skjemaet. Ved manuell utfyllelse inne i eFORSK har man ingen mulighet for å innhente eller importere signatur. Hvis det er flere samtykkespørsmål inne i skjemaet, signerer man for alle disse i en og samme signatur.

## Innhentede samtykker

Skjemaer med samtykke blir merket i utlistinger. Går man inn på forskningsobjektet vil man også få en oppsummering av alle samtykker for alle dens skjemaer. Merk at oppsummeringen ikke viser samtykket fra skjemaer i kladd.

Skulle et forskningsobjekt levere ett skjema avkrysset "Jeg samtykker ikke", vil skjemaet leveres tilbake til eFORSK med status "Til kontroll". Har man ikke hjemmel til å oppbevare data i disse tilfellene, må skjemaet da slettes.

## Endre samtykke

Hvis et forskningsobjektet ønsker å trekke sitt samtykke, må man slette skjemaet som samtykket er gitt på. 
Har man benyttet seg av samtykkefelter i skjemaet og man har hjemmel til å lagre skjema uten at samtykke foreligger, kan man gjenåpne skjemaet og endre samtykkespørsmålet til "jeg samtykker ikke".

## Trukket samtykke - slette data

Har et forskningsobjekt trukket sitt samtykke må man manuelt slette forskningsobjektet. Dette vil også automatisk slette all tilhørende data på forskningsobjektet. 
