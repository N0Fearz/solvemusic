### solvemusic
# Learning outcomes




# You design and build user-friendly, full-stack web applications
**Individueel**
- [Project description]()
For my individual project I am going to make an application which moves files and folders to given locations automatically, sort music by genre autoatically and show which genres there are. In the Issues i described all the things I want to add to this project. 

 - [Front-end]()
 For the front-end I have chosen to use react. This because its widely used in the world and it has a large community. Because of this it's eassier to find solutions for some problems that I may encounter during the proces of creating the application.<br />
 De git repository van de frontend: https://github.com/N0Fearz/frontend-solvemusic
 - [Back-end]()
 For the back-end of the application I chose to use Java, because it's a language that is commonly used in the software branch. Because I already have experienced working with C# I decided to work with Java so I can learn this language too. I will use microservices because i want to learn to work with that too. <br />
 de git repository van de backend: https://github.com/N0Fearz/backend-solvemusic 

**Groepsproject**

- [Project description]()
Tijdens het groepsproject hebben we de opdracht gekregen om een applicatie te maken waarbij een restaurant geautomatiseerd wordt. De klant wil dat er een applicatie wordt gemaakt waar het menu ingezien kan worden, welke de bestelling doorstuurt naar een andere applicatie die bedoeld is voor het keukenpersoneel. Hier verschijnen alle orders op die klaar gemaakt moeten worden. Verder moet er een applicatie gemaakt worden welke dient voor het barpersoneel. Drinken dat besteld wordt moet naar de bar gestuurd worden en eten naar de keuken.

 - [Front-end]()
De front-end applicaties gaan we maken in react. Dit omdat een aantal van ons ervaring heeft in react en react goede oplossingen biedt voor de problemen waar wij tegenaan lopen. Ook is het gebruikmaken van react een voordeel omdat er een grote community gebruik maakt van react.

 - [Back-end]()
Er is een back-end applicatie die gemaakt is in Java. Dit omdat er al wat ervaring met C# was in het groepje hebben we gekozen voor wat meer uitdaging met het leren van een nieuwe taal. Alle communicatie verloopt via de Java applicatie, zowel REST verzoeken als websockets.

# You use software tooling and methodology that continuously monitors and improve the software quality during software development.

 **Individueel project** 

