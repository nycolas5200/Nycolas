# LAB-001 — Wazuh SIEM / SOC

> Portfólio técnico de Nycolas Borges · Segurança da Informação, Redes e Infraestrutura

**Área:** Segurança defensiva · SIEM · Monitoramento de endpoints  
**Status atual:** GUIA TÉCNICO PREPARADO — execução e evidências ainda pendentes

## 1. Objetivo
Construir um ambiente isolado para centralizar eventos de segurança, integrar um endpoint Windows e validar monitoramento de integridade de arquivos (FIM).

## 2. Pré-requisitos
- VirtualBox com rede interna ou host-only
- VM Ubuntu Server para o Wazuh Manager
- VM Windows 10/11 para o agente
- Acesso administrativo às VMs e documentação oficial Wazuh

## 3. Procedimento passo a passo
1. Criar as VMs e configurar uma rede privada entre elas.
2. Atualizar o Ubuntu e registrar versão, hostname e IP privado.
3. Instalar Wazuh seguindo o procedimento oficial da versão escolhida.
4. Validar serviços e acessar o dashboard somente pela rede privada do laboratório.
5. Instalar o agente Windows compatível com a versão do manager.
6. Configurar o endereço privado do manager e iniciar o agente.
7. Confirmar o endpoint como ativo no dashboard.
8. Configurar FIM para uma pasta de teste não sensível.
9. Criar, alterar e remover um arquivo fictício nessa pasta.
10. Localizar os eventos e registrar horário, endpoint, caminho e tipo de alteração.
11. Produzir uma análise com evento, hipótese, evidência e próximo passo.

## 4. Conceitos e pontos de atenção
SIEM coleta, normaliza, correlaciona e analisa eventos. O agente encaminha telemetria do endpoint. FIM identifica alterações em arquivos monitorados. Um alerta, isoladamente, não confirma um incidente.

## 5. Evidências a registrar
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`

Crie a pasta `evidencias/` somente quando tiver arquivos reais para adicionar. Remova dados pessoais, endereços públicos, nomes de clientes, tokens, credenciais e qualquer informação corporativa.

## 6. Resultado esperado
Demonstrar o fluxo endpoint → agente → manager → dashboard e explicar como alterações controladas podem ser identificadas.

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
- https://documentation.wazuh.com/

## 9. Transparência do portfólio
Este repositório diferencia estudo, roteiro e execução prática. Não declare o laboratório como concluído até executar as etapas, validar os resultados e incluir evidências próprias. Se uma etapa não puder ser realizada, documente a limitação.

## Documentação anterior
[Consultar a versão original em `labs/`](../labs/LAB-001-Wazuh-SIEM-SOC.md)

[Voltar ao portfólio principal](../README.md) · [Site profissional](https://nycolas5200.github.io/Nycolas/)
