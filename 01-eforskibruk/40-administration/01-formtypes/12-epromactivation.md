# ePROM aktivering

Aktiverer man ePROM vil det i øyeblikket skjemaet publiseres bli kopiert til den eksterne ePROM-løsningen.
I testmodus kan man umiddelbart bestille ePROM av skjematypen, mens utenfor testmodus må det godkjennes 
av eFORSK fagansvarlig før det kan bestilles. Superbruker tar kontakt med fagansvarlig (eforsk@hemit.no) når et skjema er ferdig testet og skal godkjennes.

## Vis hovedgrupper som egne skjema i ePROM

Ved å aktivere "Vis hovedgrupper som egne skjema i ePROM" vil hele eFORSK-skjemaet samles til et samleskjema i ePROM, hvor hver hovedgruppe i skjemabyggeren blir et eget ePROM-skjema i samleskjemaet. Dette vil også reflekteres i forhåndsvisningen av ePROM-skjema i eFORSK. 

Dette er et standardvalg som automatisk aktiveres for nye skjema hvis ePROM aktiveres. NB: Aktivering av dette fører også med seg at regler ikke kan peke til felter fra andre hovedgrupper i en ePROM-utsending. Skjemabyggeren i eFORSK varsler om slike tilfeller gjennom valideringssystemet. 

Eksisterende skjema må oppfylle krav om at det bare er hovedgrupper og ikke enkeltfelter på toppnivå i skjemaet for at dette kan aktiveres.

For skjema som inneholder standardskjema (f.eks. EQ5D) er denne funksjonen alltid aktivert og kan ikke deaktiveres med mindre man fjerner standardskjemaet.

## ePROM oppsett

### Utfylling via lenke

Huker man av for utfylling via lenke vil man få en lenke som kan distribueres til forskningsobjekter man ønsker skal besvare skjemaet.
Her trenger det altså ikke å foreligge bestilling fra eFORSK for å få inn svar. Merk at det vil være en lenke for testmodus og en lenke for ikke-testmodus. Det er viktig å distribuere riktig lenke.

Selv om man har aktivert denne funksjonen kan man likevel bestille skjemautfyllelse på vanlig måte i eFORSK. Funksjonene kan kombineres som man vil.

Husk at det ved distribusjon av lenken ikke må avsløres mottakers sykdommer, helsetilstand eller lignende sensitive data. Sender man for eksempel lenken på e-post (ikke godkjent kanal for sensitive data), må informasjonen være veldig generell. Man kan for eksempel ikke skrive "Vi ønsker å inkludere deg i vår studie fordi du har diabetes type 2", men man kan formulere det slik: "Kjenner du noen som har diabetes type 2? Vi leter etter deltakere til en studie om dette.".

### Papirskjema

Skal man støtte papirutsendelse av skjemaet må det aktivt velges, da dette medfører kostnader for etablering, utsendelse og innskanning. Her må prosjektleder fra Hemit involveres, superbruker tar kontakt med fagansvarlig (eforsk@hemit.no) for å komme i gang. Prosessen med å få klargjort papirskjemaet vil ta flere uker. Digital utsendelse kan likevel godkjennes og tas i bruk i påvente av at papirskjemaet klargjøres.

Skanning og tolkning av svar skjer hos ekstern leverandør, og her tolkes alt annet enn kryss dårlig. Det vil si at felter med tall og tekst må manuelt sjekkes opp og korrigeres inne i eFORSK etter at svaret er mottatt. Derfor er det ikke anbefalt å aktivere papirskjema på annet enn skjemaer som kun inneholder valgfelt og avkrysningsfelt hvis det forventes mange svar, da det krever etterarbeid å gå igjennom disse. 

Det anbefales å legges inn informasjonstekst i starten av skjemaet med utfyllingsveilder for papir (legg på regel "vis kun på papirskjema"). Dette bør være med:
* Ikke returner forsiden
* Bruk blå penn, ikke rød penn
* Sett tydelige kryss
* Hvis du har krysset av feil, skraver feltet og sett et nytt kryss på riktig sted
* Skjemaet tolkes automatisk, håndskrevne tekster og vedlagte lapper blir ikke tatt hensyn til
* Vi setter pris på om du leverer alle arkene riktig orientert


### Informasjonstekst til mottaker og avsendernavn

Når skjema skal fylles ut av mottaker i ePROM møter man en tekst som bør forklare hvorfor man har mottatt skjemaet
og hva dataene skal brukes til. Dette spesifiseres i "informasjonstekst til mottaker". Videre kan man spesifisere hvem 
som forespør disse dataene i avsendernavnet.

I informasjonsteksten kan man sende med verdier fra systemutfylte felter som blir beregnet ved skjemaopprettelse, eksempelvis alder. Hvis variabelnavnet er "Alder", skrives følgende kode i teksten for å få verdien:  [\_ALDER\_]  (med store bokstaver). Man kan også bruke verdier fra foreldreskjemaet, eksempelvis hvis det er et felt som heter "Sykehusnavn": [\_FORELDRESKJEMA\_SYKEHUSNAVN\_]. Hvis det ikke velges et eksisterende foreldreskjema ved bestilling, blir kodene blanket ut i teksten. For valgfelt og avkrysningsfelt vil man få tallverdier ved å bruke variabelnavnet direkte, men ved å legge på "\_txt" kan man få den tekstlige verdien: [\_KJOENN\_TXT\_].

Merk at disse ikke erstattes med verdier i forhåndsvisning, men først når man legger inn en bestilling.
