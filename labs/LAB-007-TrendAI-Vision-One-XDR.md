# LAB-007 — TrendAI Vision One: fundamentos XDR

**Área:** Segurança de endpoints · XDR · Operações de segurança  
**Status:** estudo técnico documentado; prática depende de conta e treinamento autorizados.

## Objetivo
Compreender como uma plataforma XDR reúne telemetria, correlaciona atividades e apoia a investigação de alertas.

## Conceitos
- **EDR:** monitoramento e resposta no endpoint.
- **XDR:** correlação de telemetria de múltiplas camadas.
- **SIEM:** coleta, normalização, correlação e análise de eventos.
- **IOC:** indicador técnico associado a possível comprometimento.
- **Workbench/alerta:** agrupamento de atividades para investigação, conforme recursos/licença.
- **Response actions:** ações de contenção sujeitas a permissão e política.

## Fluxo de investigação
1. Receber alerta e identificar origem, horário, ativo e severidade.
2. Ler descrição e contexto da detecção.
3. Examinar processo, usuário, endpoint, rede e arquivos relacionados, quando disponíveis.
4. Correlacionar eventos pela linha do tempo.
5. Consultar reputação/contexto de IOC em fonte confiável.
6. Mapear comportamento para MITRE ATT&CK somente com evidência.
7. Classificar como esperado, falso positivo, suspeito ou incidente confirmado.
8. Registrar evidências, lacunas, impacto e recomendação.
9. Escalar conforme procedimento; não executar contenção em ambiente real sem autorização.

## Modelo de registro
| Campo | Registro |
|---|---|
| Alerta | ID e nome |
| Ativo | endpoint fictício/sanitizado |
| Timestamp | data, hora e fuso |
| Evidência | evento, processo, hash ou conexão |
| IOC | valor e fonte |
| ATT&CK | técnica sustentada pela evidência |
| Veredito | benigno / suspeito / confirmado / inconclusivo |
| Ação | validar / monitorar / escalar |

## Limites de conhecimento
Estudar a documentação não equivale a operar a console. Descrever como conhecimento introdutório até concluir treinamento e demonstrar uma investigação em laboratório autorizado.

## Evidências
Adicionar capturas de treinamento autorizadas e sanitizadas, sem tenant ID, e-mail, cliente, token ou informação corporativa.

## Referências
- https://www.trendmicro.com/en_us/business/products/one-platform.html
- https://success.trendmicro.com/
- https://attack.mitre.org/
