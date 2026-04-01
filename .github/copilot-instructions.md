# Instruções do Projeto

## Visão Geral

Este é o repositório de perfil do GitHub (`andrediasbr/andrediasbr`). O README.md é exibido na página principal do perfil GitHub do André Dias.

## Conteúdo Bilíngue

- `README.md` — versão principal em **Português (PT-BR)**
- `README_EN.md` — versão espelho em **Inglês (EN)**
- **Toda alteração de conteúdo deve ser replicada em ambos os arquivos**, mantendo a mesma estrutura, seções e ordem.

## Estrutura de Pastas

```
assets/
├── badges/       # Badges de certificações (PNG, SVG, JPG, GIF)
├── mvp/          # Imagens do prêmio Microsoft MVP
├── github-partner-award/  # Imagens do GitHub Partner Award
├── profile/      # Fotos pessoais (jiu-jitsu, etc.)
```

## Convenções de Markdown

- Badges de certificação usam `<img>` com `height="100"` dentro de `<p align="left">`
- Seções de prêmios usam `<table>` HTML para layout lado a lado
- Nomes de arquivos de badges seguem o padrão: `nome-descritivo.png` (kebab-case, minúsculas)
- Links de redes sociais ficam na seção final "Como me encontrar" / "How to Find Me"

## Tom e Estilo

- Tom profissional, mas acessível
- Ênfase em resultados e impacto, não apenas títulos
- Certificações mais relevantes ficam em **negrito**, demais em texto normal
- Emojis são usados nos títulos de seção (ex: 🚀, 🏆, 💼)

## Ao Editar

- Manter a paridade completa entre `README.md` e `README_EN.md`
- Ao adicionar badges, colocar a imagem E o texto descritivo na lista
- Ao adicionar certificações, atualizar também `assets/badges/README.md` com o novo badge
- Preservar a ordem das seções existentes
- Usar imagens já salvas em `assets/badges/` — nunca referenciar URLs externas para badges

## Fonte de Dados: Credly

- O perfil público do Credly é a fonte de verdade para certificações e badges:
  - **Aba Credly**: https://www.credly.com/users/andredias/badges (badges principais)
  - **Aba Other**: https://www.credly.com/users/andredias/badges?tab=other (badges adicionais de MeasureUp, Certiprof, etc.)
- Ao atualizar certificações, **sempre consultar ambas as abas** do Credly para verificar novos badges
- **Ignorar badges de MeasureUp / Cert Ready** — são simulados de prática, não certificações reais
- **Ignorar badges de Microsoft Applied Skills** — não devem ser incluídos no perfil
- A aba "Other" do Credly agrega certificações do **Microsoft Learn** (incluindo AI Transformation Leader, MS-365 Fundamentals, e renovações de certificações Azure). Esses badges são reais e devem ser incluídos
- Badges expirados podem ser mantidos no README (representam conquistas históricas), mas novos badges expirados não precisam ser adicionados
- O campo "Issued/Expires" do Credly indica a validade do badge
- Imagens de badges das certificações Microsoft podem ser baixadas diretamente do Credly CDN: `https://images.credly.com/images/{id}/image.png`
- Algumas certificações podem vir de fontes fora do Credly (ex: Sun/Oracle) — essas são mantidas manualmente
- O arquivo `assets/badges/README.md` serve como catálogo completo de todos os badges, incluindo os que não são exibidos no perfil principal
