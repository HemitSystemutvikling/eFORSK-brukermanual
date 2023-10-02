# Hovedskjematype og underskjematype

Hvis et skjema av en skjematype (B) krever eksistensen av et skjema av en annen skjematype (A), er det god praksis å opprette skjematypen B som en underskjematype av skjematypen A. Man får da et metadatafelt på skjematype B med den unike nøkkelen til skjematype A som kan være nyttig ved dataaggregering.

I noen prosjekt kan det være ønskelig med oppfølgingsskjema, og dette kan løses ved å opprette en underskjematype av en hovedskjematype.

Ved opprettelse av en underskjematype må denne kobles til en eksisterende skjematype. Man kan ha flere nivå med underskjematyper.

Disse koblingene reflekteres også ved utfylling av disse skjematypene; utfylling av en underskjematype for et forskningsobjekt må kobles til et foreldreskjema som er fylt ut for samme forskningsobjekt.

### Fordeler ved å ha en underskjematype
*    Man er garantert at hovedskjemaet eksisterer før underskjemaet
*	Man får en koblingsnøkkel på underskjemaet tilbake til hovedskjemaet
*	Hvis et forskningsobjekt har flere skjemaer av hovedskjematypen, så vet man ikke (ingen sterk kobling) hvem et oppfølgingsskjema hører til uten at det er et underskjema av en av de
*	Man kan koble inn skjemaverdier fra hovedskjemaet inn i følgebrevet ved ePROM bestilling av underskjema
*	Fremtidig videreutvikling av eFORSK kan gi ekstra funksjonalitet som om at
     *	verdier arves ned til/er ferdigutfylt i underskjemaet (kompleks ytelsesmessig, ikke sikkert det blir slik)
     *	koblet dataeksport, der man får slått sammen hovedskjema og underskjema i en linje med data (MRS har slik funksjonalitet, men anbefales ikke løst i eFORSK. Mener kobling skjer utenfor eFORSK)

### Ulemper ved å ha en underskjematype
*	Ekstra kompleksitet!
*	Vanskeligere å bestille ePROM av underskjema, da må man referer inn hvilket hovedskjema det skal ligge på
*	Vanskeligere å importere skjemaet av underskjematypen, da må man referer inn hvilket hovedskjema det skal ligge på
