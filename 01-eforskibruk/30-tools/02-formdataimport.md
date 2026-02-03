# Importer data 

## Importfil

Filer av typen csv, xls, xlsx og sav støttes. 
Første rad i fila skal inneholde variabelnavn.
Det finnes ingen deteksjon for om et skjema er importert fra før, dette må man holde orden på selv.
Importerer man samme fil to ganger vil man få dobbelt opp med skjema.

## Forskningsobjektets ID

Det er krav om at en kolonne inneholder forskningsobjektets ID. 
I tilfelle forskningsobjekttypen "personer fra personregisteret", må man ha tall med nøyaktig lengde 11 siffer.
Sørg for at fødselsnummer som starter på tallet 0 ikke får denne fjernet (i excel formaterer man kolonnen som tekst).

## Datatyper

Hver kolonne i importfila vil analyseres, og sammenlignes opp mot felter i valgt skjematype.
Man får mulighet til å koble en kolonne i importfila til passende felter i skjematypen. 
Skulle en verdi i kolonnen ikke ha en gyldig verdi for feltet, får man ikke mulighet til å importere denne kolonnen til dette feltet.
Eksempelvis vil et tallfelt som har satt minimumsverdi 0, ikke godta en kolonne som skulle inneholde et negativt tall.
Hvis tall i kolonnen har flere desimaler enn hva tallfeltet er satt opp for, blir det avrundet ved import.

Det er ikke mulig å importere data til systemutfylte felter. Disse vil fylles ut av systemet ved importering. Unntaket her er forskningsobjektets ID som kreves for å koble mot riktig forskningsobjekt.

## Store datamengder 

Store mengder skjemaer som skal importeres bør deles opp i flere filer slik at hver fil ikke inneholder mer enn et par tusen skjema.
Denne datamengden tar få minutter å importere, avhengig av ledige ressurser på server. 
Det er ikke mulig å stoppe en importjobb som er i gang.
Store importjobber tar lang tid, og øker sannsynligheten for at serveren kan bli avbrutt i arbeidet med å importere skjema.
Mindre filer gjør det enklere å starte på nytt om noe skulle gå galt.

## Feil i importjobb

Om importjobben skulle få status "feilet" har mest sannsylig serveren blitt forstyrret i arbeidet.
Noen av skjemaene har antagelig ikke blitt importert, man må da lage en ny importjobb for å gjøre et nytt forsøk.
Dette vil føre til duplikater av skjemaene som faktisk ble importert i første forsøk.
Dette unngår man ved bruk av knappen "Slett importerte skjema" i den feilede importjobben.
