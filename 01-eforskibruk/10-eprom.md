# ePROM

En skjematype kan bestilles utfylt av personer i Folkeregisteret via det eksterne systemet ePROM.
ePROM ligger åpent på internett og sørger for å tilgjengeliggjøre skjema for alle innbyggere i Norge,
enten digitalt eller via papirskjema sendt i posten. Digital utfylling er tilpasset mobile enheter.

Skjemaet vil bli opprettet i databasen når personen besvarer skjemaet. 

Skjematyper kan også besvares via lenke, hvis skjematypen settes opp for dette. Det trenger da ikke å foreligge en bestilling for å innhente besvarelser, det er nok å distribuere lenken. Alle ePROM-bestillinger styres fra "ePROM-fanen" i eFORSK.

## Følgebrev

Følgebrevet vil være det første skjemamottaker ser. Teksten bør inneholde informasjon om hvorfor mottaker har fått skjemaet, samt hva dataene som samles inn skal brukes til. Her er det også mulig å gi spesifikke instrukser til utfyllingen dersom det er nødvendig. Dersom man benytter seg av papirutsending, har følgebrevet en lengdebegrensning på ca 1.5 A4 side.

Det anbefales å plassere all informasjonstekst i følgebrevet. Dette for å unngå at store tekstmengder plasseres i felt i skjemabyggeren, i mellom eller i tilknytning til spørsmål i skjemaet. Dette kan føre til forskyvninger eller "hopp" til bunnen av skjemaet, mens bruker fyller ut skjemaet. Følgebrevet kan redigeres under Administrasjon - Skjematyper - velg aktuelle skjematype - ePROM-oppsett. 

## Varslingskanaler

Ved bestilling av skjemautfyllelse bestemmer man om man vil varsle mottaker selv eller om ePROM skal sende ut varsel.
Velger man å varsle mottaker selv er man selv ansvarlig for at dette gjøres på et lovlig vis uten å eksponere sensitive data om mottaker. Velger man å sende varsel til mottaker vil systemene sørge for å varsle på en trygg måte, så lenge man har satt opp avsendernavn og tekster på riktig måte.

Ved bestilling av skjemautfyllelse må man legge inn utløpsdato for denne. 

### Jeg vil varsle mottaker selv

Her vil man få en kode som man sammen med fødselsdatoen til mottaker kan bruke for å logge seg på og besvare skjemaet, gjennom en nettadresse som oppgis i skjemabestillingen. Denne koden må man selv distribuere til mottaker.
Dette valget får man ikke på samtykkeskjema der man skal innhente signatur ved ePROM-besvarelse, for her kreves det at mottaker identifiserer seg med BankID.

### Send varsel til mottaker

Mottaker kan forsøkes nås på følgende kanaler i prioritert rekkefølge via ePROM:

#### 1. Helsenorge

Dersom studiedeltaker har registrert seg på Helsenorge med samtykke er dette den høyest prioriterte kanalen, da denne er sikker og ikke medfører kostnader. 
I Helsenorge kan mottaker ha satt opp varsling på SMS, e-post eller bli varslet via app (push) når det kommer en melding. Med andre ord varsles studiedeltaker i henhold til sin varselprofil. Studiedeltakere får påminnelse om skjemaoppgaver som er mottatt men ikke utført: 
    
* 5 dager før frist dersom det er mer enn 10 dager fra mottak av skjemaoppgave til fristen går ut
* 1 dag før fristen for oppgaven går ut

Mottaker av en skjemaoppgave har imidlertid mulighet til å skru av og på påminnelsesfunksjonen for hver enkelt skjemaoppgave.

Ved utsending til studiedeltakere som er barn via Helsenorge, skal man alltid sende til barnet, ikke til deres foresatte. Dette gjelder også når det er representant med foreldreansvar eller fullmakt som forventes å håndtere henvendelsen.

#### 2. Sikker digital postkasse

Dette er også en sikker kanal, og består av tjenestene Digipost og E-box. Hvis mottaker har registrert seg på noen av disse vil dette brukes som varslingskanal.
I sikker digital postkasse kan mottaker ha satt opp varsling på SMS eller e-post når det kommer en melding. Bruk av denne kanalen medfører kostnader.

#### 3. Papirskjema i posten

For å kunne bruke denne kanalen må man ha aktivert papirskjema ved skjemabygging.
Denne kanalen er prioritert nederst da det er den mest kostbare måten å nå mottaker på.
Sist kjente bosted i personregisteret brukes som adresse.

For varslingskanaler 1 og 2 gjelder at mottaker må logge inn med sikkerhetsnivå 4, det vil si BankID eller tilsvarende, for å besvare skjema.

