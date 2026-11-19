# Checklist de validação da estrutura ACADEMIA GAIA (P05)

- **ID:** GAIA-EDU-VAL
- **Versão:** 0.2.0
- **Data:** 2026-11-19
- **Estado:** MODELO DE CHECKLIST — NÃO HOMOLOGADO
- **Escopo:** validação técnica antes de qualquer integração; não executa CI

## Referência
- Repositório: `williamiaguzeski18-ai/ACADEMIA-GAIA`
- Branch de trabalho: `docs/academia-gaia-estrutura-base-v01`
- PR: `#1`
- Commit verificado (preencher no momento do teste): PENDENTE
- Validador/data/hora/fuso/relógio: PENDENTE

## Matriz mínima — cada item exige evidência
| ID | Verificação | Evidência requerida | Situação |
|---|---|---|---|
| V01 | Quatro trilhas 00–03 presentes | Listagem do commit | NAO_EXECUTADO |
| V02 | Base comum C01–C04 preservada | Paths e SHAs | NAO_EXECUTADO |
| V03 | Oito módulos especializados por trilha (32) | Paths e SHAs | NAO_EXECUTADO |
| V04 | CURSO / EVOLUCAO / PROJETO presentes em cada agente | Paths e links | NAO_EXECUTADO |
| V05 | Markdown e links relativos íntegros | Relatório de checker com erros=0 | NAO_EXECUTADO |
| V06 | IDs de curso/módulo/documento únicos | Relatório de IDs e duplicações=0 | NAO_EXECUTADO |
| V07 | Metadados e estados exigidos presentes | Lista de campos/erros | NAO_EXECUTADO |
| V08 | Nenhum gabarito real ou caso cego publicado | Revisão humana, busca por padrões e diff | NAO_EXECUTADO |
| V09 | Verificação de segredos e arquivos sensíveis | Scanner e revisão dos achados | NAO_EXECUTADO |
| V10 | CI exigida no commit exato | URL de execução e conclusão verde | NAO_EXECUTADO |

## Procedimento
1. Conferir HEAD da branch e SHA antes da validação.
2. Limitar diffs ao escopo documental autorizado; registrar caminhos incluídos.
3. Validar V01–V09 com ferramentas de leitura e registrar seus resultados. Uma busca por padrões não substitui auditoria completa de dados sensíveis.
4. Verificar execução de CI pertinente ao projeto para o commit exato, sem confundir ausência de verificações com CI verde.
5. Fazer readback remoto de todos os arquivos modificados e criados.
6. Comparar SHAs dos 36 módulos com a referência anterior.
7. Registrar falhas, evidências e recomendações; solicitar decisão humana de integração separadamente.

## Regra de aceite
**Sem CI verde exigida e comprovada no commit exato, não declarar pronto para merge.** Documentar verificações pontuais separadamente da CI. Nem um relatório aprovado nem um clique em controle de continuidade concede autorização para merge ou deploy.

**Este arquivo é um modelo, não atesta que as verificações foram executadas.**
