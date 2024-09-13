# Skjemautforming, felter og regler

Under bygging av skjematyper skal man legge til elementer. Dette kan være grupper, informasjonstekst, felter eller regler.

Som nevnt er det viktig å tenke på utforming av skjema før man begynner å bygge. Oppdeling av skjema eller gjenbruk av deler av et skjema som blir repeterende er ting å ta hensyn til, da skjemabygger **ikke** skalerer ubegrenselig i skjemastørrelse. Ved for store/komplekse skjema (mtp. felter/regler) kan det oppstå ytelsesproblemer som brukere vil merke, da er det anbefalt med oppdeling i flere mindre skjema for å unngå dette. Derfor er det viktig å ta hensyn til dette på forhånd med å planlegge skjemaform og størrelse. Oppdeling og gjenbruk står det mer relevant informasjon om i **Hovedskjematype og underskjematype** og **Kopi av eksisterende skjematype**.
                    
## Grupper
Grupper brukes for å samle elementer. Gruppen vil få en overskrift som vil utheves i skjemaet. "Vis hvis" regler kan legges på grupper for å styre visning av alle dens elementer.

For å forbedre kapasitet og unngå ytelsesproblemer i skjemabygger, vil visning av grupper på toppnivå i skjemabygger være begrenset når man bygger skjema. Bare **én** gruppe på toppnivå i skjemabygger vil kunne være åpen om gangen. Denne begrensningen vil ikke eksistere utenfor skjemabygger, og merkes ikke i skjema som skal fylles ut.

## Informasjonstekst
Informasjonstekst kan legges til hvor man ønsker i skjemaet, eksempelvis for en ekstra forklaring til den som skal fylle ut skjemaet.
                    
## Felter
Feltene er det som skal besvares i et skjema. Felttypene som støttes er **tallfelt**, **avkrysningsfelt**, **datofelt**, **tekstfelt**, **valgfelt**, **randomiseringsfelt**, **samtykkefelt** og **personvelgerfelt**. 

Det finnes ikke en egen felttype for **flervalgsfelt**, da analyse av eksportert data blir vanskelig om et svar på en variabel inneholder flere verdier. Men, man kan lage illusjonen av et flervalgsfelt ved å ha en gruppe med avkrysningsfelt for hvert alternativ. På gruppen legger man på regelen "Vis som flervalgsfelt", som gjør at den vises som ett felt.

I noen tilfeller ønsker man å samle inn **fødselsnummeret** til andre enn selve forskningsobjektet, eksempel for pårørende. Her må man bruke **tekstfelt**, da et **tallfelt** ikke holder store nok tall for personnummer i tillegg til at fødselssnummer som starter med 0 ikke bevares i et tall. Husk at man skal huke av for at **"Feltet inneholder personopplysninger"**. **personvelger**-feltet kan også brukes for å hente fødselsnummer, men det er bare tilgjengelig ved direkte skjemautfylling i eFORS, ikke ved skjemabestilling til mottakere.

### Variabelnavn og eksport
Alle felt vil ha et variabelnavn som brukes ved eksport, og en visningstekst som gjør det enkelt for bruker å vite hva som skal fylles ut.

For eksport av data som skal videre skal importeres til Stata eller SPSS, er det viktig å merke seg at Stata har en maks lengde på variabelnavn på 32 karakter, mens SPSS har maks lengde på 64 karakter. Derfor er det viktig å holde variabelnavnene kortere enn 32/64 karakterer hvis dataen skal importeres videre til noen av disse formatene.

### Systemutfylte felt
Et systemutfylt felt vil automatisk fylles ut ved opprettelse, endring eller ferdigstillelse. Les mer i egen artikkel.

### Personvelgerfelt
Et **personvelgerfelt** er et felt som bare vil være aktivt og mulig å bruke i utfylling av skjema direkte inne i eFORSK. Ved skjemabestilling til mottakeren vil personvelgerfelt deaktiveres og ikke være synlig for mottakere.
Personvelgerfelt gir skjemautfyller i eFORSK muligheten til å søke opp en person (på samme måte som man søker opp personer fra personregisteret i forskningsobjektssøk), og velge en person som verdi til feltet. 

Et personvelgerfelt vil inneholde fødselssnummeret til den valgte personen som verdi, som er den verdien man får ved å eksportere skjemadataen, og den verdien feltet skal inneholde ved evt. dataimport til personvelgerfelt.

Personvelgerfelt kan brukes fritt ved bygging av skjema og utfylling av skjema, men hovedbruken til **personvelgerfelt** er for å opprette skjematyper som kan brukes som **relasjonsskjematyper**. 
**Relasjonsskjematyper** defineres som skjematyper som inneholder ett (eller flere) **personvelgerfelt**, og kan brukes til å utføre skjemabestillinger i ePROM til relasjoner av forskningsobjekt, **på vegne av** forskningsobjektet.
Les mer om **på vegne av**-funksjonalit og prosessen under **ePROM**-delen.

### Randomiseringsfelt
Et randomiseringsfelt kan settes opp til å utføres på tre måter;
1. Manuelt ved klikk på knapp i skjema
2. Automatisk ved skjemaopprettelse
3. Automatisk ved første ferdigstillelse

I de tilfellene et randomiseringsfelt er lagt til en skjematype som kan bestilles utfylt (ePROM), så vil ikke feltet være synlig for vedkommende som skal fylle ut. Ved valgt utførelse 1 eller 2 vil feltet vil bli randomisert ved bestillingstidspunktet, det vil si at randomiseringen er utført uansett om skjemaet blir besvart eller ei.

For stratifisert blokkrandomisering er utførelse 3 anbefalt, da felter med data for stratifiseringskategoriene må være besvart. Merk at besvarelser kan endres etter at randomisering er kjørt, og at man da kan havne i feil stratifiseringsgruppe i forhold til utført randomisering. Randomiseringen utføres kun en gang og blir ikke oppdatert.

En opprettet randomisering kan brukes på tvers av felter og skjematyper. Unntaket her er stratifisert blokkrandomisering, som kun kan brukes innad skjematypen den er opprettet på.

Les mer om randomisering under "Administrasjon" i brukermanualen.

## Skjemaregler
Skjemaregler omfavner både validerings- og vis/skjul-regler. Reglene kan på lik linje med felter opprettes på en versjon, og fjernes i senere versjoner.

Man kan teste reglene i forhåndsvisning av skjematypen under bygging.

