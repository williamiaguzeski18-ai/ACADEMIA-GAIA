# Gates da Academia GAIA

- **ID:** GAIA-EDU-GATES
- **Versão:** 0.2.0
- **Data:** 2026-11-19
- **Estado:** CRITÉRIOS CORRIGIDOS — NÃO HOMOLOGADOS
- **Responsável proposto:** Proprietário / CHAT 00
- **Escopo:** formação técnica, sem autorizar ação no projeto operacional

| Gate | Critério de saída | Estado documentado |
|---|---|---|
| G00 — Estrutura | Diretórios, modelos e 36 módulos identificados em branch | ESTRUTURADO EM PR #1, NÃO INTEGRADO |
| G01 — Revisão/homologação | P01–P05 documentados, diff/readback e aceite humano expresso | HOMOLOGAÇÃO PENDENTE |
| G02 — Calibração | Tokenizer, `T`, tolerância e medição real aprovados | PENDENTE |
| G03 — Conteúdo | Aulas, fontes e exercícios elaborados e revisados | NAO_INICIADO |
| G04 — Avaliação | Casos executados, rubrica, baseline, evidências e revisão | NAO_INICIADO |
| G05 — Publicação/reuso | Aprovações, licença e destino correto; CI e integração quando aplicáveis | NAO_INICIADO |

## Critérios G01 (P01–P05)
- **P01:** separar enunciado entregável e gabarito efetivo reservado; publicar somente formulário vazio.
- **P02:** 24 casos propostos por agente; cobertura, rubrica, estados e falha crítica descritos, sem resultados fictícios.
- **P03:** método de tokens documentado, valores de `T` e tolerância explicitamente pendentes para G02.
- **P04:** contrato de aula com competência, fontes, exercícios, critérios e rastreabilidade, sem conteúdos preenchidos.
- **P05:** checklist V01–V10 e evidências; CI verde no commit exato antes de integrar, conforme política aplicável.

## Fronteiras
- Revisão documental ≠ homologação educacional.
- Homologação educacional ≠ autorização de merge ou publicação.
- CI configurada ≠ CI executada ≠ CI aprovada.
- Curso disponível no contexto ≠ competência comprovada.
- Sem escrita de memórias, acesso a outros serviços ou execução no projeto operacional.

**Estados:** CONCLUIDO apenas com evidência e autorização; PROCESSADO é não definitivo; PENDENTE exige decisão; BLOQUEANTE impede a operação afetada; NAO_ANALISADO não foi tratado.