#### Mottakere under 18 år

For å nå studiedeltakere under 18 år kan man varsle mottaker selv (se neste avsnitt), sende direkte til forskningsdeltakeren via Helsenorge eller opprette et relasjonsskjema som blir sendt til en relasjon av studiedeltaker (se lenger nede). For studiedeltakere yngre enn 18 år kan skjema distribueres og besvares via Helsenorge, så lenge samtykke til det er gitt i Helsenorge og det er i tråd med deres <a href="https://helsenorge.atlassian.net/wiki/spaces/HELSENORGE/pages/2520481794/Representasjon+p+Helsenorge" target="_blank">representasjonsreglement</a> 

## Send skjema til relasjon av mottaker

For å kunne sende skjema til en relasjon av mottaker må man ha aktivert denne funksjonaliteten ved opprettelse av database (spesifisert i vedlegg til DBA). Ved tilfeller hvor man vil utføre en skjemabestilling til et forskningsobjekt som ikke kan nås via vanlige kanaler, kan man velge å sende skjema til en relasjon av forskningsobjektet, som kan fylle ut skjema på vegne av forskningsobjektet. Et typisk scenario vil være skjemautsending til forskningsobjekter som er under 16 år, hvor skjema kan fylles ut av foresatte eller verger.

For å utføre utsending til relasjon av forskningsobjekter, må det først opprettes et relasjonsskjema for de aktuelle forskningsobjektene (Les mer om relasjonsskjematyper under _Skjemautforming, felter og regler_). 

Når man velger å sende skjema til relasjon av forskningsobjektet (gjøres i oppsettet ved skjemabestilling), vil det vises en liste over alle relasjonsskjematyper som eksisterer, og man må velge den relasjonsskjematypen som er aktuell for bestillingen. Ved tilfeller hvor relasjonsskjematypen består av flere enn ett **personvelgerfelt**, vil det første aktuelle feltet bli valgt for å finne relasjonen det skal bestilles til. Merk at man ikke kan bruke Helsenorge som utsendingskanal ved relasjonsskjemaer.


## Status på bestillinger

En bestilling kan ha følge statuser:

**Planlagt:** En bestilling vil skje frem i tid. Tidligste tidspunkt for bestilling er gitt under "bestillingstidspunkt". De planlagte bestillingene blir kjørt ca hver hele time. Har man mer enn 1 000 bestillinger med passert planlagt bestillingstidspunkt, blir kun 1 000 av disse bestilt hver kommende time frem til alle er bestilt.

**Bestiller:** En bestilling er levert til ePROM systemet, og det ventes på en tilbakemelding om hvilken varslingskanal bestillingen sendes på. Det kan ta opptil 48 timer å få svar. 

**Bestilt:** Bestillingen er sendt ut, og det ventes på svar.

**Besvart:** Et svar har ankommet eFORSK.

**Utløpt:** Bestilling er ikke besvart innen utløpsfristen. For påstartede besvarelser via lenke som ikke blir fullført, vil det dukke opp en bestilling med denne statusen i eFORSK to dager etterpå.
Merk at en ubesvart papirskjemabestilling aldri løper ut på dato, svaret kan komme inn når som helst frem i tid.

**Feilet:** Se mer spesifikk feilmelding ved siden av statusen.

**Avbrutt:** Bestillingen har hatt status "planlagt", men den har blitt avbrutt før den har blitt forsøkt bestilt.

**Ukjent:** Bestillingen har ukjent status

## Testutsending

Man kan teste bestilling av skjemautfyllelse i testmodus. Helsenorge-aktive testpersoner man kan bestille utfyllelse til kan man finne <a href="https://eforskbrukermanual.azurewebsites.net/#testmode" target="_blank">her</a>. 

Utsendelse av papirskjema er naturligvis vanskelig å teste. Her vil man i testmodus etter en stund få et tilfeldig generert svar tilbake. Laster man ned den skannede PDF-fila i testmodus, vil denne ikke være utfylt.

## Kopi til studiedeltaker

Dersom skjema besvares via Helsenorge, vil studiedeltaker motta kopi av skjemabesvarelsen på Helsenorge. For skjema som er besvart via sikker digital postkasse gjelder det samme, da vil pasienten motta en kopi i sin sikre digitale postkasse. Kopi av skjema blir med andre ord sendt til samme kanal der skjema er besvart. 

Imidlertid; for skjema som krever signatur gjelder *i tillegg* at kopi av signerte skjema blir sendt til sikker digital postkasse. Det vil si at signerte skjema som blir besvart via lenke vil bli sendt til studiedeltakers digitale postkasse. 

