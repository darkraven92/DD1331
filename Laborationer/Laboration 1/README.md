Labb 1
Laboration 1 – Introduktion och Kubsummor
Labbarna görs i i tvåpersonsgrupper. Försök hitta en labbkompis som har lika lite eller lika mycket programmeringserfarenhet som du själv har. I undantagsfall kan man jobba ensam.

Deadline för bonus är 2017-09-08. Skriv ut ett labbkvittoLänkar till en externa sida. för att få papperskopia på dina kursresultat.

Queue
Queue är ett köprogram där studenter kan ställa sig i kö under labbpassen. Finns på queue.csc.kth.se (Länkar till en externa sida.)Länkar till en externa sida. Logga in med kth-konto, välj gruprog och ställ er i kö när ni vill att handledare ska komma för att hjälpa er eller när ni vill redovisa.

Repository på Git
Se till att skapa ett konto och logga in på Kth:s github (Länkar till en externa sida.)Länkar till en externa sida.. Om du gjorde det här för några dagar sedan bör du hitta ett Githubrepo här som heter [ditt användarnamn]-gruproglabb1 här. Om du av någon anledning inte har ett sådant repo så behöver du skapa skapa ett eget privat repo där du kan spara ditt arbete med labben. Klicka på '+'-symbolen i överkanten till höger och välj "create new repo". Välj ett lämpligt namn till exempel [Ditt namn]_labb1. Välj Private och välj valfritt att kryssa i README-rutan. Välj .gitignore för det programmeringsspråk som du har tänkt använda och klicka på "Create repository". I högermarginalen på den sida som kommer upp finns längst ner en knapp märkt "settings". Gå in där och välj "Collaborators" i vänstermarginalen. Se till att din labbkamrat också har skapat ett githubkonto och lägg sedan till hen genom att skriva in användarnamnet och klicka "Add collaborator".

 

För att checka ut repot och göra ändringar i det, följ githubinstruktionerna som finns här (Länkar till en externa sida.)Länkar till en externa sida..

Valfri fördjupning i Git
Instruktionerna i detta stycke ger inte fler bonuspoäng eller högre betyg. Om du vill fördjupa dig i Git så kan du se till att alltid göra en egen fork av ditt genererade repo och när du är klar skicka en pull request till ursprungsrepot. När du gjort detta så kan du stänga issuen om detta i ditt repo. Efter denna mening är den här texten inte längre en valfri fördjupning. Detaljerna om detta står i överkursdelarna av Gitdokumentationen.

Mål för labben
Att bli förtrogen med att köra Pythonprogram från terminalfönstret (eller annat enkelt sätt).
Att kunna skriva små Pythonprogram som
Gör inläsning från terminalfönstret och utskrift i terminalfönstret.
Gör små beräkningar
Använder villkor och repetition.
Kan du redan programmera?
I så fall behöver du kanske inte göra alla små steg i labbarna. Tag fasta på de gråa redovisningsrutorna och se till att du har de program som krävs där.

Tips för alla
Labben har fyra deluppgifter. Endast nr 3 och 4 behöver redovisas. Nybörjare rekommenderas att göra alla uppgifter men försök klara av 1–3 snabbt. Uppgift 4 tar mycket längre tid än övriga uppgifter för de flesta.

 

Uppgift 1
Uppgift 1 behöver inte redovisas

Provkör ett Pythonprogram. Programmet finns här: firstto21.py (Länkar till en externa sida.)Länkar till en externa sida.. Spara programmet på er egen dator. Kör programmet med

python3 firstto21.py
python3 firstto21.py

Spelet går ut på att de två spelarna du respektive datorn omväxlande väljer om 1 eller 2 ska läggas till aktuell summa. Den spelare som når 21 vinner. Går det att vinna över datorn? Titta noga på programkoden och försök förstå de olika delarna. Vilken är datorns(programmets) strategi? Uppgift 1 behöver inte redovisas

1729
1729 är ett intressant tal. Enligt en välkänd anekdot besöker den engelske matematikern Hardy den indiske matematikern Ramanujan på ett sjukhus i London år 1917. Hardy åker taxi till sjukhuset och memorerar taxins nummer, 1729. När Hardy träffar Ramanujan berättar han vilket nummer taxin hade: "Taxins nummer var 1729, det verkar vara ett mycket tråkigt tal. Hoppas det inte är ett dåligt tecken". "Inte alls" svarar Ramanujan. "1729 är ett mycket intressant tal. Det är det minsta (positiva) tal som kan skrivas som summan av två kuber på två olika sätt."

Uppgift 2
Uppgift 2 behöver inte redovisas

Gå till katalogen för första labben. Starta en editor, förslagsvis Atom, och skriv ett program som

Frågar användaren efter två heltal, a och b samt hämtar a och b från terminalfönstret.
Beräknar och skriver ut deras kubsumma, dvs a^3 + b^3.
Programfilen ska ges ett namn som slutar på ".py" t.ex. kubsumma.py. Kör programmet i terminalfönstret med kommandot

