# Scripts Video's Inleiding Wetenschappelijk Programmeren

## Overzicht
1. VSC gebruiken - *Ingesproken door: Mirja - Render ready*
2. Variabelen - *Ingesproken door: Wouter -* *Render ready*
3. Condities - *Ingesproken door: Quinten - Render ready*
4. Loops
    1. Tellen/Herhalen - *Ingesproken door: Mirja - Render ready*
    2. Rekenen - *Ingesproken door: Mirja - Render ready*
    3. Filteren - *Ingesproken door : Mirja - Render ready* 
    4. Gebruikersinvoer - *Ingesproken door Mirja - Render ready* 
5. Lijst - *Ingesproken door: Quinten - Script besproken*
6. Functies
    1. Functies definiëren & aanroepen - *Low priority*
    2. Functies met één parameter - *Ingesproken door: Tim -* *Render ready*
    3. Functies met meerdere parameters -*Ingesproken door: Tim -* *Render ready*
    4. Functies met lijsten - *Render ready*
    5. Functies in functies aanroepen & meegeven - *Low priority*


## 1. Visual Studio Code gebruiken

In deze video leg ik uit hoe je Visual Studio Code kunt gebruiken. 
Het is een vrij uitgebreide omgeving en je hebt eigenlijk maar een paar onderdelen nodig. 

Voordat je begint met programmeren is het gemakkelijk om een map aan te maken om je bestanden in op te slaan. 
Daarna kun je op “Open Folder” klikken om deze map te openen in Visual Studio Code. 

Nu kun je aan de linkerkant van het scherm zien welke bestanden in de map opgeslagen zitten. 
Op dit moment is de map nog leeg. 
Door op het document-icoontje te klikken kun je een nieuw bestand aanmaken en een naam geven, bijvoorbeeld: hello.py. 
Na het aanmaken van het bestand wordt het automatisch geopend aan de rechterkant van het scherm. 

Je kunt code schrijven in het bestand, bijvoorbeeld print “Hallo python” en opslaan met **control s**.

Om je programma te runnen moet je eerst een terminal openen door tegelijkertijd control en achterwaartse apostrof in te drukken. 
De terminal verschijnt onderaan het scherm. 
Het kan zijn dat de terminal er bij jou iets anders uitziet. 
Tik vervolgens in “python” gevolgd door de naam van het bestand,  in dit geval “hello.py”, en druk op Enter. 
Zoals je ziet wordt inderdaad “Hallo Python” geprint.

Je kunt de terminal ook gebruiken om direct commando’s te geven. 
Tik in “python” en druk op Enter om python op te starten.
Als je bijvoorbeeld **p****rint “Hallo”** typt en op Enter drukt, dan wordt “Hallo” geprint.  
Daarnaast kun je berekeningen doen, bijvoorbeeld 4 + 4. 
Om python weer te stoppen kun je “exit” intikken gevolgd door een haakje openen en haakje sluiten en op Enter drukken. 

Het kan soms zijn dat de directory van de terminal niet overeenkomt met de directory van het programma dat je wil runnen. 
Dan krijg je de foutmelding “can’t open file ‘hello.py’”. 
Door “pwd” in te typen en op Enter te drukken kun je zien in welke directory de terminal zich op dit moment bevindt. 
Je ziet dat de terminal in de **downloads** directory staat, maar het bestand hello.py staat in een speciale map. 
Om dit te fixen kun je met de rechtermuisknop klikken op het bestand hello.py en dan op “Open in command prompt”.
Zo kun je het programma weer runnen. 

Oh, nog even een trucje.
Stel je past het programma hello.py aan door leestekens toe te voegen …  
[Hallo komma Python uitroepteken aanpassen]
Als je het programma nu nog een keer wil runnen, dan kun je het pijltje naar boven gebruiken om vorige commando’s in de terminal op te halen. 
Door op Enter te drukken wordt het programma meteen opnieuw gerund. 


## 2. Variabelen

In deze video leg ik uit hoe je variabelen kunt gebruiken. 

Variabelen zijn bijvoorbeeld handig wanneer je de uitkomst van een berekening wilt gebruiken in een andere berekening. 
Elke variabele heeft een *naam* en een *waarde*.
~~~~Je mag de naam van de variabele zelf bepalen, maar zorg er wel voor dat je een korte en duidelijke naam kiest.
~~~~
Een voorbeeld.
Stel je wilt je inkomsten en uitgaven van deze maand berekenen. 

