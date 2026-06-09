# ePROM

En skjematype kan bestilles utfylt av personer i Folkeregisteret via det eksterne systemet ePROM. ePROM ligger åpent på internett og sørger for å tilgjengeliggjøre skjema for alle innbyggere i Norge, enten digitalt eller via papirskjema sendt i posten. Digital utfylling er tilpasset mobile enheter. Løsningen legger til rette for enkel masseutsending av skjematype og brev til inntil 500 000 studiedeltakere (se **Masseutsending** lenger nede).

Skjemaet vil bli opprettet i databasen når personen besvarer skjemaet. 

Skjematyper kan også besvares via lenke, hvis skjematypen settes opp for dette. Det trenger da ikke å foreligge en bestilling for å innhente besvarelser, det er nok å distribuere lenken. Alle ePROM-bestillinger styres fra "ePROM-fanen" i eFORSK.



## Send skjema til relasjon av mottaker

For å kunne sende skjema til en relasjon av mottaker må man ha aktivert denne funksjonaliteten ved opprettelse av database (spesifisert i vedlegg til DBA). Ved tilfeller hvor man vil utføre en skjemabestilling til et forskningsobjekt som ikke kan nås via vanlige kanaler, kan man velge å sende skjema til en relasjon av forskningsobjektet, som kan fylle ut skjema på vegne av forskningsobjektet. Et typisk scenario vil være skjemautsending til forskningsobjekter som er under 16 år, hvor skjema kan fylles ut av foresatte eller verger.

For å utføre utsending til relasjon av forskningsobjekter, må det først opprettes et relasjonsskjema for de aktuelle forskningsobjektene (Les mer om relasjonsskjematyper under _Skjemautforming, felter og regler_). 

Når man velger å sende skjema til relasjon av forskningsobjektet (gjøres i oppsettet ved skjemabestilling), vil det vises en liste over alle relasjonsskjematyper som eksisterer, og man må velge den relasjonsskjematypen som er aktuell for bestillingen. Ved tilfeller hvor relasjonsskjematypen består av flere enn ett **personvelgerfelt**, vil det første aktuelle feltet bli valgt for å finne relasjonen det skal bestilles til. Merk at man ikke kan bruke Helsenorge som utsendingskanal ved relasjonsskjemaer.


## Les mer om:

- [Kostnader ved bruk av ePROM](./01-costs.md)
- [Følgebrev](./02-coverletter.md)
- [Varslingskanaler](./03-notificationchannel.md)
- [Testutsending](./04-testdistribution.md)
- [Status på ePROM-bestillinger](./05-status.md)
- [Kopi til studiedeltaker](./06-copy.md)
- [Masseutsending](./07-bulkdistribution.md)
- [Papirskjema](./08-paperform.md)
- [Send skjema til relasjon](./09-relation.md)
