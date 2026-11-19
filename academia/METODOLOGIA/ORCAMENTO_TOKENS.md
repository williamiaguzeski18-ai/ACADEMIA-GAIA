# Equivalência de carga e tokens — protocolo de calibração G02

- **ID:** GAIA-EDU-TOKENS
- **Versão:** 0.2.0
- **Data:** 2026-11-19
- **Estado:** PROCEDIMENTO DOCUMENTADO — CALIBRAÇÃO PENDENTE (G02)
- **Responsável proposto:** Coordenação pedagógica
- **Escopo:** medir carga documental com evidência, não inferir competência

## Princípio e parâmetros ainda não fixados
As quatro formações terão o mesmo orçamento curricular-alvo **T = NÃO DEFINIDO** até escolha de referência e medição dos materiais reais. Proporção inicial **20% T para base comum** e **80% T para especialização**, **NÃO HOMOLOGADA**. A base comum é guardada uma só vez e contabilizada uma vez no total de cada curso que a utiliza.

`T` ≠ janela de contexto, tokens efetivamente consumidos, custo de inferência ou aprendizado permanente.

| Parâmetro | Valor |
|---|---|
| `T` tokens de material por curso | NÃO DEFINIDO |
| Tokenizer e versão/snapshot | NÃO DEFINIDO |
| Regra de limpeza/normalização de Markdown | NÃO DEFINIDA |
| Tolerância percentual de desvio | NÃO DEFINIDA |
| Escopo de contagem (fonte, exemplos, exercícios) | NÃO DEFINIDO |
| Limite por execução e estratégia de recuperação | NÃO DEFINIDOS |
| Responsável pela aprovação | PROPRIETÁRIO |

## Procedimento medível G02
1. Escolher modelo/tokenizer compatível, versão exata e ferramenta reprodutível de contagem; indicar referências oficiais.
2. Fixar e justificar o que entra no orçamento: texto das aulas, exemplos, enunciados e eventual metadado. Separar URLs, gabaritos privados, logs e histórico operacional.
3. Padronizar codificação UTF-8, quebras de linha, tratamento de Markdown e arquivos excluídos.
4. Produzir inventário `file_path`, `git_blob_sha`, `course_id`, `module_id`, `token_count`, `tokenizer_version` e `measured_at`.
5. Calcular por curso `B` (base comum, contada uma vez) e `S_i` (especialização), com `T_i=B+S_i`.
6. Para cada curso, calcular `desvio_i = |T_i-T|/T × 100%` apenas se `T>0`; qualquer tolerância exige decisão humana.
7. Verificar execução com retrieval/chunking e janelas de contexto reais; não presumir carregamento simultâneo.
8. Documentar diferenças em profundidade e resultados das avaliações. Igualdade numérica de tokens não prova equivalência de competência.
9. Registrar versão da contagem, evidências, data/hora/fuso/relógio e responsável; submeter a homologação.

## Aceite P03
O método é especificado neste G01. **Nenhum valor T, tokenizer, tolerância, medição ou conclusão de equivalência está aprovado ou executado.** Esses resultados pertencem ao G02.
