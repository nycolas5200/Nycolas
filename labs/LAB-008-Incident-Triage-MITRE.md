# LAB-008 — Incident Triage & MITRE ATT&CK

**Área:** SOC N1 · Triagem · Resposta inicial  
**Status:** estudo de caso sintético; não representa incidente real.

## Cenário fictício
Um endpoint de laboratório registra falhas de autenticação em sequência e, depois, um logon bem-sucedido. Os dados são sintéticos e não executam ataques.

## Objetivo
Praticar triagem baseada em evidências, linha do tempo, hipóteses, classificação e escalonamento.

## Procedimento
1. Ler o arquivo `sample-events.csv`.
2. Normalizar data/hora para UTC.
3. Agrupar por host e usuário fictício.
4. Verificar quantidade e intervalo das falhas.
5. Correlacionar com o evento de sucesso.
6. Considerar hipóteses: erro de senha, automação, usuário legítimo ou tentativa indevida.
7. Listar informações adicionais necessárias.
8. Mapear MITRE ATT&CK apenas se a técnica for sustentada; T1110 pode ser relevante para brute force, conforme contexto.
9. Classificar prioridade considerando impacto, probabilidade e criticidade do ativo.
10. Elaborar recomendação e escalonamento.

## Linha do tempo ilustrativa
| Horário UTC | Evento | Interpretação provisória |
|---|---|---|
| 13:02 | Falha de autenticação | Validar origem |
| 13:03 | Falhas repetidas | Investigar frequência |
| 13:05 | Logon bem-sucedido | Correlacionar usuário e host |

## Modelo de relatório
- Resumo executivo em até cinco linhas.
- Escopo e fontes.
- Linha do tempo.
- Evidências confirmadas.
- Hipóteses e lacunas.
- Classificação justificada.
- Ações recomendadas.
- Limitações.

## Princípio
Não confundir alerta com incidente confirmado. Não atribuir intenção ou autoria sem evidência.

## Referências
- https://attack.mitre.org/techniques/T1110/
- https://www.cisa.gov/resources-tools/resources/incident-response