Eerst de inkomsten. 
Je krijgt van DUO studiefinanciering van 277 euro per maand.
Dus je maakt de variabele “studiefinanciering” aan, en geeft deze de waarde 277.
En je hebt een bijbaan waarmee je 500 euro per maand verdient.
Dus dan maak je de variabele “bijbaan” en je geeft ‘m de waarde 500. 
Je kunt nu al je inkomsten berekenen door de variabelen bij elkaar op te tellen. 
Deze uitkomst kun je ook weer opslaan in een variabele, dus: “inkomsten… is… studiefinanciering… plus bijbaan”.  
Als je nu de variabele “inkomsten” print…
en het programma runt…
[runnen programma]


    studiefinanciering = 277
    bijbaan = 500
    inkomsten = studiefinanciering + bijbaan
    print("Inkomsten:", inkomsten)

… dan zie je dat je totale inkomsten gelijk is aan 777 euro. 

Op dezelfde manier kun je nu ook je uitgaven berekenen. 
De huur voor je studentenkamer is 390 euro per maand. 
Je gaat deze maand 175 euro uitgeven aan boodschappen en 125 euro aan leuke dingen. 
[korte pauze]
Vervolgens bereken je je totale uitgaven: “uitgaven… is gelijk aan… huur… plus boodschappen… plus leuke dingen”.
Dus je uitgaven van deze maand zijn…
[runnen programma]


    studiefinanciering = 277
    bijbaan = 500
    inkomsten = studiefinanciering + bijbaan
    print("Inkomsten:", inkomsten)
    
    huur = 390
    boodschappen = 175
    leuke_dingen = 125
    uitgaven = huur + boodschappen + leuke_dingen
    print("Uitgaven:", uitgaven)

…  690 euro. 

Als je dit hebt kun je ook uitrekenen hoeveel geld je aan het einde van de maand over houdt.
Je trekt de “uitgaven” van de “inkomsten” af en slaat het resultaat op in een nieuwe variabele, bijvoorbeeld “spaarrekening”. 
Dus: “spaarrekening… is gelijk aan… inkomsten… min… uitgaven”.
Dus aan het einde van de maand hou je in totaal…
[runnen programma]


    studiefinanciering = 277
    bijbaan = 500
    inkomsten = studiefinanciering + bijbaan
    print("Inkomsten:", inkomsten)
    
    huur = 390
    boodschappen = 175
    leuke_dingen = 125
    uitgaven = huur + boodschappen + leuke_dingen
    print("Uitgaven:", uitgaven)
    
    spaarrekening = inkomsten - uitgaven
    print("Spaarrekening:", spaarrekening)

… 87 euro over.

Nu alle formules op een rijtje staan hebben we een recept voor het doorrekenen van al je financiën. 
Dat kunnen we dan ook makkelijk aanpassen.
Stel je hebt een nieuwe bijbaan gevonden waar je niet 500 euro, maar 575 euro per maand gaat verdienen. 
Je hoeft deze wijziging maar op één plek in het programma door te voeren om het totaal weer kloppend te maken.
Namelijk… de waarde van de variabele bijbaan moet veranderd worden van 500 naar 575 euro.
Als we het programma nu opnieuw runnen…
[runnen programma]


    studiefinanciering = 277
    bijbaan = 575
    inkomsten = studiefinanciering + bijbaan
    print("Inkomsten:", inkomsten)
    
    huur = 390
    boodschappen = 175
    leuke_dingen = 125
    uitgaven = huur + boodschappen + leuke_dingen
    print("Uitgaven:", uitgaven)
    
    spaarrekening = inkomsten - uitgaven
    print("Spaarrekening:", spaarrekening)

 
… dan zie je dat je nu 162 euro aan het einde van de maand overhoudt. 

Je moet bij het aanmaken van variabelen erop letten dat Python je code van boven naar beneden doorloopt. 
Dat betekent dat je een variabele eerst aangemaakt moet hebben, voordat je de variabele kunt gebruiken. 
Als je bijvoorbeeld het printen van de variabele “spaarrekening” bovenaan het programma zet…
[korte pauze]
En het programma runt…
[runnen programma]


    print(spaarrekening)
    
    studiefinanciering = 277
    bijbaan = 600
    ouders = 200
    inkomsten = studiefinanciering + bijbaan
    
    huur = 390
    boodschappen = 225
    leuke_dingen = 150
    uitgaven = huur + boodschappen + leuke_dingen
    
    spaarrekening = uitgaven - inkomsten

… dan krijg je de error: “ name 'spaarrekening' is not defined”. 

Dit komt dus omdat je de variabele “spaarrekening” op regel 1 wilt printen, terwijl je deze variabele pas aan het einde van het programma aanmaakt.

## 3. if

In deze video leg ik uit hoe je gebruik kunt maken van if-statements. 

