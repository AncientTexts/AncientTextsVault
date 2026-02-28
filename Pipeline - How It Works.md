# Pipeline — How It Works

## Overview

Perseus XML → LLM Translation → QC → EPUB with cover → Amazon KDP

## Stack

- **Dagster** — pipeline orchestration
- **OpenAI / Anthropic** — LLM translation + QC
- **Perseus Digital Library** — source texts (public domain Latin XML)
- **Amazon KDP** — distribution

## Source Texts

- Sourced from Perseus Digital Library (GitHub mirror)
- XML format, converted as needed for pipeline ingestion

## Cover Generation

Each book gets a custom thematic cover:

| Title | Colour Theme |
|-------|-------------|
| De Republica | Slate |
| Dialogue on the Orators | Maroon/Red |
| De Bello Gallico | Imperial/Purple |
| The Twelve Caesars | Amber/Gold (#7B4F00 / #FFE8A3) |

## QC Process

- Sam reads every published book on his Kindle (commute)
- Any translation errors flagged for pipeline improvement

## Running a New Book

1. Download source XML from Perseus GitHub
2. Convert XML format if needed
3. Add to library-ai repo (books.json, author metadata, acknowledgements)
4. Run `dagster dev` from babel-ai
5. Review epub output
6. Upload to KDP, set 70% royalty tier, enrol in KDP Select