In mijn individueel project heb ik meerdere dingen gedaan om de kwaliteit van mijn code te verbeteren en te monitoren. Ik heb de volgende tools gebruikt om mij hierbij te helpen en dit vast te leggen, namelijk:
 
 - SonarQube
 - SonarLint
 - Jenkins
 - Cypress e2e tests
 - JUnit unit tests

 Voor het bouwen van mijn projecten maak ik gebruik van Jenkins. Dit is een CI/CD programma waarmee software gebouwd kan worden maar ook getest kan worden. Tijdens het bouwen van een project wordt er gekeken of er fouten zijn in het bouw proces. Als dit niet het geval is dan wordt de volgende stap in het proces gezet en dat is het uitvoeren van de tests. Als deze testen niet falen zal de code doorgestuurd worden naar SonarQube waar deze een volledige code scan ondergaat. Hier komt een raport uit, als de code niet voldoet aan de eisen die ik ingesteld heb, zal Jenkins een seintje krijgen en de pipeline afkeuren. Hierdoor is er een proces ontstaan waarbij er meer garantie is op een applicatie die goed werkt en niet zal falen.

 Tot nu toe heb ik alleen bij de Backend, welke gemaakt is in Java, een SonarQube project draaien welke van begin tot eind afgewerkt wordt. Voor de frontend gebruik ik de ingebouwde lint die de code controleert tijdens het bouwen van de applicatie en hier meldingen van geeft waar de code niet goed is. Mochten er grote gebreken zijn wordt ook hier de pipeline afgekeurd en zal deze niet afronden. Tijdens het bouwen van het project wordt de applicatie gestart en wordt deze geverifieerd door Cypress. Als de applicatie opgestart is wordt de volgende stap gestart. Hier wordt de End to End test, gemaakt in Cypress gestart. Deze zal alle tests doorlopen. Mocht er een test falen, wordt ook hier de pipeline afgekeurd. Er wordt een video gemaakt van de test welke ik kan terug kijken om te zien wat de test doet en of deze wel goed werkt.

 De eerste code-scan waren er een aantal code smells aanwezig, zoals te zien op de afbeelding hieronder:
 
 ![code fails 21 nov](https://user-images.githubusercontent.com/55428530/206020294-f3ff6ea8-6358-4dbc-b559-cb3c8cb2ca46.PNG)


 De tweede code-scan had een aantal code-smells meer. Dit komt doordat nog niet alle code was gepusht naar de master branch.
 
![code fails 23 nov](https://user-images.githubusercontent.com/55428530/206020330-422de697-c8cf-4059-a1a4-3a88ddb6df4a.PNG)

 De derde code-scan had er geen meer, hier heb ik alle fouten opgelost. De SonarQube geeft wel aan dat ik dedupliceerde code heb, hiervoor heb ik aangegeven dat dit genegeerd kan worden omdat dit voor foutmeldingen gaat in 2 verschillende projecten is dit hetzelfde.
 
 ![code success 23 nov](https://user-images.githubusercontent.com/55428530/206020396-df7050c5-a532-4c00-9643-39f62e2288df.PNG)


**Groepsproject**

in het groepsproject heb ik een aantal dingen gebruikt om de continuously integration en monitoring toe te passen, namelijk:

- Github Actions
- Docker

Wanneer een push event plaatsvind op de main branch, zal Github Actions de applicatie bouwen en op basis van die build een docker image maken. Deze wordt naar docker.io gepusht en kan vervolgens door de live omgeving opgehaald worden. In Azure heb ik een omgeving aangemaakt met een linux server waar de backend applicatie draait in een docker container. Op het moment dat Github Actions aangeeft dat er een nieuwe versie beschikbaar is, zal azure deze van docker.io af halen en een nieuwe container starten op de live omgeving.

Ditzelfde geldt voor de frontend, welke niet op azure staat maar op vercel.


# You choose and implement the most suitable agile software development method for your software project.

Gedurende dit semester wordt er van de ons als studenten verwacht dat wij één van de agile manieren vinden waarop we werken.

**Wat is agile?**

Agile is een iteratieve benadering van het managen van projecten en ontwikkelen van software. Het idee van agile is dat er in plaats van een hele applicatie op wordt geleverd, een klein deel van de applicatie wordt opgeleverd. Hierdoor kan er door de klant continu feedback gegeven worden en kunnen er vrijwel direct veranderingen doorgevoerd worden.
 
 
Het agile manifest is in begin jaren 2000 opgericht samen met alle sleutelfiguren van de 'lichtgewicht' methoden en hun doelstelling was om op zoek te gaan naar gemeenschappelijke inzichten die zich tegen het traditionele softwareontwikkeling keerden. Deze groep mensen hebben het voor elkaar gekregen om het Agile Manifest te formuleren. Verder in het dit onderzoek heb ik de waardes en principes waar dit manifest uit bestaat geschreven.

 ![image](https://user-images.githubusercontent.com/55428530/196798478-f5067dc6-e8c5-4064-aef1-e5029548b4f0.png)

 De waardes van de het Agile Manifest:
- Mensen en hun onderlinge interactie boven processen en hulpmiddelen.
- Opgeleverde deelprojecten boven allesomvattende documentatie of plannen.
- Samenwerking met de klant boven contractonderhandelingen.
- Inspelen op verandering boven het volgen van een plan.

Agile is een manier van werken. Hier horen ook een aantal principes bij welke gelden voor het werken met Agile. Hieronder zal ik er een aantal noemen:
- De hoogste prioriteit is het tevreden stellen van klanten door het vroegtijdig en voortdurend opleveren van producten.
- De mogelijkheid van veranderde behoeftes, zelfs laat in het ontwikkelproces.
- Teams reflecteren hoe ze nog effectiever kunnen werken en passen hier hun gedrag op aan.
- Lever regelmatig werken producten op. Iedere paar weken het liefst, hooguit iedere paar maanden.

**Welke methodes zijn er?**

**Scrum**:
Scrum is een methode waar bedrijven gebruik van maken met zelforganiserende teams. Iedereen heeft een eigen rol binnen een team. Elke dag wordt er een korte meeting gehouden waarin er een review over het proces wordt gedaan. De verschillende rollen zijn 
-	Ontwikkelteam
-	Product owner
-	Scrum master
-	Stakeholder

Bij de scrum methode wordt er in sprints gewerkt. Na de sprint periode word het product opgeleverd en vervolgens een review met de stakeholder gehouden om aan te geven hoe het gegaan is en hoe het de volgende sprint opgepakt of wat er veranderd moet worden. Daarna zal er een retrospective plaatsvinden waarin het team overlegd wat er moet veranderen om zo effectief mogelijk te blijven.

**Lean:**
Lean is een managementfilosofie dat gericht is op het maximaliseren van de waarde voor de klant met zo min mogelijk verspillingen. Lean is oorspronkelijk gebaseerd op een proces ontwikkeld door Toyota. Door gebruik te maken van de lean methode werd elke actie die niet bijdroeg aan het productieproces verwijderd. Hierdoor werden er minder middelen en tijd verspild. Lean heeft 5 principes:
- Value: Weet wat klanten willen betalen
- Value stream mapping: Het in kaart brengen van het proces, de stappen of de volgorde die een product of dienst doorloopt in een bedrijf.
- Flow: Zorgen dat product- en informatie verzoeken zonder slag of stoot door het proces kunnen gaan.
- Pull: Alleen materiaal vervangen dat wordt gebruikt en het elimineren van overtollige voorraad waardoor er snel gereageerd kan worden op deeisen van de klant.
- Strive for perfection: altijd streven om het proces zo efficient mogelijk te maken en de waarde verbeteren dat geleverd wordt aan de klant.

**Kanban:**
Het doel van kanban is om op een efficiënte manier een product produceren. Het proces wordt doormiddel van de kanban methode visueel gemaakt door gebruik te maken van een Kanbanbord. Het proces wordt vaak gevisualiseerd in 3 categoriën, namelijk to-do, doing en done. Bij complexere processen kunnen meerdere categorieën gevisualiseerd worden om knelpunten te identificeren.

**Welke Methode zal ik gebruiken en waarom:**

Tijdens het groepsproject gebruiken we Scrum. Dit omdat Scrum een methode is wat fijn is om te werken in groepsverband en voor de klant waarmee we werken is dit ook een voordeel. Waaromm? De klant kan na een sprint van 3 weken aangeven dat er iets anders moet. Hierdoor zijn we erg flexibel en  staan de wensen van de klant op 1. Verder hebben we na elke sprint een retrospective waarin we veranderingen kunnen aangeven of juist niet als het proces goed verloopt.

Een ander voordeel aan scrum is dat wij elke ochtend een stand-up houden om te weten waar iedereen gebleven is, waar de knelpunten zitten en hoe de voortgang is. Hierdoor weten we waar er verbeterd moet worden of waar er goed gewerkt wordt. Ook kan er hier meteen ideeën voor eventuele knelpunten besproken worden.

Na elke sprint houden we een retrospective om de sprint daarvoor te evolueren. Hierdoor blijven we aanpassen aan de wensen van de klant en zelf een zo efficiënt mogelijk team. Zo heeft onze klant altijd een effectief en effiënt team wat voor hen werkt en kunnen zij aanpassingen aanvragen wanneer zij willen. Ook hebben we een dashboard aangemaakt in Jira waar we de sprintplanning in maken en bijhouden. Dat ziet er uit zoals in de afbeelding hieronder.

Ook maken we gebruik van Epics. Een Epic is een taak die te groot is om in een keer uit te voeren is. In dit geval hebben we ervoor gezorgd dat we de Epics hebben opgedeeld in user stories. Een user story hoort dus bij een Epic.

![jiraboard](https://user-images.githubusercontent.com/55428530/207855516-6698996b-bcf2-4745-a5f7-0a969aa4824c.png)

Ook maken we gebruik van een tijdschema zodat we kunnen zien wie waar mee bezig is geweest en hoelang dat per issue geduurt heeft.

![image](https://user-images.githubusercontent.com/55428530/207856177-09a31132-4320-463c-88f0-805f71e2fca4.png)

![image](https://user-images.githubusercontent.com/55428530/207856387-34472ae4-7c54-4d71-b9d2-0ba8ca5c27b3.png)

Na elke sprint doen we met het projectgroepje een retrospective waar ook de docent bij zat om de sprint te beoordelen. Hier kan iedereen aangeven wat er goed is gegaan, wat er minder goed is gegaan en wat we de volgende keer anders moeten doen.

![image](https://user-images.githubusercontent.com/55428530/207856816-94a1aa87-e904-4395-a241-61aad09349b5.png)

Hieronder is te zien hoe de acties worden beschreven welke wij voor de volgende sprint doen implementeren.

![image](https://user-images.githubusercontent.com/55428530/207856912-45bbc641-8060-4a01-856c-23b57db2d32c.png)


# You design and implement a (semi)automated software release process that matches the needs of the project context. (CI/CD)

Zoals ik in een hoofdstuk hierboven al wat heb toegelicht heb ik met twee soorten tools gewerkt om een proces te maken waarbij software automatisch gereleased wordt.

de tools:

- Jenkins
- Github Actions

**Individueel project**

Voor mijn individueelproject heb ik gebruik gemaakt van Jenkins. Jenkins is een open source server waarmee software mee gebouwd en uitgerold kan worden. Ik heb hier voor gekozen omdat ik gebruik maak van SonarQube en deze op mijn lokaal netwerk geïnstalleerd is. Wegens security overwegingen doe ik geen poorten open zetten om van buiten het netwerk deze te kunnen bereiken. Er is een tool waar ik gebruik van maak om het mogelijk te maken om Jenkins en github te laten communiceren zonder dat ik hier mijn netwerk voor open hoef te zetten. Deze tool heet smee.io en deze is verbonden met Github. Op het moment dat Github een push event ontvangen heeft, wordt er een webhook geactiveerd welke een sein stuurt naar de door mij aangemaakte URL in smee.io. Jenkins luistert continu naar de smee.io link en op het moment dat er een melding open staat zal Jenkins de juiste repository van Github halen en de master branch bouwen. Hier worden ook de tests en kwaliteit scans uitgevoerd. Op het moment dat de build faalt zal er een kruis op het dashboard van Jenkins te zien zijn en als deze successvol voltooid zal er een vink staan.

![Jenkins screenshot](https://user-images.githubusercontent.com/55428530/206020813-b62e1895-3155-4c55-9a9b-5661f95975fd.png)


**Groepsproject**

In het groepsproject heb ik gebruik gemaakt van Github Actions. Dit omdat alles dan op een plaats geregeld wordt, wat voor de rest van de groep fijn is zodat zij ook in de gaten kunnen houden of de build slaagd of faalt. Ook heb ik gezorgd dat het project in een docker container draait. Hierdoor kan er op elke omgeving het project gedraaid worden waardoor we zeker weten dat de applicatie op elk systeem draait. De docker image wordt gemaakt in tijdens de job in Github Actions en wordt vervolgens naar dockerhub gestuurd. Op het moment dat het bouwen van de applicatie succesvol is afgerond zal deze op de live omgeving gezet worden waar vervolgens de nieuwste versie van de applicatie zal draaien.

# You recognize and take into account cultural differences between project stakeholders and ethical aspects in software development.

**Wat is cultuur?**

Een systeem van afspraken dat beschrijft hoe mensen in een samenleving zich gedragen. Het wordt ook wel een manier van leven genoemd. Dit geldt per samenleving en is per samenleving anders. Mensen van verschillende culturen zien dingen anders of plaatsen dingen in een ander perspectief, hierdoor is communiceren ooit moeilijker dan met mensen uit dezelfde cultuur.

**Wat zijn bekende dimensies van culturele verschillen?**
-	Machtsafstand
Dit houdt in hoe een samenleving omgaat met ongelijkheid.

-	Masculiniteit/feminiteit
Mensen die feminien denken vinden relaties en levenskwaliteit belangrijk, werken om te leven. Mensen die masculien denken vinden uitdaging, salaris, erkenning en promotie belangrijk. 

-	Termijn denken
In culturen is er verschil in kortetermijngerichtheid en langetermijngerichtheid. 
Bij korte termijn vinden mensen het belangrijk dat tradities gerespecteerd moeten worden en dat sociale verplichtingen voldaan moeten worden.

In cultuur met lange termijn vinden ze het belangrijk om te streven naar beloning voor de toekomst en zijn zij spaarzaam en vasthoudend.

-	Onzekerheidsvermijding:
Dit houdt in hoe mensen handelen in onbekende situaties. Ook licht het hier aan hoe gelukkig mensen zijn en hoe zij zorgen voor gezondheid.

-	Individualisme:
in deze dimensie wordt er gerefereerd naar hoe mensen zichzelf zien in relatie met anderen. Als mensen meer individueel denken zullen zij eerder zichzelf vooropzetten dan een groep mensen. Het tegenovergestelde geldt voor collectivisme.


**Culturele verschillen die ik heb meegemaakt:**

Ik heb familie wonen in België. Mijn tante is Nederlands maar haar kinderen zitten in België op school waardoor zij wel de Belgische cultuur hebben overgenomen. Wat ik merk is dat wij veel directer zijn in het communiceren. Hierdoor denken zij dat wij Nederlanders brutaal zijn en wij denken dat zij heel zachtaardig zijn. Wat ik ook merk is dat zij onderdanig zijn, aangezien als iemand iets verteld dat zij moeten doen zullen zij niet snel een weerwoord hebben in tegenstelling tot Nederlanders die dat wel doen.

**Mijn cultuur**

Mijn cultuur is de Nederlandse cultuur, waar ik geboren en getogen ben.


# You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using multiple types of test techniques.

**Individueel**

Tijdens het maken van de applicatie heb ik een aantal requirements opgesteld. Deze requirements heb ik opgesteld op basis van user stories. Deze heb ik beschreven in de issues van mijn github repository. Ik ben begonnen met het uitwerken van één user story, hierbij heb ik rekening gehouden met wat de user story precies inhoudt. Hiervoor heb ik een klein architectuur design gemaakt wat mij verduidelijkt hoe ik de applicatie wil laten werken. Ook heb ik een simpel wireframe design gemaakt hoe een pagina er uit moet zien.

![Figma screenshot](https://user-images.githubusercontent.com/55428530/206020768-beffa0a2-2111-44aa-a823-9337bf0d3c28.png)

Ook heb ik gebruik gemaakt van een zelfgeschreven UI test om te zien of data wel gevalideerd wordt. Hierdoor weet ik zeker dat ik de data in goede vorm binnen krijg.

![image](https://user-images.githubusercontent.com/55428530/206414861-d2694a6e-8c87-40e2-8aef-252a8818d825.png)

Zoals hieronder te zien is heb ik een C4 model level 2 gemaakt om globaal te zien hoe mijn applicatie met elkaar zal werken. Ik heb gekozen voor microservices, dit heb ik verder toegelicht in mijn onderzoek.

![image](https://user-images.githubusercontent.com/55428530/206425773-e20e3685-48d4-4d3a-b6bf-2562935ebb74.png)

**Groepsproject**

Voor het groepsproject hebben we requirements gekregen van de klant welke wij uit hebben geschreven in epics en user stories. In ons dashboard op Jira zijn de uitgewerkte requirements te zien. Om dit project te kunnen maken hebben we een architectuurdesign gemaakt en designs voor de front-end. Hieronder zijn deze te zien:

c4 model:

![c4 model groeps](https://user-images.githubusercontent.com/55428530/207858754-f892aeee-3864-43ad-a12b-4eaa81ca9787.png)

design front-end:

![Artboard 1](https://user-images.githubusercontent.com/55428530/207859506-e5050615-8b2c-496f-a4dc-415d6a9429ec.png)


# You analyze and describe simple business processes that are related to your project.

Tijdens het groepsproject heb ik twee businessprocessen gemaakt. De klant vroeg om een managementtool waarmee de voorraad en boekhouding mee bijgehouden kon worden. Er is geen tijd over om deze tool te maken maar ik heb er alsnog een businessproces van gemaakt om aan te geven waar winst wordt behaald op het moment dat de tool gebruikt gaat worden. 

Op het bovenste proces in de afbeelding hieronder is het proces te zien met de app. Zoals te zien is kan door het digitaliseren van het berekenen van de voorraad constant de voorraad berekend worden. In het proces daaronder is te zien dat dit altijd handmatig gedaan moet worden omdat de bestellingen niet digitaal vastgelegd worden.

In de onderste proces is te zien er een dag maand of weekstaat uitgredraaid kan worden door het systeem, terwijl dit zonder digitaal systeem handmatig gedaan moet worden. Alle bonnetjes moeten elke dag opgeteld worden waar uiteindelijk een maandstaat uit voort komt, terwijl het systeem dit automatisch doet. 

![image](https://user-images.githubusercontent.com/55428530/209165883-1fd3a00c-efc3-4c15-af2c-79b9ffe0dd7d.png)

# You act in a professional manner during software development and learning.

Ik heb meerdere keren om feedback gevraagd bij beide docenten om te weten of ik de goede richting in ga. Ik stuur bij waar nodig om zo dit semester zo goed als mogelijk af te kunnen ronden.