Stel je wil een programma schrijven dat een leeftijdscheck doet.

De eerste stap is om de gebruiker te vragen om een leeftijd, dus we gebruiken *input*: 
“leeftijd… is gelijk aan… input… leeftijd”.
De functie input geeft altijd een *string* als resultaat. 
Om een goede leeftijdscheck te doen moeten we eerst dit resultaat omzetten naar een integer. 
Dat gaat zo: “leeftijd… is gelijk aan… int… leeftijd”. 
Deze regel heeft dus als enige functie om het formaat van de invoer om te zetten naar een integer.
De invoer is nu klaar.
 
Dan wil je controleren of de leeftijd van de gebruiker kleiner is dan 18. 
Als dit het geval is dan wil je printen dat de gebruiker nog niet volwassen is.
Je kunt hiervoor een if-statement gebruiken. 
Dat ziet er als volgt uit: 
“als de leeftijd van de gebruiker kleiner is dan 18… print ‘je bent nog niet volwassen…”. 

Nu willen we ook iets printen als de gebruiker ***wel*** 18 jaar of ouder is. 
Je kunt dit doen door een “else”-statement toe te voegen. 
Dus als de leeftijd kleiner is dan 18, print “je bent nog niet volwassen…” 
en ***anders,*** print: “je bent volwassen!”.
Laten we het programma runnen…
[runnen programma]


    leeftijd = input("Leeftijd: ")
    leeftijd = int(leeftijd)
    
    if leeftijd < 18:
      print("Je bent nog niet volwassen...")
    else:
      print("Je bent volwassen!")

Als je nu 13 invult als leeftijd…
dan wordt gecontroleerd of 13 kleiner is dan 18,
en dat is zo,
dus dan print het programma “je bent nog niet volwassen”,

Als we het programma nog een keer runnen…
[runnen programma]
en 21 invullen als leeftijd…
dan wordt eerst gecontroleerd of 21 kleiner is dan 18…
dat is *niet* zo, en dus print het programma “je bent volwassen!”…
…het werkt! 

Je kunt dit programma uitbreiden met meer voorwaarden. 
We willen bijvoorbeeld ook onderscheid maken voor mensen die ouder zijn dan 65.
Dit doe je door een extra voorwaarde toe te voegen met een **elif** ofwel **else if**.
Dus: “als de leeftijd kleiner is dan 18… print ‘je bent nog niet volwassen’,
***anders als*** de leeftijd groter of gelijk is aan 65… print ‘je bent een senior!’
en ***anders*** print ‘je bent volwassen!’. 

Laten we het programma runnen…
[runnen programma]


    leeftijd = input("Leeftijd: ")
    leeftijd = int(leeftijd)
    
    if leeftijd < 18:
      print("Je bent nog niet volwassen...")
    elif leeftijd >= 65: 
      print("Je bent een senior!")
    else:
      print("Je bent volwassen!")

Als je nu 15 invult als leeftijd…
… dan print het programma “je bent nog niet volwassen”,
want 15 is kleiner dan 18.

[runnen programma]

en als je 71 invult als leeftijd…
… dan print het programma “je bent een senior!”…
want 71 is groter dan 65.

[runnen programma]

en als je 33 invult als leeftijd…
… dan print het programma “je bent volwassen!”
want 33 is niet kleiner dan 18, maar ***ook*** niet groter of gelijk aan 65. 
Dus het programma werkt opnieuw! 

Tot slot kun je ook meerdere voorwaarden combineren tot één.
Stel je krijgt korting op je toegangsticket bij een museum als je jonger dan 18 bent ***en ook*** ******als je 65 of ouder bent.
Dan ziet de combinatie van voorwaarden er zo uit:
“als de leeftijd kleiner is dan 18… 
***OF***… 
als de leeftijd groter of gelijk is aan 65…
print ‘je krijgt korting in het museum!’…
***anders***…
print ‘je krijgt helaas geen korting’…
dus één van deze voorwaarden moet waar zijn voordat ‘je krijgt korting’ wordt geprint. 

Laten we het programma runnen…
[runnen programma]


    leeftijd = input("Leeftijd: ")
    leeftijd = int(leeftijd)
    
    if leeftijd < 18 or leeftijd >= 65:
      print("Je krijgt korting in het museum!")
    else:
      print("Je krijgt helaas geen korting...")

Als je nu 17 invult als leeftijd…
… dan print het programma “je krijgt korting!”.
want 17 is kleiner dan 18. 

[runnen programma]

en als je 45 invult als leeftijd…
… dan print het programma “je krijgt helaas geen korting…”…
want 45 is en niet kleiner of gelijk aan 18 en niet groter of gelijk aan 65.

