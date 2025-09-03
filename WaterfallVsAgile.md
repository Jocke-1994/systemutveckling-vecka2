Din uppgift är att jämföra hur du skulle bygga en Instagram-liknande app med två olika arbetssätt: Agile och Waterfall (vattenfall). Du ska visa hur plan, process och resultat skulle skilja sig – och vad du hade valt i verkligheten. 

Vattenfall modellen:
I och med att den kräver att man har all info på plats så krävs en gedigen kunskap innan man börjar bygga. Dvs forskning och behovsanalys. Vad krävs för att skapa en socialmedie-app (typ instagram).

Vad är funktioner i en app som instagram? 
-Skapa konto, logga in-ut, radera konto. (glömt lösen)
-Ladda upp bilder på sitt konto (profilbild) eller som en statusuppdatering eller annat.
-Ladda upp film.
-Flöden, kunna kommentera (i text eller bild(gif)), svara flöden 
-Skicka vänförfrågningar.
-Blockera konton.

Extra funktioner?:
-Begära ut eller radera sin egen data (oftast i samband med konto radering.)
-2FA

Systemdesign: Frontend (UI/UX). Databas för att lagra all data. Ett system(kan man kalla det system?) för att hantera frontend och backend samt eventuell molntjänst. 
API för att hantera förfrågningar/requests/begäran om olika data, dvs det som används som kommunikation mellan frontend och backend. Tex för att hämta info om andra konton.


Programmering och Utveckling:
När det kommer till vattenfall modellen som kräver att man vet i förväg vad som ska finnas i appen. Bör man börja med backend delen, databas osv. Innan man angriper frontend. Börjar man med frontend delen först så kan det bli att man måste koda om delar eller hela frontend när man väl ska ge sig på backend, just för att koden inte matchar. Börjar man med backend kan man styra hur koden både ska se ut och bete sig.

Kvalitet och tester:
Det är först här som man i vattenfall modellen får möjlighet att testa sin kod, vilket gör att det kan bli MYCKET extra jobb om det är saker i koden som inte fungerar. Fungerar det inte, får man backa tillbaka och skriva om koden. I detta steget har man alltså byggt klart hela backend och frontend men det är först nu man upptäcker felen.

Leverans och underhåll:
Har man kommit till denna punkt med vattenfalls modellen så är man antingen väldigt bra på att skriva kod, man har gett sig fan på att lyckas eller så är programmet gjort av någon annan som man får fortsätta jobba på.




AGILE:
När det kommer till den agila utvecklingen till att bygga en social-medie app likt instagram:
Skillnaden mellan vattenfall och agila modellen är att du måste utveckla steg för steg på vattenfall. 
I agila modellen bygger du varje sak i en vattenfallsliknande modell. Tex. 
Ska man bygga Databasen så applicerar man vattenfallsmodellen genom att man gör en behovsanalys, design, själva byggandet/koden, testar och kvalitet säkrar för databasen. I och med att man gör dessa steg för varje del av systemet så kan man snabbt se, ok databasen fungerar som jag vill, nu kan jag gå vidare till nästa del i backend och stegen upprepas.

Behovsanalys: Vad ska den användas till och innehålla men även fungera. När man har det kan man gå till designen

Design: Vilka tabeller ska finnas i databasen och vad ska dessa tabeller innehålla. Finns det några nyckelord vi kan använda för att undvika dubbellagring och på så sätt minska minnesanvändning, bibehålla bra prestanda, kanske nyttja user_id istället för det faktiskt namnet. 
Använda indexering, dvs ofta återkommande sökningar. Om någon söker på en kändis så ligger deras konto under user_id i Users och det går snabbare att hitta än att söka igenom hela databasen för att hitta kontot som matchar namnet. osv.

Programmering och Utveckling:
Nu vet man hur man vill att det ska se ut och fungera. Så här bygger vi utefter det som man skissat fram.

Kvalietet och tester:
I detta steget har man antingen byggt en del som man vill testa och se så den fungerar eller så har man byggt allt och nu vill man bara veta att allt fungerar ihop.

Leverans och underhåll: 
Leverera lösningen till kund och se till så att det går att fortsätta bygga systemet, det kommer tillkomma fler saker, uppdateringar för att bibehålla stabilitet, utöka med funktioner och/eller att systemet ska prata med andra system.



Resultatet hade egentligen inte skiljt sig så mycket, skillnaden är hur mycket tid man kunnat lägga ner, hade man orkat lägga tiden som krävs om det är ett stort projekt där risken att man ändrar mycket och man måste använda vattenfallsmodellen?

Jag hade valt agile pga flexibiliteten som man har då.