Dersom skjema besvares med engangskode blir det aldri sendt kopi til studiedeltaker.

## Papirskjema (fysisk post)

Papirskjema blir tolket av en skanner hos ekstern leverandør, det er viktig å sammenligne den innskannede PDFen med de tolkede svarene i skjemaet at det faktisk er tolket riktig. Skanneren tolker alt annet enn avkryssning veldig dårlig. Skjema kan gjenåpnes og rettes i eFORSK i etterkant.

Veiledning for besvarelse av papirskjema:
*	Ikke returner forsiden
*	Bruk blå penn, ikke rød penn
*	Sett tydelige kryss
*	Hvis du har krysset av feil, skraver feltet og sett et nytt kryss på riktig sted
*	Skjemaet tolkes automatisk, håndskrevne tekster og vedlagte lapper blir ikke tatt hensyn til
*	Vi setter pris på om du leverer alle arkene riktig orientert

Papirskjema vil alltid komme tilbake til eFORSK med status "Til kontroll".

## Masseutsending
eFORSK støtter masseutsending ved ePROM‑bestilling av både skjema til utfylling og brevutsending. Funksjonaliteten blir tilgjengelig når man innledningsvis i bestillingsprosessen velger alternativet **masseutsending**. Funksjonen er ment for situasjoner der samme skjematype eller brev skal sendes ut til et stort antall mottakere på samme tid (flere enn 500).

### Valg av utsendingstype
Når du har valgt skjematypen eller lastet opp brevet som skal sendes ut, må du velge en av følgende utsendingstyper:
* **Ordinær utsending:** Standardutsending tilpasset under 500 studiedeltakere. 
* **Masseutsending:** Benyttes ved utsending til flere enn 500 studiedeltakere. 

Neste valg, **Opplasting av fil for masseutsending,** krever opplasting av en excelfil med "ID" i første kolonne, etterfulgt av fødselsnumrene til mottakerne. Formatet er identisk ved både ordinær og masseutsending. Etter opplasting av excelfilen valideres denne. Dette gjøres ved å velge **"Valider fil"**. Dette gir en tilbakemelding på om filformatet er gyldig, antall gyldige fødselsnummer det vil bli sendt ut til, eventuelle duplikater og om det finnes ugyldige fødselsnummer. Dersom filen ikke er gyldig eller inneholder gyldige fødselsnummer kan du ikke gå videre herfra.

For masseutsending er det krav om å oppgi **planlagt utsendingsdato** og denne må settes før bestillingen kan fullføres. Tidligste mulige utsendingsdato er neste dag. Utover obligatorisk felt med planlagt utsendingsdato, er fremgangsmåten i dette utsendingssteget lik som ved ordinær ePROM-bestilling.

### Hvordan fungerer det
Når du velger "Bestill masseutsending", blir bestillingene opprettet i bakgrunnen. Du får opp et informasjonsvindu i siste steg og det genereres et varsel i eFORSK. De opprettede bestillingene blir synlige i ePROM- eller brevoversikten og får status "Planlagt" sammen med planlagt utsendingsdato. Når bakgrunnsjobben er ferdig får du varsel om at alle bestillinger er opprettet. 

### Kansellering av planlagte utsendinger
For å kansellere en planlagt masseutsending av ePROM-bestillinger eller brev, søker du opp de aktuelle utsendingene i oversikten og huker av utsendinger med status "Planlagt". Når man har filtrert søket slik at resultatet bare viser planlagte utsendinger blir kanselleringsknappen aktiv. Alle utsendingene kan da kanselleres samtidig. Slik er det mulig å stoppe en masseutsending før den faktisk blir sendt ut dersom det er nødvendig. 

### Avgrensninger og køhåndtering ved masseutsending
Masseutsendingen av ePROM-bestilling eller brev skjer via bakgrunnsjobber med disse avgrensningene: 
* Maks 2000 per time per eFORSK-prosjekt
* Maks 3600 totalt på tvers av alle eFORSK-prosjekt per time
* Ingen bestillinger blir levert innenfor tidsrommet 22:00-07:00
* Det er ikke garantert at planlagt utsendingsdato blir den faktiske utsendingsdatoen. Ved kø kan enkelte utsendinger bli forsinket og sendt flere dager senere.

Disse begrensningene vil sjelden bli et reelt problem, men bør tas høyde for dersom man planlegger store utsendinger. 

## Kostnader ved bruk av ePROM

Informasjon om kostnader finnes i ePROM sin egen dokumentasjon: <a href="https://eprom.hemit.org/kostnader" target="_blank">ePROM-kostnader</a>.