[runnen programma]

en als je 81 invult als leeftijd…
… dan print het programma weer “je krijgt korting!”
want 81 is groter dan 65. 

## 4. Loops

**Herhalen**
In deze video leg ik uit hoe je loops kunt gebruiken om stukjes code **herhaaldelijk** uit te voeren.  

Stel je wil de getallen 1 tot en met 10 uitprinten,  
dan kun je dit doen door tien losse print statements neer te zetten en te runnen. 
[kopieëren en plakken print statements en runnen]


    print("1")
    print("2")
    print("3")
    print("4")
    print("5")
    print("6")
    print("7")
    print("8")
    print("9")
    print("10")

Zoals je ziet worden de getallen 1 tot en met 10 geprint. 
Dit is alleen niet zo praktisch, want wat als je nu de getallen 1 tot en met 1000 wil printen?
Dan kun je een loop gebruiken.
Dat ziet er als volgt uit: “for… getal… in range… 1 **tot** 11… print getal”. 
Let op dat de range die je opgeeft 1 **tot** 11 is, en **niet** 1 tot en met 11. 

Als je dit programma runt dan zal de variabele “getal” eerst de waarde 1 aannemen.
Vervolgens wordt dit getal geprint. 
Daarna zal het programma terug gaan naar de beginregel bij “for”, 
en de variabele “getal” zal de waarde 2 aannemen. 
Dan wordt **dit** getal geprint. 
Dit zal herhaald worden tot 11, dus in totaal 10 keer. 
Laten we kijken of dit klopt… 
[runt programma]


    for getal in range(1, 11):
        print(getal)

… zoals je ziet worden inderdaad de getallen 1 tot en met 10 geprint. 

Je kunt met deze loop nu ook makkelijk de getallen 1 tot en met **1000** uitprinten.
Hiervoor moet je de 11 veranderen in 1001.
[runt programma]


    for getal in range(1, 1001):
        print(getal)

… en inderdaad, de getallen 1 tot en met 1000 worden geprint. 

Zo kun je elk aantal getallen printen dat je wilt met één enkele wijziging.

**Rekenen**
In deze video leg ik uit hoe je loops kunt gebruiken om **berekeningen** te doen.

Hoe kun je nou een loop gebruiken om een heleboel getallen op te tellen? 
Bijvoorbeeld de som van de getallen 1 tot en met 1000.

Met dit stukje code in de file rekenen.py kun je in ieder geval de getallen 1 tot en met 1000 printen:


    for getal in range(1, 1001):
      print(getal)

Om al deze getallen op te tellen, maak je eerst de variabele “som**”** aan met beginwaarde 0.
**In** de for-loop ga je dan de optelling doen.
Je wil de waarde die de variabele "getal” op dat moment heeft, optellen bij de waarde van de variabele “som”: “som = som + getal” … of de kortere notatie … “som += getal”. 
Onder de for-loop kun je de totaalsom printen… en dan ben je klaar.

Als je dit programma runt dan zal dus eerst de variabele “som” worden geïnitialiseerd met de waarde 0.
Vervolgens zal in de eerste stap de variabele “getal” de waarde 1 aannemen en worden opgeteld bij de waarde die de variabale “som” op dat moment heeft.
De waarde van de variabele “som” is 0, dus 0 + 1 is 1. 
Daarna zal het programma terug gaan naar de beginregel bij “for”. 
De variable “getal” zal nu de waarde 2 aannemen. 
De waarde van variabele “getal” wordt opnieuw opgeteld bij de waarde die de variabele “som” al had, dit is 1, dus 1 + 2 is 3. 
Dit zal herhaald worden tot de computer bij 1001 is, en daarna zal het resultaat worden geprint. 
Laten we het programma runnen… 
[runnen programma]


    som = 0
    for getal in range(1, 1001):
      som += getal
    print(som)

… zoals je ziet, de som van de getallen 1 tot en met 1000 is 500500. 

Door een simpele aanpassing in het programma zou je ook de som van andere getallen kunnen berekenen.  

**Filteren**
In deze video leg ik uit hoe je loops kunt gebruiken om te **filteren**.  

Stel je wilt de getallen die tussen de 1 en de 50 liggen **en** die deelbaar zijn door 3 printen. 
Dan heb je eerst een loop nodig die de getallen 1 tot en met 50 aftelt: “for getal… in range… 1 tot 51”. 
Vervolgens moet je checken of de waarde die de variabele “getal” op dat moment heeft deelbaar is door 3. 
Dit doe je met de modulo-operator, welke de rest van de deling van twee getallen geeft. 
Dus: “als de variabele ‘getal’… modulo 3… gelijk is aan 0… print getal”. 
Als de uitkomst van de variabele “getal”…modulo 3… gelijk is aan 0, dus rest 0, 
dan betekent dit dat de variabele “getal” deelbaar is door 3.  

