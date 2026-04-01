---
description: "Sync certifications from Credly profile. Fetches both Credly and Other tabs, compares with current READMEs, and proposes additions or removals."
agent: "agent"
argument-hint: "Sincronizar badges do Credly"
---
Sincronize as certificações do perfil com o Credly público do André Dias.

## Fontes de Dados

Consultar **ambas** as URLs:
1. **Aba Credly**: https://www.credly.com/users/andredias/badges
2. **Aba Other**: https://www.credly.com/users/andredias/badges?tab=other

## Passos

1. Acessar ambas as URLs do Credly usando a ferramenta de fetch
2. Mapear todos os badges encontrados com: nome, emissor, data, status (ativo/expirado)
3. Comparar com a lista atual em `README.md` e `assets/badges/README.md`
4. Identificar:
   - **Novos**: badges no Credly que não estão no repositório
   - **Expirados recentes**: badges que expiraram desde a última sync
   - **Removidos**: badges no README que não estão mais no Credly
5. Para cada badge novo:
   - Verificar se o arquivo de imagem existe em `assets/badges/`
   - Se não existir, informar o usuário que precisa baixar manualmente e sugerir nome no padrão kebab-case
   - Adicionar à categoria correta em `README.md` e `README_EN.md`
   - Adicionar ao catálogo em `assets/badges/README.md`
6. Apresentar resumo das diferenças ao usuário antes de aplicar mudanças

## Regras

- **Ignorar badges de MeasureUp / Cert Ready** — são simulados de prática, não certificações reais. Nunca incluir no README
- **Ignorar badges de Microsoft Applied Skills** — não devem ser incluídos no perfil
- Badges expirados que já estão no README podem permanecer (conquistas históricas)
- Novos badges expirados NÃO precisam ser adicionados ao README principal
- Certificações de fora do Credly (Sun/Oracle, Microsoft Learn) são mantidas manualmente
- Manter paridade PT-BR/EN em ambos os READMEs
- Certificações relevantes ficam em **negrito**, demais em texto normal
