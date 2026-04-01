---
description: "Use when editing README.md or README_EN.md. Covers bilingual sync, markdown conventions, section structure and badge formatting for the GitHub profile README."
applyTo: "README*.md"
---
# Regras para Edição dos READMEs do Perfil

## Paridade Bilíngue Obrigatória

- `README.md` é PT-BR. `README_EN.md` é EN.
- Toda mudança de conteúdo deve ser aplicada nos **dois arquivos**.
- Seções, ordem e estrutura devem ser idênticas. Apenas o idioma muda.

## Estrutura de Seções (preservar ordem)

1. Cabeçalho e link para versão no outro idioma
2. 🚀 Sobre Mim / About Me
3. 🌟 Premiações e Reconhecimento / Awards and Recognition
4. 🏆 Certificações / Certifications
5. 🎓 Instrutor / Instructor
6. 🎓 Formação Acadêmica / Education
7. 💼 Destaques da Experiência / Experience Highlights
8. 🥋 Além do Código: Jiu-Jitsu / Beyond Code: Jiu-Jitsu
9. 📫 Como me encontrar / How to Find Me

## Formatação de Badges de Certificação

Cada grupo de certificações segue o padrão:
```html
<p align="left">
  <img src="assets/badges/nome-do-badge.png" alt="Descrição" height="100"/>
</p>
```
Seguido de lista Markdown com as certificações. Relevantes em **negrito**.

## Badges Legacy (width diferente)

Certificações legacy da Microsoft e Java usam `width="100"` com `align="top"` e `&nbsp;&nbsp;` como separador.

## Seção de Prêmios

Usa `<table>` com `<tr>/<td>` para layout. Imagens de prêmios usam `height="200"` ou `height="250"`.

## Links de Redes Sociais

Formato: `- 🔗 Plataforma: [handle](url)`. Sempre na última seção.