Als je dit programma runt dan zal de variabele “getal” eerst de waarde 1 aannemen.
Vervolgens wordt gecontroleerd of de waarde van variabele “getal” modulo 3 gelijk is aan nul. 
Dit is niet het geval, want de uitkomst van 1 modulo 3 is 1, dus het getal 1 wordt niet geprint. 
Hierna gaat het programma terug naar de beginregel bij “for”.  
Vervolgens neemt de variabele “getal” de waarde 2 aan.
Dit getal wordt ook niet geprint, want de uitkomst van 2 modulo 3 is 2. 
Dan gaat het programma weer terug naar de beginregel bij “for” en neemt de variabele “getal” de waarde 3 aan. 
Dit getal wordt wel geprint, want de uitkomst van 3 modulo 3 is gelijk aan 0. 
Dit zal herhaald worden tot en met het getal 50. 
Laten we het programma runnen…
[runnen programma]


    for getal in range(1, 51):
      if getal % 3 == 0:
        print(getal)

… zoals je ziet worden onder andere de getallen 3, 6 en 9 uitgeprint, welke allemaal deelbaar zijn door 3. 

Door een simpele aanpassing in het programma zou je ook op andere voorwaarden getallen kunnen filteren. 

**Gebruikersinvoer**
In deze video leg ik uit hoe je gebruik kunt maken van loops om gebruikersinvoer op te vragen en te controleren.   

Je hebt een programma geschreven dat de naam van de gebruiker opvraagt en daarna Hallo en dan de naam van de gebruiker uitprint. 

Laten we het programma runnen om het te testen…
[runnen programma]


    naam = input("Wat is je naam? ")
    print("Hallo", naam)

… het programma vraagt om de naam van de gebruiker…
… en vervolgens print het programma Hallo ***Mirja***, dus dit werkt! 

Alleen als we het programma nu nog een keer runnen …
[runnen programma]
… en je vult **geen** naam in - wat niet de bedoeling is - dan wordt de rest van het programma **toch** uitgevoerd. 

Om ervoor te zorgen dat de gebruiker een geldige naam invult, 
kun je gebruik maken van een loop die herhaaldelijk de gebruiker om zijn of haar naam vraagt, totdat de gebruiker ***wel*** een valide naam invult. 
Je gebruikt hiervoor **geen** for-loop maar een while-loop, 
omdat je niet van te voren weet hoe vaak de gebruiker erover gaat doen om een valide naam in te vullen. 

Dus: “zolang de naam… is gelijk aan… een lege string….  vraag nog een keer de naam op”
Nu zal het programma iedere keer opnieuw de naam van de gebruiker vragen, zolang naam een lege string is. 
Laten we het programma runnen…
[runnen programma]


    naam = input("Wat is je naam? ")
    
    while naam == "":
      naam = input("Wat is je naam? ")
      
    print("Hallo", naam)

Als je nu geen naam invult, dan blijft het programma steeds opnieuw om je naam vragen. 
[aantal keer op enter drukken]
En als je wel je naam invult en op enter drukt, dan wordt net als eerder “Hallo ***Mirja***” geprint. 


## 5. Lijst

In deze video leg ik uit hoe je gebruik kunt maken van lijsten. 

Lijsten zijn handig om data te groeperen en vervolgens als geheel te verwerken. 
In een lijst kun je losse getallen opslaan, maar bijvoorbeeld ook strings. 
Denk aan een lijst met priemgetallen of een lijst met de namen van je studiegenoten. 
Het is zelfs mogelijk om lijsten in lijsten opslaan. 

Voor nu hebben we een boodschappenlijst gemaakt waar vijf items op staan: 
hummus, quinoa, knakworsten, puntpaprika en kokosmelk. 
We kunnen deze hele lijst printen door “print boodschappenlijst” te runnen…
[runnen programma]


    boodschappenlijst = ["hummus", "quinoa", "knakworsten", "puntpaprika", "kokosmelk"]
    print(boodschappenlijst)

… en zoals je ziet wordt inderdaad de hele lijst geprint. 

We kunnen ook één element van de lijst opvragen en uitprinten.
Daarvoor hebben we de ***positie*** nodig van dat element.
Als we het derde element van de lijst willen weten, 
dan kunnen we deze als volgt opvragen:
“print… boodschappenlijst… twee”.
Omdat een computer begint met tellen vanaf 0… 
zal “print boodschappenlijst twee” het derde element van de lijst printen.  

