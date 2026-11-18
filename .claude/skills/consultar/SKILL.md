---
name: consultar
description: Responde perguntas e apoia projetos usando o hub como base primária — busca conceitos, cases e referências relevantes, cita as notas, e indica o que vem do hub e o que é conhecimento geral. Use quando a pessoa perguntar algo sobre o conteúdo da pós ou quiser aplicar o que aprendeu a um projeto, briefing, apresentação ou decisão.
---

# Consultar o hub

1. Entenda a pergunta ou o projeto. Se for um projeto, identifique: objetivo, público,
   categoria, restrição.
2. Busque no hub (`INDEX.md`, `grep -ril` por termos e sinônimos em `hub/`). Leia as notas
   mais relevantes.
3. Responda estruturado:
   - **Do seu hub:** o que suas notas dizem, com links (`hub/conceitos/x.md`), e o selo de
     evidência de cada base usada;
   - **Complemento (IA):** conhecimento geral que ajuda e não está no hub — marcado como tal;
   - **Cuidados:** limites da evidência, riscos éticos (manipulação, públicos vulneráveis,
     LGPD para dados biométricos/neurofisiológicos) e de execução;
   - Para projetos: proposta prática, como medir/testar, e o que levar para um briefing.
4. Se a pergunta revelar uma lacuna no hub, diga e ofereça criar a nota (não crie sem
   pedir). Se a pessoa quiser guardar a resposta, salve em `hub/aplicacoes/`.
5. Não invente que algo está nas notas. Se não está, diga.
