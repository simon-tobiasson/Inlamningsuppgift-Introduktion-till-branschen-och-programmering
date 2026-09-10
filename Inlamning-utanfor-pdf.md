Del 1 - Analysera en teknisk lösning 
Välj en digital tjänst du använder varje dag (t.ex. Spotify, Instagram, Swish eller Google Drive). Analysera den utifrån de två nedan perspektiv: (G)
Viktigt här att det handlar inte om att jag förväntar mig ett visst svar utan jag vill se hur dina idéer och hur du resonerar. Det är väldigt svårt att faktiskt veta hur många tjänster fungerar. 
Hållbarhet 
Hur använder tjänsten resurser? 
Hur skulle den kunna bli mer hållbar? 
Säkerhet 
Vilka typer av data hanterar tjänsten? 
Vilka säkerhetsåtgärder tror du finns? 
Finns det några risker? 
Svara med cirka 300–500 ord. 

Del 1 
Jag kommer analysera den mest använda spelplattformen på windows (Steam), vilka resurser som används samt hur ägaren och skaparen av tjänsten (Valve Corporation) använder de olika resurserna. Därefter går jag in på hur hållbar resurserna är och hur dem skulle kunna vara mer hållbara. Jag kommer även gå in på vilka typer av data som steam hanterar, hur de hanterar dem, vilka säkerhetsåtgärder jag tror finns inom dem datatyperna på steam samt att jag kommer röra vid olika risker som finns inom dem. 

Vilka olika resurser använder steam och hur används dem? 
Valve Corporation har mängder olika resurser för att driva spellagrings plattformen Steam. Jag kommer fokusera på 3 stora resurser inom Steams backend infrastruktur (Steam Cloud, SteamPipe och Steam Datagram Relay). 

Steam Cloud är en resurs som både steam och spelutvecklare använder. Steam använder Steam Cloud inom att lagra användarinformation medan spelutvecklare kan använda Steam Cloud för att lagra olika datatyper såsom spelinställningar, sparfiler och profilinställningar.  

En annan resurs vid namnet SteamPipe är ett innehålls distributionssystem som Valve dem själva har byggt upp. SteamPipe har huvudmålet att göra det mer tillgängligt för spelare att ladda ner och uppdatera sina spel samt öka hastigheten på nedladdningarna med hjälp av att använda HTTP istället för att använda ett egenutvecklat leveransprotokoll.  

Den sista resursen jag har fördjupat mig inom är Steam Datagram Relay (SDR), Valves privata virtuella spelnätverk. Resursen används inom spelutvecklare som har spelare som ska spela med varandra, multiplayer. Det främsta målet med SDR är att göra det svårare för Dos-attacker genom att skydda och aldrig avslöja IP-adresser på både spelare och servrar. Med de dedikerade spelservrarna flyttas även spelarna snabbare över internet vilket resulterar till lägre ping hos spelarna. Valves egna spel såsom Counter Strike 2, Team Fortress 2 och Dota 2 använder exklusivt SDR inom officiella servrar.  

Hur skulle de 3 resurserna bli mer hållbara? 

Dessa 3 resurserna är optimerade för att vara så hållbara som möjligt.  

När det kommer till Steam Cloud har Valve skapat ett val för användaren som ändrar vilka spel som steam ska synkronisera med Cloud. Om användaren har bestämt sig att bara spela ett specifikt spel på en specifik enhet, då kan användaren slå på den egenskapen. Dessutom har Valve utvecklat en funktion vid namnet Dynamic Cloud Sync (DCS) där bara filer som har ändrat sig synkroniserar. DCS fungerar även när Steam Deck (Valves handhold konsoll) går i viloläge och sparfilerna automatiskt synkroniserar sig med molnet så det blir enklare att byta från Steam Deck till en annan enhet. 

Det jag kan se som kan vara mer hållbart är för spel som inte har DCS. Spel som har flera hundra olika sparfiler som måste synkronisera tar upp en del molnlagring. Att ha en funktion som raderar gamla sparfiler som användaren godkänner kan göra det mer hållbart i själva molnlagringen. 

SteamPipes hållbarhetsfrågor strävar in mot dess huvudfunktion, nedladdningar. Det som SteamPipe gör när filer uppdateras är att den skriver in filerna innan den raderar gamla filer. Spel som är gigantiska kontra andra spel, alltså 100 GB stora, tar rätt så lång tid att uppdatera om användarens diskar har för lite utrymme på dem. Jag själv har detta problem med större spel såsom Diablo 4 och Baldur’s Gate 3 att det tar längre tid att uppdatera spelet än att installera om hela spelet på nytt.  

