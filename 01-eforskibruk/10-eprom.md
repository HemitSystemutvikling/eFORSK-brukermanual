# ePROM

En skjematype kan bestilles utfylt av personer i Personregisteret via det eksterne systemet ePROM.
ePROM ligger åpent på internett og sørger for å tilgjengeliggjøre skjema for alle innbyggere i Norge,
enten digitalt eller via papirskjema sendt i posten. Digital utfylling er tilpasset mobile enheter.

Skjemaet vil bli opprettet i databasen når personen besvarer skjemaet. 

Skjemaer kan også besvares via lenke, hvis skjematypen settes opp for dette. Det trenger da ikke å foreligge en bestilling for å innhente besvarelser, det er nok å distribuere lenken.

## Varslingskanaler

Ved bestilling av skjemautfyllelse bestemmer man om man vil varsle mottaker selv eller om ePROM skal sende ut varsel.
Velger man å varsle mottaker selv er man selv ansvarlig for at dette gjøres på et lovlig vis uten å eksponere sensitive data om mottaker. Velger man å sende varsel til mottaker vil systemene sørge for å varsle på en trygg måte, så lenge man har satt opp avsendernavn og tekster på riktig måte.

### Jeg vil varsle mottaker selv

Her vil man få en kode som man sammen med fødselsdatoen til mottaker kan bruke for å logge seg på og besvare skjemaet, gjennom en nettadresse som oppgis i skjemabestillingen. Denne koden må man selv distribuere til mottaker.
Dette valget får man ikke på samtykkeskjema der man skal innhente signatur ved ePROM besvarelse, for her kreves det at mottaker identifiserer seg med BankID.

#### Mottakere under 16 år

For mottakere under 16 år er dette per nå eneste mulighet for at enten mottaker eller noen på vegne av mottaker kan fylle ut skjema. De andre alternativene for utsending av varsel til mottaker listet nedenfor kan ikke brukes for mottakere under 16 år. For mottaker mellom 16 og 18 år kan skjema besvares på helsenorge, så lenge mottaker har gitt samtykke.

### Send varsel til mottaker

Mottaker kan forsøkes nås på følgende kanaler i prioritert rekkefølge via ePROM:

#### 1. Helsenorge

Hvis mottaker har registrert seg på Helsenorge med samtykke er dette den høyest prioriterte kanalen, da denne er sikker og ikke medfører kostnader. 
I Helsenorge kan mottaker ha satt opp varsling på SMS eller e-post når det kommer en melding.

#### 2. Sikker digital postkasse

Dette er også en sikker kanal, og består av tjenestene Digipost og E-box. Hvis mottaker har registrert seg på noen av disse vil dette brukes som varslingskanal.
I sikker digital postkasse kan mottaker ha satt opp varsling på SMS eller e-post når det kommer en melding. Bruk av denne kanalen medfører kostnader.

#### 3. E-post

Denne kanalen kan nyttes hvis mottaker har en e-postadresse oppført i kontaktregistret (difi).
E-post er en usikret kanal, og informasjonen som sendes hit er veldig begrenset. Den er prioritert over SMS da det er mulighet for mer tekst i en e-post. 
Les mer om hvordan e-post er utformet: <a href="https://eprom.hemit.org/PasientskjemaViaEpostSms" target="_blank">ePROM dokumentasjon</a>.

#### 4. SMS

Denne kanalen kan nyttes hvis mottaker har et telefonnummer oppført i kontaktregistret (difi).
SMS er som e-post en usikret kanal, og hit sendes det en veldig kort tekst.
Les mer om hvordan SMSen er utformet: <a href="https://eprom.hemit.org/PasientskjemaViaEpostSms" target="_blank">ePROM dokumentasjon</a>.

#### 5. Papirskjema i posten

For å kunne bruke denne kanalen må man ha aktivert papirskjema ved skjemabygging.
Denne kanalen er prioritert nederst da det er den mest kostbare måten å nå mottaker på.
Sist kjente bosted i personregisteret brukes som adresse.

For varslingskanaler 1-4 gjelder at mottaker må logge inn med sikkerhetsnivå 4, dvs BankID eller tilsvarende, for å besvare skjema.

## Status på bestillinger

En bestilling kan ha følge statuser:

#### Planlagt
En bestilling vil skje frem i tid. Tidligste tidspunkt for bestilling er gitt under "bestillingstidspunkt". De planlagte bestillingene blir kjørt ca hver hele time. Har man mer enn 1 000 bestillinger med passert planlagt bestillingstidspunkt, blir kun 1 000 av disse bestilt hver kommende time frem til alle er bestilt.

#### Bestiller
En bestilling er levert til ePROM systemet, og det ventes på en tilbakemelding om hvilken varslingskanal bestillingen sendes på. Det kan ta opptil 48 timer å få svar. 

#### Bestilt
Bestillingen er sendt ut, og det ventes på svar.

#### Besvart
Et svar har ankommet eFORSK.

#### Utløpt
Bestilling er ikke besvart innen utløpsfristen. 
For påstartede besvarelser via lenke som ikke blir fullført, vil det dukke opp en bestilling med denne statusen i eFORSK to dager etterpå.
Merk at en ubesvart papirskjemabestilling aldri løper ut på dato, svaret kan komme inn når som helst frem i tid.

#### Feilet
Se mer spesifikk feilmelding ved siden av statusen.

#### Avbrutt
Bestillingen har hatt status "planlagt", men den har blitt avbrutt før den har blitt forsøkt bestilt.

#### Ukjent
Bestillingen har ukjent status

## Kopi til pasient

Dersom skjema besvares via helsenorge, vil pasienten motta kopi av skjemabesvarelsen på helsenorge. For skjema som er besvart via sikker digital postkasse gjelder det samme, da vil pasienten motta en kopi i sin sikre digitale postkasse. Kopi av skjema blir med andre ord sendt til samme kanal der skjema er besvart. For andre kanaler blir det i utgangspunktet ikke sendt kopi til pasienten, med mulighet for endring i fremtidige versjoner av eFORSK. 

Imidlertid; for skjema som krever signatur gjelder *i tillegg* at kopi av signerte skjema blir sendt til sikker digital postkasse. Det vil si at signerte skjema som blir besvart via lenke eller epost/sms vil bli sendt til pasientens digitale postkasse. 

Dersom skjema besvares med engangskode blir det aldri sendt kopi til pasienten.

## Testmodus

Man kan teste bestilling av skjemautfyllelse i testmodus. Testpersoner man kan bestille utfyllelse av kan man finne under egen artikkel om testmodus i brukermanualen. Her er det spesielle testpersoner som har fått satt opp konto på helsenorge.no.

Utsendelse av papirskjema er naturligvis vanskelig å teste. Her vil man i testmodus etter en stund få et tilfeldig generert svar tilbake. Laster man ned den skannede PDF-fila i testmodus, vil denne ikke være utfylt.

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

## Kostnader

Informasjon om kostnader finnes i ePROM sin egen dokumentasjon: <a href="https://eprom.hemit.org/kostnader" target="_blank">eprom.hemit.org/kostnader</a>.
