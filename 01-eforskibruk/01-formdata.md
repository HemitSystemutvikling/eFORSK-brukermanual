# Skjema

Et skjema er en utfyllelse/besvarelse av en skjematype. Et skjema tilhører ett forskningsobjekt. Skjemaer kan opprettes og fylles ut i eFORSK, eller det kan bestilles utfylt via ePROM-løsningen hvis man har dette aktivert.

## Skjemastatus

* **Kladd** (0) - Grunntilstand når et nytt skjema blir opprettet. Dette er den eneste statusen hvor skjemadata kan endres. 
* **Til kontroll** (2) - Det er to scenarier for denne statusen: 1. Bruker med rollen *databaseansvarlig*, *dataansvarlig* eller *monitor* kan returnere skjema til kontroll av skjemaeier sammen med en årsakstekst. 2. Ved bestilling av skjemautfyllelse (ePROM), kan ePROM sende advarsler om mulige feil i skjemadata på svarskjema og skjemaet får dermed statusen "Til kontroll". For papirskjema må signert samtykke manuelt kontrolleres. Et skjema til kontroll må gjenåpnes før det kan redigeres og ferdigstilles på nytt. 
* **Ferdigstilt** (1) - Et ferdigstilt skjema kan ikke endres, men kan gjenåpnes til kladd eller sendes til kontroll. 
* **Slettet** (9) - Et slettet skjema vil ikke lenger være tilgjengelig. Det eksisterer likevel i hendelsesloggen for å overholde krav om sporbarhet.

Et skjema ønsker å oppnå statusen "ferdigstilt". Et skjema som ikke er ferdigstilt sies å være i arbeid.

## Eierskap til skjema
Den som har opprettet skjemaet, eller bestilt det utfylt, er definert som eier av skjemaet.

## Hovedskjema og underskjema 
I noen prosjekt velger man å ha flere koblede skjematyper; disse består av en hovedskjematype og en eller flere underskjematyper. 
            
Et underskjema vil typisk være et oppfølgingsskjema og må kobles til et foreldreskjema (kan være hovedskjema eller underskjema). Et hovedskjema kan ikke kobles til andre skjema.
            
Velger man å fylle ut et underskjema for et forskningsobjekt som ikke har sitt foreldreskjema registrert fra før, får man muligheten til å opprette en kladd og koble underskjemaet til dette. Foreldreskjemaet kan da fylles ut senere.