För att göra det hållbart och inte slita på diskar skulle jag göra det så att SteamPipe inte skriver ner uppdaterade filer före den raderar gamla filer.  

Med att Steam Datagram Relay är ett system som forslar speltrafik så måste det finnas datacenter runt omkring världen för att göra pingen så låg som möjligt för så många spelare som möjligt. SDR:s datacenter har exakt samma hållbarhets problem som vartenda datacenter har... det tar mycket energi att hålla igång dygnet runt och det krävs mycket vatten för att kyla ner servrarna.  

Datacenter har blivit mer effektiva över åren. Från förbättrad effektivitet inom energianvändande till att använda luften för att kyla ner. Jag själv tror nog att bygga datacenter där det är riktigt kallt som till exempel Sibirien (som det säkert redan finns men Ryssland är Ryssland och den informationen fanns inte på det diagrammet vi kollade på onsdag 2 september) är en bra plats att bygga datacenter. Tråkigt nog är det ineffektivt att bygga datacenter i Sibirien på grund av att infrastrukturen inte finns, energin är dålig, internet-förbindelsen till Sibirien är också dålig samt att det politiska läget vi lever i med Ryssland har ändrats drastiskt efter Ryssland började invasionen av Ukraina. Det kommer kosta för mycket att bygga upp en ny civilisation ute i Sibirien för att starta datacenter. Ställen där det redan finns civilisation och infrastruktur är de norra länderna, varav i Sverige finns det redan datacenter i vårt nedkylda norr där centrarna använder den kalla luften istället för enorma mängder vatten. 

Vilka typer av data hanterar steam? 

Steam hanterar mängder av olika datatyper, från bildfiler, inloggnings- och transaktionsuppgifter till kommunikationsinformation och spelstatistik.  

Vilka säkerhetsåtgärder tror jag finns på steam? 

Kort sagt: MÄNGDER med säkerhetsåtgärder. 

Lite längre sagt: Som varje lösenord på internet, dem är krypterade. Användaren kan sätta på tvåfaktorsautentisering för att få återkomst till sitt konto. Denna F2A kommer i form av en 5 teckenkod vilket skickas till användarens email. BankID används när man köper spel. När man skapar ett lösenord för användarens Steam konto måste lösenordet ha minst 6 tecken, en stor och en liten bokstav samt minst en siffra.  

Finns det några risker? 

Ja, det finns ett antal olika risker inom Steam. Hackare kan komma in på ens konto om man inte använder alla säkerhetsåtgärder, om man använder ett av sina globala lösenord.  

Steam support är stenhårda och har alltid varit stenhårda på att återfå ett hackat konto.  Om någon annan person har fått tillgång till ett konto utan original användarens godkännande, då är Steam support monstret under sängen till hackaren. 


Del 2 - Pseudokod 

Skriv pseudokod för nedan problem. Du kan göra detta i textdokument eller använda ett program som draw.io och då bifoga en länk till ditt flödesdiagram. Ifall man siktar på VG så behöver man göra både G och VG - nivån. 

G - nivå - Split the nota 

Split the nota räknar ut hur mycket varje vän ska betala på exempelvis en restaurang när notan kommer. Användaren matar in summan, antal vänner och sedan dricks (som skrivs i decimalform d.v.s 10% blir 0.10). Skisserna nedan är mest för att ge visuell bild av hur det ser ut, ni behöver inte ha med sådant som "byt vy" eller liknande i er pseudokod.  

Del 2 uppgift 1 (G) 

Pseudokod för ett program som ska ta in en summa, hur många personer som ska betala summan och dricks i form av decimaltal som är en andel procent av total summan och sedan adderas på summan. Sedan ska den summan divideras med antal personer som ska betala och den individuella summan skrivs ut till användaren. 

 

START 

Output “Ange hur mycket notan kostar:” 
nota = Input 

Output “Hur många ska betala?” 
antalPersoner = Input 

Output “Hur mycket dricks i procent vill ni ge?” 
dricksProcent = Input 

dricksSumma = nota * (dricksProcent /100) 

helaNotan = nota + dricksSumma 

summaPerPerson = helaNotan / antalPersoner 

Output “Ni ska betala “summaPerPerson” var.” 

END 


Del 2 uppgift 2 (VG) 

VG - nivå - Bibliotekssystem 

Du arbetar med ett bibliotekssystem. Nedan hittar du något som liknar pseudokod men jag vill att du utvecklar detta mer samt ser till att allt körs i rätt ordning. 

