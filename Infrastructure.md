# Infrastructure

## Repositories

| Repo | Path | GitHub |
|------|------|--------|
| babel-ai (pipeline) | ~/repos/babel-ai | https://github.com/AncientTexts/babel-ai |
| library-ai (texts/data) | ~/repos/library-ai | https://github.com/AncientTexts/library-ai |
| AncientTextsVault (this vault) | ~/Obsidian/AncientTextsVault | https://github.com/AncientTexts/AncientTextsVault |

## Environment Variables

```
OPENAI_API_KEY       — in BabelSettings (OpenAI, ~$8.96 credit remaining as of 2026-02-27)
LIBRARY_PATH         — ~/repos/library-ai
PROMPT_DIRECTORY     — ~/repos/babel-ai/babel/prompts
```

## Running the Pipeline

```bash
cd ~/repos/babel-ai
dagster dev
```

## AI Budget Notes

- OpenAI credit running low (~$8.96 as of 2026-02-27)
- Plan: switch to Anthropic when exhausted
- Watch usage carefully during Suetonius run

## Obsidian Vault

- Path: ~/Obsidian/AncientTextsVault
- Git remote: https://github.com/AncientTexts/AncientTextsVault
- Managed by: Orion (Chief AI Officer)
