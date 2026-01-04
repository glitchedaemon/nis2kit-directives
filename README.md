# NIS2Kit Compliance Directives

This repository contains the **open-source compliance logic** for [NIS2Kit](https://nis2kit.com), 
an AI-powered SaaS helping European SMBs achieve NIS2 compliance.

## Purpose
- **Transparency:** Clients can audit how AI validates their documents
- **Community:** Accept pull requests for regulation updates
- **Portability:** Use these directives with any LLM (OpenAI, Claude, Gemini)

## Structure
- `/requirements/` – 87-point NIS2 checklist requirements (Article 21)
- `/incident-templates/` – 24-hour early warning drafts (Article 23)
- `/acn-taxonomy/` – Italian CSIRT Italia notification formats

## Usage
These markdown files are consumed by n8n workflows via:
https://raw.githubusercontent.com/glitchedaemon/nis2kit-directives/main/requirements/*.md

## License
MIT License (Compliance logic is public, NIS2Kit platform is proprietary)

## Contributing
Pull requests welcome for:
- Regulatory interpretation updates
- Sector-specific requirements (healthcare, energy, finance)
- Translation to other EU languages