Laten we dit controleren…
[runnen programma]


    boodschappenlijst = ["hummus", "quinoa", "knakworsten", "puntpaprika", "kokosmelk"]
    print(boodschappenlijst[2])

… en inderdaad, het derde element in de lijst wordt geprint.

Je kunt elementen in een lijst ook wijzigen. 
Dit kan als volgt: “boodschappenlijst… twee… is… “kipknakworsten”” 
Als we het programma runnen…
[runnen programma]


    boodschappenlijst = ["hummus", "quinoa", "knakworsten", "puntpaprika", "kokosmelk"]
    boodschappenlijst[2] = "kipknakworsten"
    print(boodschappenlijst[2])

… dan zie je dat knakworsten inderdaad veranderd is naar kipknakworsten.                        

En we kunnen items aan de lijst toevoegen, bijvoorbeeld “kaas”. 
Dit doen we door eerst de naam van de lijst neer te zetten… dan een punt… append… kaas. 

Laten we de boodschappenlijst printen om dit te controleren…
[runnen programma]


    boodschappenlijst = ["hummus", "quinoa", "knakworsten", "puntpaprika", "kokosmelk"]
    boodschappenlijst.append("kaas")
    print(boodschappenlijst)

… en inderdaad, kaas is aan het einde van de lijst toegevoegd. 

Tot slot is het mogelijk om een lijst in een loop te gebruiken, bijvoorbeeld als we de boodschappenlijst netjes onder elkaar willen printen. 
Dat gaat zo:
“voor iedere item op de boodschappenlijst… print het item”. 

Als we dit runnen…
[runnen programma]


    boodschappenlijst = ["hummus", "quinoa", "knakworsten", "puntpaprika", "kokosmelk"]
    
    for item in boodschappenlijst:
        print(item)        

… dan worden inderdaad alle elementen van de lijst netjes leesbaar geprint. 


## 6. Functies

**Functies definiëren en aanroepen**
In deze video leg ik uit hoe je functies kan definiëren en aanroepen. 

Als je een stuk code meerdere keren nodig hebt in je programma, dan kun je het stuk in een functie plaatsen en de functie aanroepen op het moment dat je het nodig hebt. 
Hiermee voorkom dat je jezelf herhaalt, en je geschreven code wordt overzichtelijker en leesbaarder. 

In Python zijn al heel veel functies ingebouwd, bijvoorbeeld de functie “len”, 
waarmee je de lengte van een lijst kan op te vragen… 
of de functie “round”, 
waarmee je een getal op de wiskundig juiste manier kunt afronden. 

Naast deze ingebouwde functies kun je ook eigen functies maken in Python. 
Stel je hebt een programma geschreven dat… 

Je begint een functie met “def” en daarna de naam van de functie, welke je zelf kunt bepalen. 
Geef functies een korte, duidelijke en unieke naam, zodat het direct duidelijk is wat de functie doet en het niet conflicteert met iets anders in je code. 
Geïndenteerd is IN de functie, anders schrijf je code buiten de functie.
Deze regel sluit je af met een haakje openen en een haakje sluiten.
Funtie schrijven en runnen → er gebeurt niks 
functie moet nog gecalled worden
In feite gebruik je dus nu de naam van de functie, maar zet je er niet de bijbehorende code bij. 
Die is al vastgelegd bij de definitie.

**Functies met één parameter**
In deze video leg ik uit hoe je functies met één parameter kunt schrijven. 
~~~~
We schrijven een functie die het kwadraat van een willekeurig getal berekent.
We definieëren de functie door eerst “def” neer te zetten, 
gevolgd door de naam van de functie, in dit geval “kwadraat”.
De functie heeft één parameter, die we hier “x” noemen. 
~~~~De inhoud van de functie houden we simpel: 
het resultaat is X vermenigvuldigd met X… ofwel “return x… maal x”. 

Om te testen, roepen we de functie meteen even aan: “print kwadraat”… 
en runnen het programma…
[runnen programma]


    def kwadraat(x):
            return x * x
            
    print kwadraat()

Zoals je ziet krijgen we de error:  “missing 1 required positional argument: 'x' “
Dit komt omdat in onze test de functie geen parameter heeft meegekregen,
terwijl de functie wel een parameter nodig heeft, 
namelijk het getal waarvan we het kwadraat willen weten.
Laten we dus het getal 3 invullen op de plek van de parameter.
Nu wordt het kwadraat van drie berekend en de uitkomst geprint… 

[runnen programma] 


    def kwadraat(x):
            return x * x
            
    print kwadraat(3)

… dat klopt.

