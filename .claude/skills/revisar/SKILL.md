---
name: revisar
description: Auditoria de qualidade do hub — links quebrados, notas órfãs, duplicatas, conceitos sem selo de evidência, referências não verificadas, metadados pendentes. Use quando a pessoa pedir para revisar, limpar, checar ou fazer manutenção do hub.
---

# Revisar o hub

1. Rode as checagens:
   - **links quebrados:** todo link Markdown relativo em `hub/` e `INDEX.md` aponta para
     arquivo existente;
   - **órfãs:** notas em `hub/` que nenhuma outra nota linka;
   - **duplicatas:** conceitos com nomes/sinônimos sobrepostos (inclusive PT × EN);
   - **evidência:** conceitos e cases sem selo ou com ⚪;
   - **referências** com `verificada: false` — se houver busca disponível, tente verificar;
   - **status** `revisar-metadados` / `revisar-transcricao`;
   - **front matter** inválido ou fora do template.
2. Corrija automaticamente o que é mecânico (links, `Aparece em` faltando, INDEX).
3. Para o que exige decisão (fundir duplicatas, rebaixar selo, apagar), liste e pergunte.
4. Commit: `revisar: manutencao`.
5. Relatório: o que foi corrigido, o que precisa da pessoa.
