# EVSE ID Generator

Generate and validate **EVSE identifiers** compliant with **ISO 15118** and **OCPP 2.0.1** standards for electric vehicle charging infrastructure.

[![EVSE ID Generator](https://raw.githubusercontent.com/lex/evse-id-generator/master/preview.png)](https://lex.github.io/evse-id-generator/)

[**Open EVSE ID Generator**](https://lex.github.io/evse-id-generator/)

## Features

- **Generate EVSE IDs** with configurable country code, operator code, and suffix patterns (sequential, random, alphanumeric)
- **Validate EVSE IDs** against the ISO 15118 format specification
- **Bulk generation** of sequential EVSE ID series for fleet deployment
- **Batch validation** — paste multiple IDs to check and parse at once
- **Export to TXT** — download generated or validated IDs for use in OCPP systems
- **Format parsing** — breaks down each ID into its country code, operator, and EVSE components

## EVSE ID Format

The EVSE identifier follows the ISO 15118 structure:

```
[CC]*[OP]*E[EVSE]
```

- **Country Code** — 2-letter ISO 3166-1 alpha-2 code
- **Operator Code** — 3-character operator identifier
- **EVSE Identifier** — unique charging station suffix (alphanumeric, 1-30 characters)
- **Separator** — optional `*` between segments

## Use Cases

- Setting up charging stations for OCPP 2.0.1 backend integration
- Generating test identifiers for ISO 15118 development
- Batch provisioning EVSE IDs for charging infrastructure deployment
- Validating existing EVSE identifiers against the standard

## Tech Stack

Built with React, Babel (standalone), and Geist/Geist Mono fonts. Hosted as a static site on GitHub Pages.