We kunnen ook een variabele als parameter meegeven aan de functie. 
We definieëren de variabele “getal” en geven deze de waarde 12.
Als we bij het aanroepen van de functie variabele “getal” opgeven, 
dan zal de parameter “x” de waarde van variabele “getal” aannemen, dus dat is 12.

Laten we het programma runnen…


    def kwadraat(x):
            return x * x
    
    getal = 12
    print kwadraat(getal)

… en inderdaad, 144 wordt geprint. 

**Functies met meerdere parameters**
In deze video leg ik uit hoe je functies met meerdere parameters kunt gebruiken. 

We schrijven een functie die twee getallen met elkaar vergelijkt en het *grootste* getal teruggeeft.
Je definieert de functie met “def” en geeft de functie een naam, bijvoorbeeld, “grootste_van”. 
De functie heeft twee parameters, namelijk de twee getallen die je met elkaar wil vergelijken: 
a en b. 
Je wil eerst controleren of parameter “a” groter is dan parameter “b”, 
dus: “als a is groter dan b”. 
Als dit het geval is dan, dan wil je parameter a returnen. 
En anders wil je parameter b returnen. 


    def grootste_van(a, b):
        if a > b:
           return a
        else:
           return b

Nu moet de functie nog getest worden. 
Eerst maken we twee variabelen aan, “getal 1” en “getal 2”, 
en die geven we allebei een waarde
Om de functie “grootste van” aan te roepen geven we de variabelen “getal 1” en “getal 2” mee aan de functie als parameters. 

Als je dit programma runt dan zal parameter “a” de waarde van variabele “getal 1” aannemen, 
dit is 126.
De parameter “b” zal de waarde van variabele “getal 2” aannemen, dit is 14. 
Vervolgens wordt in de functie gecontroleerd of parameter “a” groter is dan parameter “b”. 
Dit is het geval, want 126 is groter dan 14. 
Vervolgens wordt parameter “a” teruggegeven en geprint. 

Laten we het programma runnen… 
[runnen programma] 


    def grootste_van(a, b):
      if a > b:
         return a
      else:
         return b
    
    getal1 = 126
    getal2 = 14
    print(grootste_van(getal_1, getal_2))

… en inderdaad, het getal 126 wordt geprint.
~~~~
**Functies met lijsten**
In deze video leg ik uit hoe je functies met lijsten kunt gebruiken. 
~~~~
We schrijven een functie die een lijst met x-waardes aanneemt en een lijst teruggeeft waarin voor elke x-waarde de bijbehorende y-waarde is berekend. 

Bijvoorbeeld de volgende lijst.. “posities”


    # f(x) = x * x
    posities = [1, 2, 3, 4, 5, 6]

We definiëren een functie en we geven die de naam “lijst_kwadraat”
met één parameter “x_coords”, oftewel x_coordinaten.

Nu hebben we een lijst nodig om de resultaten in te verzamelen vóórdat we deze teruggeven.
 “y_coords… is … een lege lijst”. 
Vervolgens loopen we over de lijst met x-waarden: “voor iedere x… in de lijst… met x-coördinaten”. 
Dan berekenen we de y-waarde met onze functie x… maal x… 
en de uitkomst voegen we toe aan de lijst y_coords. 
Als alle berekeningen zijn gedaan en de lijst gevuld, returnen we ‘m.

Om de functie te testen gebruiken we die lijst “posities” die we al eerder hadden gemaakt. 
Dan roepen we onze functie lijst_kwadraat aan met posities als argument. 
En we printen het resultaat…

Laten we het programma runnen…
[runnen programma]


    def lijst_kwadraat(x_coords):
        y_coords = []
        for x in x_coords:
            y_coords.append(x * x)
        return y_coords
    
    posities = [1, 2, 3, 4, 5, 6]
    hoogtes = lijst_kwadraat(posities)
    print(hoogtes)

… en zoals je ziet wordt de lijst geprint met de kwadraten van elk getal. 

De lijsten samen zouden we kunnen gebruiken om de grafiek van x-kwadraat te plotten.


**Functies die functies aanroepen & functies aan functies meegeven**
In deze video leg ik uit hoe je functies in andere functies kunt aanroepen, 
en hoe je functies aan andere functies kunt meegeven. 

Laten we een programma schrijven dat het minimum berekent van een wiskundige functie, bijvoorbeeld “x kwadraat”, binnen een bepaald bereik.
De functie voor x-kwadraat hebben we al eerder geschreven.


    def kwadraat(x):
      return x ** 2

Voor het berekenen van het minimum maken we nu een aparte functie.
…bijvoorbeeld “minimum”. 
Deze functie krijgt twee parameters: de ondergrens en de bovengrens waarin we het minimum van de functie willen zoeken.
 
