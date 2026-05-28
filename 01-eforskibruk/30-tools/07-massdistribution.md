# Masseutsending 
eFORSK støtter masseutsending ved ePROM‑bestilling av både skjema til utfylling og brevutsending. Funksjonaliteten blir tilgjengelig når man innledningsvis i bestillingsprosessen velger alternativet **masseutsending**. Funksjonen er ment for situasjoner der samme skjematype eller brev skal sendes ut til et stort antall mottakere på samme tid.

## Valg av utsendingstype
Når du har valgt skjematypen eller lastet opp brevet som skal sendes ut, må du velge en av følgende utsendingstyper:
	• Ordinær utsending: Vanlig standardutsending som fungerer som før.
	• Masseutsending (ny funksjonalitet): Benyttes ved utsending til mange mottakere basert på opplastet excel‑fil.

## Opplasting av fil for masseutsending
Dette valget krever opplasting av en excelfil med "ID" i første kolonne etterfulgt av fødselsnumrene til alle mottakerne. Formatet er identisk som ved ordinær utsending basert på mottakere i en excelfil.

## Validering av fil
Etter opplasting av excelfilen må denne valideres. Dette gjøres ved å velge "Valider fil". Dette gir en tilbakemelding på om filformatet er gyldig, antall gyldige fødselsnummer det vil bli sendt ut til, eventuelle duplikater og om det finnes ugyldige fødselsnummer. Dersom filen ikke er gyldig eller inneholder gyldige fødselsnummer kan du ikke gå videre herfra.

## Planlagt utsendingadato
For masseutsending er det krav om å oppgi planlagt utsendingsdato og denne må settes før bestillingen kan fullføres. Tidligste mulige utsendingsdato er neste dag. Utover obligatorisk felt med planlagt utsendingsdato, er fremgangsmåten i dette utsendingssteget lik som ved ordinær ePROM-bestilling.

## Hvordan fungerer det
Når du velger "Bestill masseutsending", blir bestillingene opprettet i bakgrunnen. Du får opp et informasjonsvindu i siste steg og det genereres et varsel i eFORSK. De opprettede bestillingene blir synlige i ePROM- eller brevoversikten og får status "Planlagt" sammen med planlagt utsendingsdato. Når bakgrunnsjobben er ferdig får du varsel om at alle bestillinger er opprettet. 

## Kansellering av planlagte utsendinger
For å kansellere en planlagt masseutsending av ePROM-besitllinger eller brev, søker du opp de aktuelle utsendingene i oversikten og finner utsendinger med status "Planlagt". Når man har filtrert søket slik at resultatet bare viser planlagte utsendinger blir kanselleringsknappen aktiv. Alle utsendingene kan da kanselleres samtidig. Slik er det mulig å stoppe en masseutsending før den faktisk blir sendt ut dersom det er nødvendig. 

## Avgrensninger og køhåndtering
Masseutsendingen av ePROM-bestilling eller brev skjer via bakgrunnsjobber med disse avgrensningene: 
     	* Maks 2000 per time per eFORSK-prosjekt
     	* Maks 3600 totalt på tvers av alle eFORSK-prosjekt per time
     	* Ingen bestillinger blir levert innenfor tidsrommet 22:00-07:00 
     	* Det er ikke garantert at planlagt utsendingsdato blir den faktiske utsendingsdatoen. Ved kø kan enkelte utsendinger bli forsinket og sendt flere dager senere.

Disse begrensningene vil sjelden bli et reelt problem, men bør tas høyde for dersom man planlegger store utsendinger. 
