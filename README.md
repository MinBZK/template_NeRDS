# Template NeRDS

This repository provides a standardized template for documenting NeRDS (Nederlandse Richtlijnen Digitale Systemen - Dutch Guidelines for Digital Systems) guidelines. It ensures consistency and completeness across all guidelines used within the Dutch government for digital systems.

## Background

As digital systems become increasingly complex and critical to government operations, the need for clear, comprehensive, and standardized documentation becomes essential. The NeRDS template addresses this need by providing:

1. **Consistent Structure** - All guidelines follow the same format, making them easier to understand and compare
2. **Comprehensive Coverage** - The template ensures all important aspects are documented (what, why, who, how, when)
3. **Validation** - JSON Schema validation ensures guidelines meet structural requirements
4. **Versioning** - Clear version tracking allows guidelines to evolve over time

## Structure

A NeRDS guideline document consists of nine main sections:

1. **Richtlijn Titel** - The guideline title
2. **Beschrijving (Wat)** - Description of what the guideline covers
3. **Rationale (Waarom)** - Why the guideline is important, intended effects, and risks of non-compliance
4. **Doelgroep (Wie)** - Target audience and action perspectives
5. **Implementatie (Hoe)** - How to implement: methods/techniques, tools, and sub-guidelines
6. **Succescriteria** - Success criteria for compliance
7. **Toepassingsvoorwaarde (Wie & Wanneer)** - When the guideline applies
8. **Bronnen** - Sources including laws, policies, standards, communities, literature, and developer.overheid.nl resources

## Usage

### Creating a New Guideline

1. Create a new MkDocs/YAML file using the structure defined in `nerds-standard/latest.md`
2. Fill in all relevant sections according to your guideline
3. Validate your MkDocs/YAML file against the schema


### Validating Guidelines

To validate a guideline YAML file:

```bash
./nerds-standard/script/validate --file_pairs nerds-standard/schemas/richtlijn_schema.json:your-guideline.yaml
```

## License

This project is licensed under the EUPL-1.2 License - see the LICENSE file for details.
