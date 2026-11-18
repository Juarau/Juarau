# Hub de Referências — Neurobranding & Neuromarketing

Central pessoal de anotações, conceitos, cases, referências e insights da pós,
curada por IA (Claude Code) para consulta e reuso em projetos futuros.

## Como usar (fluxo do dia a dia)

1. **Capture** — jogue o material bruto em [`inbox/`](inbox/):
   - texto digitado (`.md`, `.txt`, colado de qualquer lugar)
   - **fotos do caderno** (`.jpg`, `.png`, `.heic`* ) — uma ou várias páginas
   - PDFs de slides, prints de lousa, links soltos
2. **Processe** — numa sessão do Claude Code neste repositório, digite:
   ```
   /processar
   ```
   A IA transcreve as fotos, organiza, formata, cria/atualiza notas de conceito,
   cases e referências, conecta tudo e esvazia a inbox (originais vão para `anexos/`).
3. **Explore e use**:
   - `/consultar <pergunta ou projeto>` — ex.: `/consultar quero propor uma estratégia de embalagem para uma marca de café premium`
   - `/insights` — cruza o conteúdo acumulado e gera conexões, hipóteses e ideias de aplicação
   - `/revisar` — checagem de saúde: links quebrados, notas órfãs, afirmações sem fonte, conceitos duplicados

\* Se `.heic` der problema, exporte como `.jpg` no celular.

**Enviando do celular:** pelo app do Claude (anexando a foto numa sessão do Claude Code
apontada para este repo e pedindo `/processar`) ou pelo app do GitHub (upload direto em `inbox/`).

## Estrutura

| Pasta | O que vai lá |
|---|---|
| `inbox/` | Material bruto aguardando curadoria |
| `anexos/` | Originais preservados (fotos do caderno, PDFs) |
| `hub/notas/` | Uma nota por aula/encontro, fiel ao que você anotou + enriquecimento separado |
| `hub/conceitos/` | Uma nota atômica por conceito (ex.: viés de ancoragem, codificação de memória) |
| `hub/autores/` | Pesquisadores e autores recorrentes |
| `hub/cases/` | Cases de marca/campanha/estudo, com lição extraída |
| `hub/referencias/` | Livros, papers, artigos, vídeos, links |
| `hub/insights/` | Sínteses, conexões entre aulas, hipóteses suas |
| `hub/aplicacoes/` | Ideias de uso em projetos profissionais e pessoais |
| `_templates/` | Modelos de cada tipo de nota |
| [`INDEX.md`](INDEX.md) | Mapa geral do hub, mantido pela IA |

## Princípios de curadoria (o que a IA faz e o que ela NÃO faz)

- **Sua voz é preservada.** O que você escreveu fica na seção *Minhas anotações*, fiel.
  Tudo que a IA adiciona fica em seções marcadas *(IA)*. Você sempre sabe o que é seu.
- **Nível de evidência em toda afirmação científica.** Neuromarketing é um campo cheio de
  neuromitos (cérebro trino/"reptiliano", "botão de compra", "usamos 10% do cérebro").
  Cada conceito recebe um selo:

  | Selo | Significado |
  |---|---|
  | 🟢 forte | replicado, meta-análises, consenso |
  | 🟡 moderada | estudos sólidos, mas poucos ou com amostras pequenas |
  | 🟠 fraca/controversa | resultados mistos, falhas de replicação, extrapolação |
  | 🔴 mito | desacreditado pela literatura — útil saber, perigoso usar |
  | ⚪ não verificado | a IA não conseguiu checar; trate com cautela |

- **Nenhum link ou referência inventado.** Referências sugeridas só entram como verificadas
  se a IA conseguiu confirmá-las (busca na web); caso contrário ficam marcadas ⚪ *a verificar*.
- **Conteúdo do professor ≠ consenso científico.** Se algo dito em aula conflita com a
  literatura, a IA registra as duas coisas e aponta a divergência — sem apagar sua anotação.

## Lendo no Obsidian (opcional, recomendado)

Clone este repositório e abra a pasta como *vault* no [Obsidian](https://obsidian.md):
você ganha busca, grafo de conexões e leitura no celular. Os links são Markdown
relativos, então também funcionam navegando direto no GitHub.
