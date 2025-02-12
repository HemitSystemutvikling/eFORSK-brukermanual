# Hendelsesovervåking

Dette er et system for å overvåke hendelser i eFORSK og varsle om dette.

## Typer overvåking

Når man lager en ny hendelsesovervåking må man velge hvilken type objekter og hvilke skjematype man vil overvåke. 
Man kan overvåke hendelser fra følgende objekter:

#### Skjema

For skjema kan man velge hvilke skjemastatus og hvilke verdier skjemaet skal ha for å utløse en hendelse.

Eksempel 1: Skjema har status "til kontroll".

Eksempel 2: Ferdigstilt skjema med forskningsobjektets kjønn lik mann og forskningsobjektets alder over 90 år.

Eksempel 3: Forskningsobjektet avgår med døden. (Man må her overvåke at en skjematype med det systemutfylte feltet "forskningsobjektets dødsdato" blir besvart)


#### ePROM-bestillinger

For ePROM-bestillinger kan man velge hvilken status og hvilken varslingskanal bestillingen skal ha for å utløse en hendelse.

Eksempel 1: Bestilling oppnår status "utgått".

Eksempel 2: Bestilling sendt som fysisk post oppnår status "besvart".

## Hendelse

Hendelser dukker opp under "Verktøy" i eFORSK. Dette kan leses om tilsvarende sted i brukermanualen. Hendelser kan kun sees av databaseansvarlige, dataansvarlige og registrarer.

## Varsling

Utover hendelsesvisningen kan man opprette varsling når en hendelse oppstår. Varsling kan gjøres via:
* Varslinger i eFORSK (brukeren får beskjed når man jobber inne i eFORSK)
* E-post*
* SMS*

Man kan velge at brukeren som opprettet objektet blir varslet. 
Ellers kan også velge blant brukerne som har vært pålogget databasen.
I tillegg kan man legge til e-postadresser og telefonnumre som skal varsles.

Det "beskrivende navnet" som oppgis ved opprettelse av overvåkingen brukes i varselet som sendes ut.

Velger man varsling for hver hendelse, vil dette gjøres ca ett minutt etter at hendelses har skjedd. 
Velger man varsling oppsummert daglig, vil denne gå ut ca kl 7 hver dag hvis det har vært hendelser siden forrige varsling. 
Velger man varsling oppsummert ukentlig, vil denne gå ut ca kl 7 hver mandag hvis det har vært hendelser siden forrige varsling.

\* Merk at E-post og SMS utsendelse ikke fungerer i demonstrasjonsdatabaser.

## Begrensninger

Hendelsesovervåking skjer kun på fremtidige hendelser etter at den er opprettet, den sjekker ikke om hendelsen har skjedd blant eksisterende data før disse eventuelt oppdateres.

En hendelsesovervåking kan varsle en gang per objekt som utløser en hendelse. Eksempelvis, hvis man overvåker skjema som får status "til kontroll", vil hendelsesovervåkingen kun varsle første gangen skjemaet får status "til kontroll", men ikke de påfølgende gangene.

Overvåkingen har en forsinkelse på ca ett minutt før den sjekker et oppdatert objekt. Objektet kan i ett øyeblikk oppfylle reglene for en hendelse, men bli endret til å ikke oppfylle reglene før overvåkingen rekker å rapportere hendelsen.

Overvåking av forskningsobjektets død har en forsinkelse fra personregisteret, og vil videre kun sjekkes nattlig i eFORSK.


