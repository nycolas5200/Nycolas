# LAB-007-TrendAI-Vision-One-XDR

> Portfólio técnico de Nycolas Borges · Segurança da Informação, Redes e Infraestrutura

**Área:** Segurança de endpoints · XDR · Operações de segurança  
**Status atual:** ESTUDO TÉCNICO DOCUMENTADO — prática depende de conta e treinamento autorizados

## 1. Objetivo
Compreender como uma plataforma XDR reúne telemetria, correlaciona atividades e apoia a investigação de alertas.

## 2. Pré-requisitos
- Acesso a treinamento ou tenant autorizado, se disponível
- Documentação oficial TrendAI/Trend Micro
- Cenários de estudo sem dados corporativos

## 3. Procedimento passo a passo
1. Receber alerta e identificar origem, horário, ativo e severidade.
2. Ler descrição e contexto da detecção.
3. Examinar processo, usuário, endpoint, rede e arquivos relacionados, quando disponíveis.
4. Correlacionar eventos pela linha do tempo.
5. Consultar reputação e contexto de IOC em fonte confiável.
6. Mapear comportamento para MITRE ATT&CK somente quando houver evidência.
7. Classificar como esperado, falso positivo, suspeito ou incidente confirmado.
8. Registrar evidências, lacunas, impacto e recomendação.
9. Escalar conforme procedimento; não executar contenção em ambiente real sem autorização.

## 4. Conceitos e pontos de atenção
EDR monitora e responde no endpoint; XDR correlaciona telemetria de múltiplas camadas; SIEM coleta, normaliza, correlaciona e analisa eventos; IOC é indicador técnico associado a possível comprometimento. Estudar a documentação não equivale a operar a console: mantenha essa distinção no portfólio.

## 5. Evidências a registrar
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`

Crie a pasta `evidencias/` somente quando tiver arquivos reais para adicionar. Remova dados pessoais, endereços públicos, nomes de clientes, tokens, credenciais e qualquer informação corporativa.

## 6. Resultado esperado
Explicar o fluxo de investigação de alertas XDR e registrar limites do estudo sem alegar experiência operacional não realizada.

## 7. Modelo de registro de execução
| Campo | Registro |
|---|---|
| Data e hora | A preencher após a prática |
| Ambiente / versão | A preencher |
| Etapas concluídas | A preencher |
| Resultado observado | A preencher com evidências |
| Dificuldades | A preencher |
| Próximos passos | A preencher |

## 8. Referências oficiais
- https://www.trendmicro.com/en_us/business/products/one-platform.html

## 9. Transparência do portfólio
Este repositório diferencia estudo, roteiro e execução prática. Não declare o laboratório como concluído até executar as etapas, validar os resultados e incluir evidências próprias. Se uma etapa não puder ser realizada, documente a limitação.

## Documentação anterior
[Consultar a versão original em `labs/`](../labs/LAB-007-TrendAI-Vision-One-XDR.md)

[Voltar ao portfólio principal](../README.md) · [Site profissional](https://nycolas5200.github.io/Nycolas/)
