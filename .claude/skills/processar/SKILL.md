---
name: processar
description: Faz a curadoria do material bruto em inbox/ (textos, fotos de caderno, PDFs, links) — transcreve, organiza, enriquece, cria/atualiza notas de aula, conceitos, cases, autores e referências, e atualiza o INDEX. Use quando a pessoa pedir para processar, organizar ou subir anotações, ou anexar fotos/textos de aula.
---

# Processar inbox

Siga as regras de `CLAUDE.md` (fidelidade, separação de autoria, evidência, zero invenção).

## Passos

1. **Inventário.** Liste tudo em `inbox/` (ignore `README.md`) e qualquer arquivo/imagem
   anexado diretamente na conversa. Agrupe por aula: fotos sequenciais da mesma data/
   disciplina viram UMA nota. Se faltar data ou disciplina e não der para inferir, pergunte
   uma única vez, agrupando todas as dúvidas; se a pessoa não estiver disponível, siga com
   `status: revisar-metadados`.

2. **Transcrição (fotos/PDF).** Leia cada imagem. Transcreva preservando hierarquia,
   setas, destaques e esquemas. Marque `[ilegível]` e `[?palavra]`. Não complete lacunas
   com conhecimento próprio dentro de *Minhas anotações*.

3. **Nota de aula.** Crie `hub/notas/AAAA-MM-DD-disciplina-tema.md` a partir de
   `_templates/nota-aula.md`. Preencha *Minhas anotações* fielmente; depois as seções (IA).

4. **Extração de entidades.** Para cada conceito, autor, case e referência relevante:
   - procure se já existe (`grep -ril` por nome, sinônimos e termo em inglês em `hub/`);
   - se existe: acrescente a aula em *Aparece em*, incorpore o que for novo, ajuste o selo
     de evidência se houver motivo, atualize a data;
   - se não existe e é relevante (aparece com substância, não só mencionado de passagem):
     crie com o template correspondente.
   Não crie notas vazias só para ter link.

5. **Enriquecimento.** Na nota de aula e nos conceitos novos:
   - contexto e estudos de base (com selo de evidência);
   - contrapontos e críticas — especialmente neuromitos, inferência reversa, amostras
     pequenas, validade ecológica, questões éticas;
   - 1–3 cases relacionados (reais e verificáveis; distinga estudo científico de narrativa
     de mercado);
   - 1–3 referências para aprofundar. Se houver ferramenta de busca (WebSearch), verifique
     existência e link antes de marcar `verificada: true`. Sem verificação: `⚪ a verificar`,
     sem URL inventada;
   - *Para aplicar*: perguntas de briefing, ideias de teste/medição, cuidados.

6. **Arquivamento.** Mova originais da inbox para `anexos/` renomeados
   (`AAAA-MM-DD-disciplina-tema-pN.ext`) e linke-os no front matter `originais`.
   Textos já transcritos integralmente na nota podem ser apagados da inbox.

7. **INDEX.md.** Atualize: aulas por disciplina (mais recentes primeiro), conceitos por área
   com selo, cases, referências, insights, aplicações, e a seção *Pendências* (itens ⚪,
   `revisar-*`, dúvidas em aberto).

8. **Commit.** `git add -A && git commit -m "processar: <aulas processadas>"` e push no branch
   de trabalho, se houver remoto configurado.

9. **Relatório curto** para a pessoa:
   - o que foi criado/atualizado (com links);
   - trechos com transcrição incerta para ela conferir;
   - divergências aula × literatura encontradas;
   - 1–2 conexões interessantes com o que já existia no hub.
