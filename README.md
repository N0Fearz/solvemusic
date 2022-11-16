### solvemusic

# Learning outcomes

1. [You design and build user-friendly, full-stack web applications]()
- [Project description]()<br />
For my individual project I am going to make an application which moves files and folders to given locations automatically, sort music by genre autoatically and show which genres there are. 

 - [Front-end]()<br />
 For the front-end I have chosen to use react. This because its widely used in the world and it has a large community. Because of this it's eassier to find solutions for some problems that I may encounter during the proces of creating the application.<br />
 De git repository van de frontend: https://github.com/N0Fearz/frontend-solvemusic<br />
 - [Back-end]()<br />
 For the back-end of the application I chose to use Java, because it's a language that is commonly used in the software branch. Because I already have experienced working with C# I decided to work with Java so I can learn this language too. I will use microservices because i want to learn to work with that too. <br />
 de git repository van de backend: https://github.com/N0Fearz/backend-solvemusic <br />
2. [You use software tooling and methodology that continuously monitors and improve the software quality during software development.]()<br />

3. [You choose and implement the most suitable agile software development method for your software project.]()<br />
Gedurende dit semester wordt er van de ons als studenten verwacht dat wij één van de agile manieren vinden waarop we werken.<br />
Wat is agile?<br />
Agile is een iteratieve benadering van het managen van projecten en ontwikkelen van software. Het idee van agile is dat er in plaats van een hele applicatie op wordt geleverd, een klein deel van de applicatie wordt opgeleverd. Hierdoor kan er door de klant continu feedback gegeven worden en kunnen er vrijwel direct veranderingen doorgevoerd worden.
<br />

Het agile manifest is in begin jaren 2000 opgericht samen met alle sleutelfiguren van de 'lichtgewicht' methoden en hun doelstelling was om op zoek te gaan naar gemeenschappelijke inzichten die zich tegen het traditionele softwareontwikkeling keerden. Deze groep mensen hebben het voor elkaar gekregen om het Agile Manifest te formuleren. Verder in het dit onderzoek heb ik de waardes en principes waar dit manifest uit bestaat geschreven.

 ![image](https://user-images.githubusercontent.com/55428530/196798478-f5067dc6-e8c5-4064-aef1-e5029548b4f0.png)<br /> <br />
 
De waardes van de het Agile Manifest:<br />
- Mensen en hun onderlinge interactie boven processen en hulpmiddelen.
- Opgeleverde deelprojecten boven allesomvattende documentatie of plannen.
- Samenwerking met de klant boven contractonderhandelingen.
- Inspelen op verandering boven het volgen van een plan.
<br />

Agile is een manier van werken. Hier horen ook een aantal principes bij welke gelden voor het werken met Agile. Hieronder zal ik er een aantal noemen:<br />
- De hoogste prioriteit is het tevreden stellen van klanten door het vroegtijdig en voortdurend opleveren van producten.
- De mogelijkheid van veranderde behoeftes, zelfs laat in het ontwikkelproces.
- Teams reflecteren hoe ze nog effectiever kunnen werken en passen hier hun gedrag op aan.
- Lever regelmatig werken producten op. Iedere paar weken het liefst, hooguit iedere paar maanden.
 <br />
 
Welke methodes zijn er?<br /><br />
Scrum:<br />
Scrum is een methode waar bedrijven gebruik van maken met zelforganiserende teams. Iedereen heeft een eigen rol binnen een team. Elke dag wordt er een korte meeting gehouden waarin er een review over het proces wordt gedaan. De verschillende rollen zijn 
-	Ontwikkelteam
-	Product owner
-	Scrum master
-	Stakeholder
<br />
Bij de scrum methode wordt er in sprints gewerkt. Na de sprint periode word het product opgeleverd en vervolgens een review met de stakeholder gehouden om aan te geven hoe het gegaan is en hoe het de volgende sprint opgepakt of wat er veranderd moet worden. Daarna zal er een retrospective plaatsvinden waarin het team overlegd wat er moet veranderen om zo effectief mogelijk te blijven.

<br />

Lean:<br />
Lean is een managementfilosofie dat gericht is op het maximaliseren van de waarde voor de klant met zo min mogelijk verspillingen. Lean is oorspronkelijk gebaseerd op een proces ontwikkeld door Toyota. Door gebruik te maken van de lean methode werd elke actie die niet bijdroeg aan het productieproces verwijderd. Hierdoor werden er minder middelen en tijd verspild. Lean heeft 5 principes:
- Value: Weet wat klanten willen betalen
- Value stream mapping: Het in kaart brengen van het proces, de stappen of de volgorde die een product of dienst doorloopt in een bedrijf.
- Flow: Zorgen dat product- en informatie verzoeken zonder slag of stoot door het proces kunnen gaan.
- Pull: Alleen materiaal vervangen dat wordt gebruikt en het elimineren van overtollige voorraad waardoor er snel gereageerd kan worden op deeisen van de klant.
- Strive for perfection: altijd streven om het proces zo efficient mogelijk te maken en de waarde verbeteren dat geleverd wordt aan de klant.


Kanban:<br />
Het doel van kanban is om op een efficiënte manier een product produceren. Het proces wordt doormiddel van de kanban methode visueel gemaakt door gebruik te maken van een Kanbanbord. Het proces wordt vaak gevisualiseerd in 3 categoriën, namelijk to-do, doing en done. Bij complexere processen kunnen meerdere categorieën gevisualiseerd worden om knelpunten te identificeren.<br /><br />

Welke Methode zal ik gebruiken en waarom:<br />
Tijdens het groepsproject gebruiken we Scrum. Dit omdat Scrum een methode is wat fijn is om te werken in groepsverband en voor de klant waarmee we werken is dit ook een voordeel. Waaromm? De klant kan na een sprint van 3 weken aangeven dat er iets anders moet. Hierdoor zijn we erg flexibel en  staan de wensen van de klant op 1. Verder hebben we na elke sprint een retrospective waarin we veranderingen kunnen aangeven of juist niet als het proces goed verloopt.

<br />

[Agile Manifesto](https://www.sixsigma.nl/artikelen/agile-manifesto)<br />
[Wat is Agile](https://www.sixsigma.nl/wat-is-agile)<br />
[Wat is Scrum](https://www.scrum.org/resources/what-is-scrum)<br />
[Wat is Lean](https://leanmethods.com/resources/articles/what-is-lean/)<br />
[Wat is KanBan](https://www.atlassian.com/agile/kanban)<br />

4. [You design and implement a (semi)automated software release process that matches the needs of the project context. (CI/CD)]()<br />
In het groepsproject hebben we CI/CD toegepast. Dit hebben we gedaan doormiddel van Github actions en docker. De backend is geschreven in Java, waar een docker image van gemaakt is. Deze wordt door de github actions workflow gebuild waarna deze naar een azure omgeving wordt gepusht. deze implememteerd de image waarna de omgeving vrijwel meteen live staat met de nieuwe versie.<br />
5. [You recognize and take into account cultural differences between project stakeholders and ethical aspects in software development.]()

6. [You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using multiple types of test techniques.]()

7. [You analyze and describe simple business processes that are related to your project.]()

8. [You act in a professional manner during software development and learning.]()<br />
I have asked multiple times for feedback making sure I am going the right direction with the project.
