---
description: "Add a new certification badge to the GitHub profile README. Handles image placement, text list, bilingual sync, and badges README catalog update."
agent: "agent"
argument-hint: "Nome da certificação e categoria (ex: 'GitHub Copilot Business - GitHub')"
---
Adicione uma nova certificação ao perfil. O usuário vai fornecer:
- Nome da certificação
- Categoria (Azure, AWS, GCP, GitHub, HashiCorp, Scrum, etc.)
- Se é relevante (bold) ou não
- Nome do arquivo do badge (já deve existir em `assets/badges/`)

## Fonte de Dados

Se o usuário não informar todos os detalhes, consultar o Credly para confirmar:
- **Aba Credly**: https://www.credly.com/users/andredias/badges
- **Aba Other**: https://www.credly.com/users/andredias/badges?tab=other
- **Ignorar**: badges de MeasureUp/Cert Ready (simulados) e Microsoft Applied Skills

## Passos

1. Confirmar que o arquivo do badge existe em `assets/badges/`
2. Adicionar a tag `<img>` dentro do `<p align="left">` da categoria correta em `README.md`, com `height="100"`
3. Adicionar o nome na lista Markdown abaixo (em **negrito** se relevante)
4. Replicar exatamente em `README_EN.md` (traduzir descrição se necessário)
5. Adicionar entrada no `assets/badges/README.md` na categoria correta
