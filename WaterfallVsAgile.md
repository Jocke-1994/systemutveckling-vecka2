Din uppgift �r att j�mf�ra hur du skulle bygga en Instagram-liknande app med tv� olika arbetss�tt: Agile och Waterfall (vattenfall). Du ska visa hur plan, process och resultat skulle skilja sig � och vad du hade valt i verkligheten. 

Vattenfall modellen:
I och med att den kr�ver att man har all info p� plats s� kr�vs en gedigen kunskap innan man b�rjar bygga. Dvs forskning och behovsanalys. Vad kr�vs f�r att skapa en socialmedie-app (typ instagram).

Vad �r funktioner i en app som instagram? 
-Skapa konto, logga in-ut, radera konto. (gl�mt l�sen)
-Ladda upp bilder p� sitt konto (profilbild) eller som en statusuppdatering eller annat.
-Ladda upp film.
-Fl�den, kunna kommentera (i text eller bild(gif)), svara fl�den 
-Skicka v�nf�rfr�gningar.
-Blockera konton.

Extra funktioner?:
-Beg�ra ut eller radera sin egen data (oftast i samband med konto radering.)
-2FA

Systemdesign: Frontend (UI/UX). Databas f�r att lagra all data. Ett system(kan man kalla det system?) f�r att hantera frontend och backend samt eventuell molntj�nst. 
API f�r att hantera f�rfr�gningar/requests/beg�ran om olika data, dvs det som anv�nds som kommunikation mellan frontend och backend. Tex f�r att h�mta info om andra konton.


Programmering och Utveckling:
N�r det kommer till vattenfall modellen som kr�ver att man vet i f�rv�g vad som ska finnas i appen. B�r man b�rja med backend delen, databas osv. Innan man angriper frontend. B�rjar man med frontend delen f�rst s� kan det bli att man m�ste koda om delar eller hela frontend n�r man v�l ska ge sig p� backend, just f�r att koden inte matchar. B�rjar man med backend kan man styra hur koden b�de ska se ut och bete sig.

Kvalitet och tester:
Det �r f�rst h�r som man i vattenfall modellen f�r m�jlighet att testa sin kod, vilket g�r att det kan bli MYCKET extra jobb om det �r saker i koden som inte fungerar. Fungerar det inte, f�r man backa tillbaka och skriva om koden. I detta steget har man allts� byggt klart hela backend och frontend men det �r f�rst nu man uppt�cker felen.

Leverans och underh�ll:
Har man kommit till denna punkt med vattenfalls modellen s� �r man antingen v�ldigt bra p� att skriva kod, man har gett sig fan p� att lyckas eller s� �r programmet gjort av n�gon annan som man f�r forts�tta jobba p�.




AGILE:
N�r det kommer till den agila utvecklingen till att bygga en social-medie app likt instagram:
Skillnaden mellan vattenfall och agila modellen �r att du m�ste utveckla steg f�r steg p� vattenfall. 
I agila modellen bygger du varje sak i en vattenfallsliknande modell. Tex. 
Ska man bygga Databasen s� applicerar man vattenfallsmodellen genom att man g�r en behovsanalys, design, sj�lva byggandet/koden, testar och kvalitet s�krar f�r databasen. I och med att man g�r dessa steg f�r varje del av systemet s� kan man snabbt se, ok databasen fungerar som jag vill, nu kan jag g� vidare till n�sta del i backend och stegen upprepas.

Behovsanalys: Vad ska den anv�ndas till och inneh�lla men �ven fungera. N�r man har det kan man g� till designen

Design: Vilka tabeller ska finnas i databasen och vad ska dessa tabeller inneh�lla. Finns det n�gra nyckelord vi kan anv�nda f�r att undvika dubbellagring och p� s� s�tt minska minnesanv�ndning, bibeh�lla bra prestanda, kanske nyttja user_id ist�llet f�r det faktiskt namnet. 
Anv�nda indexering, dvs ofta �terkommande s�kningar. Om n�gon s�ker p� en k�ndis s� ligger deras konto under user_id i Users och det g�r snabbare att hitta �n att s�ka igenom hela databasen f�r att hitta kontot som matchar namnet. osv.

Programmering och Utveckling:
Nu vet man hur man vill att det ska se ut och fungera. S� h�r bygger vi utefter det som man skissat fram.

Kvalietet och tester:
I detta steget har man antingen byggt en del som man vill testa och se s� den fungerar eller s� har man byggt allt och nu vill man bara veta att allt fungerar ihop.

Leverans och underh�ll: 
Leverera l�sningen till kund och se till s� att det g�r att forts�tta bygga systemet, det kommer tillkomma fler saker, uppdateringar f�r att bibeh�lla stabilitet, ut�ka med funktioner och/eller att systemet ska prata med andra system.



Resultatet hade egentligen inte skiljt sig s� mycket, skillnaden �r hur mycket tid man kunnat l�gga ner, hade man orkat l�gga tiden som kr�vs om det �r ett stort projekt d�r risken att man �ndrar mycket och man m�ste anv�nda vattenfallsmodellen?

Jag hade valt agile pga flexibiliteten som man har d�.