# LAB-001 — Wazuh SIEM / SOC

**Área:** Blue Team · SIEM · Monitoramento de endpoints  
**Status:** guia técnico preparado; execução e evidências pendentes.

## Objetivo
Construir um laboratório isolado para centralizar eventos de segurança, integrar um endpoint Windows e validar monitoramento de integridade de arquivos (FIM).

## Arquitetura sugerida
- VirtualBox com rede interna ou host-only.
- VM Ubuntu Server para Wazuh.
- VM Windows 10/11 para o agente.
- Navegador no host para acessar o dashboard pela rede privada.

## Pré-requisitos
ISOs obtidas de fontes oficiais, recursos de VM adequados à versão escolhida, acesso administrativo e leitura da documentação Wazuh. Não utilize máquinas ou dados corporativos.

## Procedimento
1. Criar as VMs e configurar uma rede privada entre elas.
2. Atualizar o Ubuntu e registrar versão, hostname e IP privado.
3. Instalar Wazuh seguindo o procedimento oficial da versão selecionada.
4. Validar os serviços e acessar o dashboard apenas pela rede do laboratório.
5. Instalar o agente Windows compatível com a versão do manager.
6. Configurar o endereço privado do manager e iniciar o agente.
7. Confirmar o endpoint como ativo no dashboard.
8. Configurar FIM para uma pasta de teste não sensível.
9. Criar, alterar e remover um arquivo fictício nessa pasta.
10. Localizar os eventos e registrar horário, endpoint, caminho e tipo de alteração.
11. Elaborar uma análise curta: evento observado, hipótese, evidência e próximo passo.

## Conceitos
- SIEM: coleta, normalização, correlação e análise de eventos.
- Agent: componente que encaminha telemetria do endpoint.
- FIM: identifica alterações em arquivos e diretórios monitorados.
- Alerta não é automaticamente um incidente confirmado.

## Evidências a adicionar após execução
- `01-topologia.png` — VMs e rede, sem dados sensíveis.
- `02-dashboard.png` — painel sanitizado.
- `03-agent-active.png` — agente ativo.
- `04-fim-event.png` — evento de teste.
- `05-analysis.md` — análise do evento real do laboratório.

## Ficha de análise
| Campo | Preencher |
|---|---|
| ID do caso | LAB001-INC-___ |
| Data/hora e fuso | |
| Endpoint | |
| Fonte do evento | |
| Evento observado | |
| Evidência | |
| Hipótese | |
| Classificação | |
| Próxima ação | |

## Resultado esperado
Demonstrar o fluxo endpoint → agente → manager → dashboard e explicar como alterações controladas podem ser identificadas.

## Referências
- https://documentation.wazuh.com/
- https://attack.mitre.org/
