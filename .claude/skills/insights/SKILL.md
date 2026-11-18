---
name: insights
description: Gera insights a partir do acervo do hub — cruza aulas, conceitos e cases para encontrar conexões, padrões, tensões e ideias de aplicação. Use quando a pessoa pedir insights, sínteses, conexões, resumo de um tema, ou "o que eu aprendi sobre X".
---

# Gerar insights

Argumento opcional: um tema, disciplina, período ou projeto. Sem argumento: o acervo todo,
priorizando o que entrou desde o último insight em `hub/insights/`.

## Passos

1. Leia `INDEX.md` e as notas relevantes (aulas, conceitos, cases).
2. Procure, nesta ordem:
   - **Conexões não óbvias** entre aulas/disciplinas diferentes (ex.: um conceito de memória
     que explica um case visto em branding);
   - **Tensões:** professor A × professor B, aula × literatura, achado de lab × prática de
     mercado;
   - **Padrões:** temas recorrentes, autores que aparecem em muitas aulas;
   - **Lacunas:** conceitos citados sem base, áreas com só evidência 🟠/⚪;
   - **Aplicações:** como combinar 2–3 conceitos numa abordagem para um problema real.
3. Para cada insight, seja honesto sobre a força: marque `confianca` como `hipotese`,
   `plausivel` ou `sustentado` e escreva *Por que pode estar errado*. Não infle — 3 insights
   bons valem mais que 10 genéricos ("emoção importa no branding" não é insight).
4. Salve cada insight relevante em `hub/insights/AAAA-MM-DD-tema.md` (template
   `_templates/insight.md`), linke nas notas de origem e no `INDEX.md`.
5. Ideias concretas de uso vão para `hub/aplicacoes/`.
6. Commit: `insights: <tema>`.
7. Responda com um resumo e os links.