Programmet ska: 
Fråga om användaren vill låna en bok. 
Om svaret är ja ska programmet fråga om bokens namn. 
Programmet ska kontrollera om boken finns. 
Om boken finns ska antalet utlånade böcker som användaren har kontrolleras 
Om användaren har mindre än två böcker lånade just nu ska boken markeras som utlånad 
Om användaren har två böcker lånade ska ett meddelande visas 
Om boken inte finns ska ett meddelande visas. 
Om användaren svarar nej ska programmet avslutas. 

START 

OUTPUT “Vill du låna en bok? (ja/nej)” 
“svar” = INPUT 

OM “svar” = “ja” DÅ 

       OUTPUT “Vad heter boken?” 
       “bokensNamn” = INPUT 

       HÄMTA “utlånadeBöcker” 

       OM “bokensNamn” INTE finns i “utlånadeBöcker” DÅ 

              HÄMTA “antalUtlånadeBöcker” 

              OM “antalUtlånadeBöcker” är mindre än 2 DÅ 

                     “bokensNamn” = utlånad 

              ANNARS 

                     OUTPUT “Du har redan 2 böcker utlånade och kan inte låna fler till du har  
                     återlämnat en bok” 

              SLUT_OM 

       ANNARS 

              OUTPUT “Tyvärr boken finns inte i vår lista” 

       SLUT_OM 

ANNARS 

       Avsluta programmet 

SLUT_OM 

SLUT 

 

Del 3 - Reflektion 

Nedan två frågor ska besvaras separat. 

Del 3 uppgift 1 (G) 

Efter två veckor på utbildningen, hur ser du på rollen som backend utvecklare? Utgå från dina tankar och resonera utifrån vad du tycker. Runt 200-500 ord. (G) 

Efter två veckor på utbildningen ser jag på backend utvecklingsrollen som en stark, och viktig del i applikationsutvecklingens kugghjul.  Utan backend kan flertalet av de andra rollerna inte göra någonting. Frontend kan till exempel inte bygga gräns-snittet utefter UI/UX-designen om dem inte har tillgång att hämta information från en server eller databas. Under de 2 veckorna har det blivit tydligt för mig att backend är fötterna som resten av applikationer vilar på. Personligen har jag blivit mer intresserad av backend efter de här 2 veckorna och är ytterst exalterad över att lära mig fördjupad C#, uppbyggningen av databaser och konnektiviteten till molnet. Det var väldigt intressant att lära mig hjärnan och tänkandet hos en datalogiker, samt att det är roligt att sätta mig in i dem tankesätten för att hitta smarta lösningar på problem och det kommer vara ännu roligare med komplexa problem.  

Utanför den tekniska biten inom backend blev jag väldigt intresserad i tankesätten bakom grupparbeten och projekt som mestadels görs inom grupper. Jag har under lång period hellre tyckt om att jobba i grupp med människor än att jobba ensam. Även inom min hobby för datorspelande har jag alltid lockats till grupp- och vänskapsspel men ändå varit intresserad i solo spel för att sedan diskutera det med vänner. När programmeringskursen startar igång kommer det vara väldigt roligt att prata med de andra studenterna på vad deras idéer är, vilka problem dem har och lösningarna dem har för dem problemen så att jag kan sedan ge in egna input om dem vill höra dem.  


Del 3 uppgift 2 (VG) 

Hur tror du AI kommer påverka yrkesrollen de kommande fem åren? Runt en 300-500 ord. (VG) 

Vad jag tror är att AI kommer förändra sig enormt innan de kommande fem åren, lika mycket som det förändrade sig de tidigare fem åren. AI kommer fortfarande finnas, det är garanterat, men jag tror att den kommer se annorlunda ut. Mina tankar kring hur kostsamt AIn är får mig att tänka på att gratis versioner inte kommer vara lönsamt längre fram. Dessutom får jag tankar om att populära LLM som allmänheten använder idag kommer antingen bli starkare eller svagare beroende på hur världen reagerar på energi- och vattenanvändningen som datacenter drar.  

Om AIn ser likadant ut om fem år som den gör idag kommer inte AIn påverka backend utvecklningsrollen lika mycket som den gör på andra roller. Vad jag tror så är det problematiskt för AI att spinna upp databaser på ett effektivt sätt utan att en människa sitter bakom ratten. AIn kan redan prata med varandra och starta databaser men om mänskligheten låter AIn göra det för sig själv, då tror jag att det blir problematiska konsekvenser.  

Men om AIn förändrar på sig, att den kan hålla iordning på databaser och molnet felfritt, då kommer backend utveckling vara mer utvecklingen bakom AI än utveckling på tjänster.  
