# Kjente feil i eFORSK

Det avdekkes innimellom feil eller mulige feil som av ulike grunner ikke kan rettes på kort eller lang sikt. Under er en beskrivelse av kjente feil i nyeste versjon av eFORSK.

### Brukere logges ut ved store utsendinger
Det er for tiden en kjent feil med at brukere som håndterer store utsendinger i eFORSK kan bli automatisk logget ut av løsningen etter en gitt tid. Dette skyldes den automatiske fornyelsen av innloggingssesjonen, som kan feile etter en stund dersom store utsendingsjobber blir for krevende. Dette kan dessverre gjøre prosessen mer tidkrevende. Feilen er identifisert og vi arbeider med å fikse metoden for store utsendinger. En nåværende tilpasning som brukere kan gjøre for å redusere risikoen for tvungen utlogging er å korte ned listen over antall personer per utsending til 500-750 personer per utsending. 

### Feil i formler ved kopiering av skjematype
Dersom man bygger en ny skjematype ved å velge "kopi av en annen skjematype" og den opprinnelige skjematypen inneholder formler vil formlene som opprettes i den nye skjematypen bli feil. Her vil det oppstå variabelnavn som ikke stemmer med originalen. 

Eksempel på formel fra opprinnelig skjematype: 

<img width="548" height="147" alt="image" src="https://github.com/user-attachments/assets/5135e222-1089-4486-9600-c4d15aa60d71" />

Formel til den nye opprettede skjematypen: 

<img width="526" height="168" alt="image" src="https://github.com/user-attachments/assets/20e7cf6f-8663-4f6b-aa3b-61f932b5e368" />

Denne kjente feilen er registrert i backlog for videreutvikling og vil bli utbedret. 