python3 kubsumma.py

Genom att köra programmet upprepade gånger och prova med olika a och b kan ni ta reda på vilka de två sätten att skriva 1729 som kubsumma är. Hitta alltså de positiva heltalen a1, b1, a2, b2 som är sådana att
a1^3 + b1^3 = 1729 och a2^3 + b2^3 = 1729 där a1, b1, a2 och b2 alla är olika. Obs! Programmet ska inte leta efter lösningar, bara hämta in två tal och skriva ut kubsumman. Letandet görs genom att ni kör programmet många gånger med olika indata.

"Upphöjt till" skrivs i Python som **, alltså 2**3 är 8. Uppgift 2 behöver inte redovisas

 
Uppgift 3
När man vet att man vill upprepa något många gånger så är det bättre och bekvämare att lägga repeterandet inuti programmet än att köra programmet många gånger. Utvidga programmet från Uppgift 2 så att frågan, beräkningen och utskriften av kubsumman upprepas i all oändlighet eller tills programmet avbryts med t.ex. Ctrl-C, Ctrl-D eller Ctrl-Z.

 

Att redovisa för grunduppgift: Programmet enligt Uppgift 3 som upprepade gånger frågar efter a och b samt beräknar och skriver ut a^3 + b^3 tillsammans med lämplig förklarande text, t.ex.   Kubsumman = 945.
 
Uppgift 4
Skriv ett program som löser problemet att hitta de två lösningarna till a^3 + b^3 = n. n sätts från början till 1729 men programmet ska fungera även för andra positiva värden på n.

 

Börja gärna med att skriva ett program som hittar och skriver ut en lösning och stannar när lösningen är funnen. Utvidga sedan till att hitta två lösningar. Lösningarna ska skrivas ut och programmet ska sluta leta när två lösningar är funna. Försök klura ut själv hur man löser uppgiften men om det är svårt så finns det tips här: 

Ramanujan-tips, hitta EN lösning (Länkar till en externa sida.)Länkar till en externa sida.    Ramanujan-tips, hitta TVÅ lösningar (Länkar till en externa sida.)Länkar till en externa sida..

Tipsen beskriver en något mer avancerad lösningsmodell än de enklaste möjliga som vi godkänner. Ni behöver inte följa tipsen. Dock får ert program inte bestå av koden för att hitta en lösning följt av en repetition av samma kod.

 

För n-värden som inte kan skrivas som summan av två kuber så ska programmet stanna (när sökning inte längre är meningsfull). Program som håller på i "oändlighet" eller "kraschar" godkänns inte. Dock behöver ingen särskild utskrift göras om lösningar saknas (men det är trevligt att ge en sådan!).

Att redovisa för grunduppgift: Programmet enligt Uppgift 4 som utan indata letar rätt på de två lösningarna till a^3 + b^3 = n, där n satts till 1729. Om man vill undersöka ett annat tal än 1729 ska det räcka med att ändra på ett enda ställe i programmet. Programmet måste avslutas även om inga lösningar hittas och det får inte ske med felavbrott.
Alternativ redovisning, med indata: Låt programmet fråga vilket tal, n som ska undersökas och skriv ut ev. lösningar till a^3 + b^3 = n.

När allt är redovisat, be om lärarens signatur på ditt labbkvittot.
Tag fram labbkvittot före redovisningen.

 

 

Extrauppgift för betygshöjning

Vi tittar igen på problemet att hitta lösningar (a,b) till a^3 + b^3 = N.   a, b och N är positiva heltal.

Skriv en funktion som returnerar en lista med lösningarna till a^3 + b^3 = n där n är funktionens enda parameter.

En lösning utgörs av ett par (a,b). En lista av lösningar är alltså en lista av sådana par. T.ex. så är  [(17,76),(38,73)]  lösningslistan för n = 443889. Observera att lösningarna ska "samlas ihop" och utgöra funktionens returvärde. Om lösningar saknas returneras [] (tomma listan). Lösningarna ska inte skrivas ut inuti funktionen (utskrift under en testningsfas är ok). Testa funktionen genom att anropa den med några värden på n där ni vet svaret och kontrollera att det blir rätt svar. Se till att inga dublettlösningar finns med i svaret. T.ex. om (17,76) är med i lösningslistan så ska inte (76,17) vara där.

Man kan leta efter lösningar på samma sätt som i Uppgift 4 men försök gärna effektivisera.

 

anrop	   	funktionsvärde
ramanujan(1729)	   	[(1,12),(9,10)]
ramanujan(152)	   	[(3,5)]
ramanujan(3697)	   	[] 

 

Att redovisa för betygshöjning:
En funktion som från n beräknar och returnerar en lista med lösningar.
Extrauppgiften bokförs på labbkvittot.
