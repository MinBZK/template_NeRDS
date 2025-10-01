# NeRDS Template v0.1.0

## Introductie

Dit document beschrijft de template voor NeRDS (Nederlandse Richtlijnen Digitale Systemen) richtlijnen. Deze template biedt een gestandaardiseerde structuur voor het documenteren van richtlijnen voor digitale systemen binnen de Nederlandse overheid.

## Specificatie van de Template

### Richtlijn Structuur

Een NeRDS richtlijn bestaat uit de volgende onderdelen:

#### 1. Richtlijn Titel
Titel van de richtlijn

#### 2. Beschrijving (Wat)
Beschrijving van de richtlijn en de belangrijkste termen daarin

#### 3. Rationale (Waarom)
- Waarom is deze richtlijn een goed idee
- Welk effect beoogt de richtlijn te bereiken
- Risico's bij niet-toepassen

#### 4. Doelgroep (Wie)
- Voor welke doelgroep is deze richtlijn primair bedoeld
- Op welke manier kan elke doelgroep met deze richtlijn aan de slag (handelingsperspectief)

#### 5. Implementatie (Hoe)

##### Methoden/Technieken
Welke methoden en/of technieken kun je gebruiken om aan de richtlijn te voldoen. Aangeven welke methoden en/of technieken al dan niet verplicht of optioneel zijn. Verplicht betekent dat je eigenlijk zonder de methode of techniek niet aan de richtlijn kan voldoen.

##### Tools
Welke tools kun je gebruiken om aan de richtlijn te voldoen. Aangeven welke tools al dan niet verplicht of optioneel zijn. Verplicht betekent dat je eigenlijk zonder de tool niet aan de richtlijn kan voldoen. Onderscheid maken tussen soorten tools en concrete voorbeelden.

##### Subrichtlijnen
Opsomming van de subrichtlijnen (de korte omschrijving), dit zijn linkjes naar aparte pagina's voor elke subrichtlijn die ook weer dit sjabloon gebruiken.

#### 6. Succescriteria
Wanneer voldoe je wel/niet aan deze richtlijn

#### 7. Toepassingsvoorwaarde (Wie & Wanneer)
Wanneer is deze richtlijn voor jou van toepassing

#### 8. Bronnen

##### Wetten
Welke wetten zijn van toepassing op deze richtlijn

##### Beleid
Welke beleidsstukken zijn van toepassing op deze richtlijn

##### Standaarden
Welke standaarden zou je kunnen gebruiken om aan de richtlijn te voldoen

##### Communities
Welke communities bestaan er (in NL) waar kennis op het vlak van deze richtlijn wordt uitgewisseld

##### Literatuur
Welke (tijdloze/wetenschappelijke) literatuur is relevant voor deze richtlijn. Denk hier aan boeken en openbare wetenschappelijke artikelen

##### Bronnen op developer.overheid.nl
Blogs en kennisbank artikelen

#### 9. Gerelateerde Richtlijnen
Welke andere richtlijnen zijn gerelateerd en waarom? Versterkend effect bijvoorbeeld

## Voorbeeld YAML Structuur

```yaml
schema_version: "0.1.0"
titel: "Voorbeeld Richtlijn Titel"

beschrijving:
  wat: "Beschrijving van de richtlijn en de belangrijkste termen"

rationale:
  waarom: "Uitleg waarom deze richtlijn belangrijk is"
  beoogd_effect: "Het beoogde effect van deze richtlijn"
  risicos:
    - "Risico 1 bij niet-toepassen"
    - "Risico 2 bij niet-toepassen"

doelgroep:
  primaire_doelgroep:
    - "Softwareontwikkelaars"
    - "Projectmanagers"
  handelingsperspectief:
    - doelgroep: "Softwareontwikkelaars"
      handelingen: "Implementeer de richtlijn in de code"
    - doelgroep: "Projectmanagers"
      handelingen: "Zorg voor naleving binnen het project"

implementatie:
  methoden_technieken:
    - naam: "Methode 1"
      beschrijving: "Beschrijving van de methode"
      verplicht: true
    - naam: "Methode 2"
      beschrijving: "Beschrijving van de methode"
      verplicht: false
  tools:
    - naam: "Tool 1"
      type: "Automated testing tool"
      beschrijving: "Beschrijving van de tool"
      verplicht: true
      url: "https://example.com/tool1"
  subrichtlijnen:
    - titel: "Subrichtlijn 1"
      omschrijving: "Korte beschrijving"
      link: "./subrichtlijnen/subrichtlijn1.yaml"

succescriteria:
  - criterium: "Criterium 1 is voldaan"
    voldaan: true
  - criterium: "Criterium 2 is voldaan"
    voldaan: false

toepassingsvoorwaarde:
  voorwaarden:
    - "Deze richtlijn is van toepassing op alle overheidssystemen"
    - "Deze richtlijn is van toepassing bij het gebruik van AI"

bronnen:
  wetten:
    - naam: "AVG"
      url: "https://example.com/avg"
  beleid:
    - naam: "Beleidsdocument X"
      url: "https://example.com/beleid"
  standaarden:
    - naam: "ISO 27001"
      url: "https://example.com/iso27001"
  communities:
    - naam: "Developer.overheid.nl"
      url: "https://developer.overheid.nl"
  literatuur:
    - titel: "Boek over digitale systemen"
      auteurs:
        - "Auteur 1"
        - "Auteur 2"
      url: "https://example.com/boek"
      doi: "10.1234/example"
  developer_overheid:
    - titel: "Blog artikel over richtlijnen"
      type: "blog"
      url: "https://developer.overheid.nl/blog/artikel"

gerelateerde_richtlijnen:
  - titel: "Gerelateerde Richtlijn 1"
    relatie: "Versterkend effect op deze richtlijn"
    link: "./gerelateerde/richtlijn1.yaml"
```

## Schema

De richtlijnen worden gevalideerd tegen een JSON Schema. Het schema is te vinden in `schemas/richtlijn_schema.json`.

## Validatie

Om een richtlijn YAML bestand te valideren tegen het schema, gebruik het volgende commando:

```bash
./script/validate --file_pairs schemas/richtlijn_schema.json:uw-richtlijn.yaml
```

## Changelog

### Version 0.1.0 (2025-10-01)
- Initiële versie van de NeRDS richtlijn template
- Gebaseerd op de structuur zoals gedefinieerd in de oorspronkelijke template
- JSON Schema voor validatie toegevoegd
- Validatie script toegevoegd
