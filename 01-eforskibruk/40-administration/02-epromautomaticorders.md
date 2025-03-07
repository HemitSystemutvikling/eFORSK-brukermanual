# ePROM automatiske bestillingsjobber

Denne funksjonen er ikke tilgjengelig som standard i eFORSK og må etterspørres for aktivering. Merk at man her kan få bestilt store mengder skjemaer til utfyllelse som medfører en **kostnad**, når man lager bestillingsjobber har man selv ansvaret for at dem settes opp riktig og at dem ikke bestiller mer enn dem skal.

## Hva er bestillingsjobber

Istedenfor å manuelt bestille skjemautfyllelse, kan man automatisere prosessen. 
Hvis man ønsker at det automatisk skal bestilles skjemautfyllelse fra personer 
eksempelvis 30 dager etter at et skjema ferdigstilles, må man sette opp en bestillingsjobb. 

I utgangspunktet 
kan man sette opp at et skjema av hvilken som helst skjematype automatisk bestiller skjemautfyllelse av hvilken 
som helst ePROM aktiverte skjematype. Det vanligste eksempelet er at man har en foreldreskjematype som bestiller utfyllelse 
av en tilknyttet skjematype:

![Skjematyper](data:image/png;base64,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)

## Konfigurasjon

Skjematype som trigger bestiling og skjemaversjon som bestilles kan ikke endres etter at bestilligsjobben er opprettet. Man må da lage en ny jobb.

### Skjematype som trigger bestilling

Skjemaer av skjematypen som er satt opp til å trigge bestilling overvåkes av bestillingsjobben. Oppfylles kravene som konfigureres her, vil bestillingsjobben planlegge bestilling. Å *planlegge en bestilling* vil si at en ePROM bestilling opprettes med status "planlagt" og et bestillingstidspunkt, som kan sees under ePROM i menyen.

Lager man en jobb der man ikke ønsker at eksisterende skjema skal bli triggerskjema, kan man spesifisere at triggerskjema må være opprettet fra og med et tidspunkt.

Videre kan man også velge at triggerskjemaet må ha noen gitte verdier i valgfelt eller avkrysningsfelt. Eksempelvis kan man si at kun skjemaer med svar "Ja" på spørsmål om "Ønsker pasient videre oppfølging?" skal være et triggerskjema.

### Skjemaversjon som bestilles

Her kan man velge når skjemautfyllelse skal bestilles i forhold til triggerskjemaet. Merk at hvis skjemaversjon som bestilles er av en underskjematype, og skjematypen som trigger bestilling ikke er foreldreskjematypen til denne, vil et foreldreskjema opprettes som kladd ved besvarelse av bestillingen.

Hvis skjemaversjonen ikke har status publisert, vil skjemabestillinger planlegges som vanlig - men bestillingen vil ikke gjennomføres og resultere i feilmelding. Avpubliserer eller låser man en skjemaversjon for godt, bør man også stoppe bestillingsjobben.

### Gjentagende bestilling

Man kan sette opp inntil 30 gjentagende bestillinger på et triggerskjema, som da kan føre til totalt 31 bestillinger. Som standard kreves det svar på en bestilling før den neste planlegges. Man kan også velge at det ikke kreves besvarelse, da vil alle gjentagende bestillinger planlegges samtidig.

Et typisk eksempel på bruk av gjentagende bestilling er ønske om svar på helsetilstand fra en pasient hver 30. dag i en periode.

## Aktivering

En bestilling jobb kan aktiveres individuelt for testmodus og ikke-testmodus. Er den aktivert for en av disse, kan den ikke redigeres. Deaktiveres jobben, vil alle bestillinger som er planlagt av jobben avbrytes. Bestillinger som allerede er bestilt røres ikke.

Endrer man status, vil det startes en prosess med å planlegge og/eller avbryte bestillinger. Mens dette skjer, har man ikke mulighet til å gjøre nye statusendringer eller konfigurasjon. Tiden dette tar avhenger av hvor man skjemaer man har i sin database.

## Bestillinger

Bestillinger fra bestillingsjobber gjøres fortløpende etter at et skjema lagres. Det vil si at om man manuelt fyller ut skjema i eFORSK, importerer data eller får svar på en bestillelse om skjemautfyllelse (via ePROM), vil bestillingsjobbene sjekke om dette er et triggerskjema som oppfyller kravene som skal føre til en bestilling.  Merk at det kan ta noen sekunder etter at et skjema er lagret før bestillingsjobben er ferdig med å planlegge bestillinger.

En bestilling opprettet av en bestillingsjobb planlegges tidligst en time frem i tid, slik at man etter aktivering av en bestillingsjobb har tid til å sjekke at bestillingene har blitt planlagt som tenkt.

Planlagte bestillinger vil bestilles av eFORSK hver hele time, det oppgitte bestillingstidspunktet er altså bare det tidligst mulige tidspunktet for bestilling.

Man kan manuelt avbryte en planlagt bestilling av bestillingsjobben ved klikk på avbryt knappen ved siden av bestillingen. Bestillingen  skal da forbli avbrutt selv om man stopper bestillingsjobben og aktiverer den igjen.

Slettes triggerskjemaet, vil alle planlagte bestillinger laget ut i fra denne avbrytes.