**In** de functie initialiseren we de variabele “minimum”. 
Een veilig startpunt is om de waarde van de functie op de ondergrens te nemen.
We roepen de functie “kwadraat” aan, die we al hadden geschreven: “minimum is gelijk aan… kwadraat bovengrens”. 
Je geeft de bovengrens dus mee als parameter aan de functie “kwadraat”. 
Vervolgens geeft de functie “kwadraat” het kwadraat van de ondergrens terug… 
en deze uitkomst wordt opgeslagen in de variabele “minimum”. 

Hierna ga je loopen binnen de opgegeven range om op zoek te gaan naar het minimum: 
“for x… in range… ondergrens plus 1… tot bovengrens”. 
Je loopt vanaf ondergrens **plus 1**, omdat je het kwadraat van de ondergrens zelf al opgeslagen hebt in de variabele “minimum”. 

X zal in de eerste loop dus de waarde van de ondergrens **plus 1** aannemen. 
Dan wil je controleren of het kwadraat van x kleiner is dan de waarde van de variabele “minimum”. 
Als dit het geval is, dan moet de variabele “minimum” gelijkgesteld worden aan het kwadraat van x. 
Dus: “als de uitkomst van de functie “kwadraat” kleiner is dan de variabele “minimum”, 
stel de variabele “minimum” gelijk aan de uitkomst van de functie “kwadraat” ”. 
Hier roep je dus opnieuw de functie “kwadraat” aan die je al eerder had geschreven en geeft hier x mee als parameter. 
Wanneer de loop klaar is maak je de functie af door de variabele “minimum” terug te geven: “return minimum”. 

Tot slot roep je de functie “bereken minimum” aan en je wilt het resultaat printen:
“print… bereken minimum…”. 
Als ondergrens geef je bijvoorbeeld -100 en als bovengrens 100 mee.

Laten we het programma runnen…
[runnen programma]


    def kwadraat(x):
      return x * x
      
    def minimum(ondergrens, bovengrens):
      resultaat = kwadraat(ondergrens)
      for x in range(ondergrens + 1, bovengrens):
          if kwadraat(x) < resultaat:
              resultaat = kwadraat(x)
      return resultaat
      
    print(minimum(-100, 100))

… en zoals je ziet is het minimum van de functie “x kwadraat” binnen de range -100 en 100 gelijk aan 0. 

Stel we willen nu van een andere wiskundige functie het minimum weten, dan zouden we een nieuwe “bereken minimum” functie kunnen schrijven, maar dit is onhandig. 
In plaats daarvan kun je ook de functie waarvan je het minimum wilt berekenen meegeven als parameter aan de functie “bereken minimum”. 
Je voegt dus een derde parameter “func” toe. 
Vervolgens moet je op de plekken waar je de functie “kwadraat” aanroept dit veranderen in het aanroepen van “func”, want de parameter “func” heeft meegekregen van welke functie je het minimum wilt berekenen.
[korte pauze]
Tot slot geef je bij het aanroepen van de functie “bereken minimum” aan van welke functie je het minimum wilt weten, in dit geval is dat de functie "kwadraat”.

Als we het programma nu runnen…
[runnen programma]


    def kwadraat(x):
      return x ** 2
    
    def bereken_minimum(func, ondergrens, bovengrens):
      minimum = func(ondergrens)
      for x in range(ondergrens + 1, bovengrens):
          if func(x) < minimum:
              minimum = func(x)
      return minimum
            
    print(bereken_minimum(kwadraat, -100, 100))

… dan zie je dat opnieuw 0 wordt geprint als minimum. 

Als je nu het minimum wilt weten van een andere functie…
bijvoorbeeld van “x tot de macht 3”…
dan hoeven we simpelweg alleen deze functie toe te voegen: 
“def macht drie… x… return x… tot de macht 3”.
En bij het aanroepen van de functie “bereken minimum” geef je niet de functie “kwadraat” als parameter mee, maar de functie “macht drie”. 

Laten we het programma runnen…
[runnen programma]


    def kwadraat(x):
      return x ** 2
    
    def macht_drie(x):
      return x ** 3
      
    def bereken_minimum(func, ondergrens, bovengrens):
      minimum = func(ondergrens)
      for x in range(ondergrens+ 1, bovengrens):
          if func(x) < minimum:
              minimum = func(x)
      return minimum
            
    print(bereken_minimum(macht_drie, -100, 100))

… en zoals je ziet is het minimum van de functie x tot de macht drie in de range -100 tot 100 gelijk aan -1.000.000. 

