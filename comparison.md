# Voorstel sjabloon voor principes in Leidraad verantwoorde softwareontwikkeling

Dit is een voorstel voor een sjabloon voor het beschrijven van de onderdelen (in de betaversie principes genoemd) van de Leidraad verantwoorde softwareontwikkeling. Daartoe bespreekt deze memo een aantal andere kaders op het gebied van softwareontwikkeling, geeft overwegingen en doet een concreet voorstel met een voorbeeld.

## Prior art

### Huidige indeling Leidraad verantwoorde softwareontwikkeling

De beta “Leidraad verantwoorde softwareontwikkeling” op developer.overheid.nl bevat 13 principes. De beschrijving van de principes kent één kopje dat gedeeld is tussen alle principes, namelijk “Belangrijke redenen”. Er zijn daarnaast nog een aantal algemene kopjes die bij meerdere (maar niet alle) principes terugkomen: “Communities”, “Standaarden”, “Bronnen”. Andere kopjes komen maar bij één principe voor, zoals “User stories”, “Personas”, “Monitoring met OpenKAT” en “Hoe word je AVG-compliant?”.

De kopjes die meer dan één keer voorkomen hebben een verschillend karakter. Sommigen zijn tools (OpenKAT, Quality-time), sommigen zijn methoden en/of technieken (User stories, Persona’s), anderen hebben weer meer het karakter van een standaard (NPR 5326, DCAT) of lijken meer een principe (Data bij de bron).

Wat verder ook opvalt is dat de principes vrij consequent in de imperatieve vorm zijn geschreven (“Werk …”, “Maak …”, “Wees …”). Een uitzondering is “Cloud-native softwareontwikkeling”. Echter, de uitwerking van de principes is niet zo duidelijk in de gebiedende wijs.

### Nederlandse Richtlijn Digitale Systemen

NeRDS kent een consistentere indeling. De 14 richtlijnen hebben allemaal kopjes voor “Waarom is het belangrijk?”, “Hoe pas je het toe?”, “Gerelateerde hulpmiddelen” en/of “Gerelateerde standaarden” en “Gerelateerde richtlijnen”. Opvallend is dat het lijstje met richtlijnen grotendeels overlapt met de leidraad verantwoorde softwareontwikkeling, maar dat het in de leidraad dus principes zijn en geen richtlijnen.

Opvallend aan NeRDS is verder dat de uitwerkingen van de richtlijnen veel lijstjes met korte bullet points bevatten.

### ICTU Kwaliteitsaanpak Softwareontwikkeling

De ICTU Kwaliteitsaanpak Softwareontwikkeling beschrijft maatregelen die ICTU en ICTU-projecten nemen om de kwaliteit van de software te waarborgen. De maatregelen hebben allemaal een rationale, maar verder geen vaste onderverdeling.

### NPR 5326 Risicobeheersing bij ontwikkeling en onderhoud van maatwerksoftware

De NPR 5326 beschrijft risico’s en beheersmaatregelen bij de ontwikkeling en het onderhoud van maatwerksoftware. De risico’s en beheersmaatregelen zijn niet onderverdeeld volgens een vaste structuur, behalve dat de beheersmaatregelen expliciet verwijzen naar de risico’s die ze zouden moeten verminderen.

### The Technology Code of Practice (GOV.UK)

De TCoP is “a set of criteria to help government design, build and buy technology”. Het is de basis voor NeRDS en de beta-richtlijn verantwoorde softwareontwikkeling. De onderdelen heten hier “points”. De points hebben als vaste onderdelen: “How the (point) will help your programme” en “Related guides”.

### Capability Maturity Model Integrated

Het CMMI is inmiddels versie 3.0 en achter een pay-wall. Als we kijken naar indeling van procesgebieden in versie 1.2 zien we de volgende onderdelen: doelen, werkwijzen (practices), subwerkwijzen (subpractices) en typische werkproducten. CMMI maakt daarbij onderscheid tussen processpecifieke doelen en werkwijzen en generieke doelen en werkwijzen. Processpecifeke doelen en werkwijzen zijn specifiek voor een procesgebied. Een processpecifiek doel van het procesgebied Process and Product Quality Assurance is bijvoorbeeld “Objectively Evaluate Processes and Work Products”. Generieke doelen zijn van toepassing op alle procesgebieden. Een generiek doel is bijvoorbeeld: “Institutionalize a Managed Process”.

ISO 15288 Systems and software engineering — System life cycle processes en ISO 12207 Systems and software engineering – Software life cycle processes

Beide ISO-standaarden 15288 en 12207 beschrijven processen voor de systeem-, respectievelijk de software life cycle. De processen worden beschreven in termen van doel, resultaten, activiteiten en taken.

## Overwegingen

Gegeven dat het doel is om een richtlijn te maken voor verantwoorde softwareontwikkeling, ligt het voor de hand dat de richtlijn voorschrijft welke activiteiten nodig zijn om op verantwoorde wijze software te ontwikkelen. En daarbij ook duidelijk maakt wat de ondergrens is om nog van verantwoorde softwareontwikkeling te spreken. Dat zou je ook weer een richtlijnen kunnen noemen. Bij elke activiteit zou eigenlijk moeten gelden dat het niet uitvoeren van de activiteit leidt tot onverantwoorde softwareontwikkeling.

De huidige versie heeft het over principes. Die zouden dus vervangen worden door richtlijnen (vergelijkbaar met NeRDS).

Omdat de richtlijn zelf ook weer uit richtlijnen bestaat krijgen we dus een boom van richtlijnen die zegt: om verantwoord software te ontwikkelen dien je A, B en C te doen. Om verantwoord A te doen, dien je A1, A2 en A3 te doen, etc. Voor de overzichtelijkheid zullen we dit waarschijnlijk tot maximaal twee niveaus willen beperken.