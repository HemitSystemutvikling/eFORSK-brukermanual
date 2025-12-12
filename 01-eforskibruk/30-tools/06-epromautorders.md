# Automatiske ePROM-bestillinger

Denne funksjonen er ikke tilgjengelig som standard i eFORSK og må etterspørres for aktivering. Merk at man her kan få bestilt store mengder skjemaer til utfyllelse som medfører en **kostnad**. Når man lager bestillingsjobber har man selv ansvaret for at disse settes opp riktig og at de ikke bestiller mer enn de skal.

## Hva er bestillingsjobber

Istedenfor å manuelt bestille skjemautfyllelse, kan man automatisere prosessen. 
Hvis man ønsker at det automatisk skal bestilles skjemautfyllelse fra personer 
eksempelvis 30 dager etter at et skjema ferdigstilles, må man sette opp en bestillingsjobb. 

I utgangspunktet 
kan man sette opp at et skjema av hvilken som helst skjematype automatisk bestiller skjemautfyllelse av hvilken 
som helst ePROM aktiverte skjematype. Det vanligste eksempelet er at man har en foreldreskjematype som bestiller utfyllelse 
av en tilknyttet skjematype:
<img width="423" height="101" alt="aut orders" src="https://github.com/user-attachments/assets/6dfc4d2d-a5c5-4c09-80ce-12f70e082dce" />

## Konfigurasjon

Skjematype som trigger bestiling og skjemaversjon som bestilles kan ikke endres etter at bestilligsjobben er opprettet. Man må da lage en ny jobb.

### Skjematype som trigger bestilling

Skjemaer av skjematypen som er satt opp til å trigge bestilling overvåkes av bestillingsjobben. Oppfylles kravene som konfigureres her, vil bestillingsjobben planlegge bestilling. Å *planlegge en bestilling* vil si at en ePROM-bestilling opprettes med status "planlagt" og et bestillingstidspunkt, som kan sees under ePROM i menyen.

Lager man en jobb der man ikke ønsker at eksisterende skjema skal bli triggerskjema, kan man spesifisere at triggerskjema må være opprettet fra og med et tidspunkt.

Videre kan man også velge at triggerskjemaet må ha noen gitte verdier i valgfelt eller avkrysningsfelt. Eksempelvis kan man si at kun skjemaer med svar "Ja" på spørsmål om "Ønsker pasient videre oppfølging?" skal være et triggerskjema.

### Skjemaversjon som bestilles

Her kan man velge når skjemautfyllelse skal bestilles i forhold til triggerskjemaet. Merk at hvis skjemaversjon som bestilles er av en underskjematype, og skjematypen som trigger bestilling ikke er foreldreskjematypen til denne, vil et foreldreskjema opprettes som kladd ved besvarelse av bestillingen.

Hvis skjemaversjonen ikke har status publisert, vil skjemabestillinger planlegges som vanlig - men bestillingen vil ikke gjennomføres og resultere i feilmelding. Avpubliserer eller låser man en skjemaversjon for godt, bør man også stoppe bestillingsjobben.

### Gjentagende bestilling

Man kan sette opp inntil 30 gjentagende bestillinger på et triggerskjema, som da kan føre til totalt 31 bestillinger. Som standard kreves det svar på en bestilling før den neste planlegges. Man kan også velge at det ikke kreves besvarelse, da vil alle gjentagende bestillinger planlegges samtidig.

Et typisk eksempel på bruk av gjentagende bestilling er ønske om svar på helsetilstand fra en pasient hver 30. dag i en periode.

## Aktivering

En bestillingsjobb kan aktiveres individuelt for testmodus og ikke-testmodus. Er den aktivert for en av disse, kan den ikke redigeres. Deaktiveres jobben, vil alle bestillinger som er planlagt av jobben avbrytes. Bestillinger som allerede er bestilt røres ikke.

Endrer man status, vil det startes en prosess med å planlegge og/eller avbryte bestillinger. Mens dette skjer, har man ikke mulighet til å gjøre nye statusendringer eller konfigurasjon. Tiden dette tar avhenger av hvor man skjemaer man har i sin database.

## Bestillinger

Bestillinger fra bestillingsjobber gjøres fortløpende etter at et skjema lagres. Det vil si at om man manuelt fyller ut skjema i eFORSK, importerer data eller får svar på en bestillelse om skjemautfyllelse (via ePROM), vil bestillingsjobbene sjekke om dette er et triggerskjema som oppfyller kravene som skal føre til en bestilling.  Merk at det kan ta noen sekunder etter at et skjema er lagret før bestillingsjobben er ferdig med å planlegge bestillinger.

En bestilling opprettet av en bestillingsjobb planlegges tidligst en time frem i tid, slik at man etter aktivering av en bestillingsjobb har tid til å sjekke at bestillingene har blitt planlagt som tenkt.

Planlagte bestillinger vil bestilles av eFORSK hver hele time, det oppgitte bestillingstidspunktet er altså bare det tidligst mulige tidspunktet for bestilling.

Man kan manuelt avbryte en planlagt bestilling av bestillingsjobben ved klikk på avbryt knappen ved siden av bestillingen. Bestillingen  skal da forbli avbrutt selv om man stopper bestillingsjobben og aktiverer den igjen.

Slettes triggerskjemaet, vil alle planlagte bestillinger laget ut i fra denne avbrytes.
