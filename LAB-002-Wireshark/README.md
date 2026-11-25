# LAB-002 — Wireshark & Network Analysis

> Portfólio técnico de Nycolas Borges · Segurança da Informação, Redes e Infraestrutura

**Área:** Segurança de redes · Análise de pacotes  
**Status atual:** PRÁTICA PARCIAL — consolidar capturas sanitizadas e relatório

## 1. Objetivo
Interpretar tráfego próprio de laboratório e reconhecer DNS, ICMP, TCP e TLS/HTTPS por meio de filtros de exibição.

## 2. Pré-requisitos
- Wireshark instalado
- Computador próprio ou VMs em rede de laboratório
- Autorização para capturar o tráfego analisado

## 3. Procedimento passo a passo
1. Abrir o Wireshark e selecionar a interface de laboratório.
2. Iniciar a captura e gerar tráfego de teste.
3. Aplicar o filtro dns e observar consultas e respostas.
4. Aplicar icmp e observar echo request/reply, quando houver ping.
5. Aplicar tcp e analisar portas, flags e estabelecimento da conexão.
6. Aplicar tls para observar metadados da negociação TLS.
7. Registrar origem, destino, protocolo, portas e horário dos pacotes.
8. Salvar somente captura reduzida e sanitizada, se apropriado.
9. Elaborar relatório explicando o que foi observado e o que permaneceu criptografado.

## 4. Conceitos e pontos de atenção
Filtros úteis: `dns`, `icmp`, `tcp`, `tls`, `tcp.flags.syn == 1`. Um filtro como `ip.addr == 192.0.2.10` usa endereço reservado para documentação; substitua por IP do laboratório. HTTPS protege o conteúdo da comunicação; a captura comum permite observar metadados, não ler o conteúdo criptografado.

## 5. Evidências a registrar
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`

Crie a pasta `evidencias/` somente quando tiver arquivos reais para adicionar. Remova dados pessoais, endereços públicos, nomes de clientes, tokens, credenciais e qualquer informação corporativa.

## 6. Resultado esperado
Relacionar pacotes aos protocolos de rede e explicar os limites de visibilidade de uma captura HTTPS.

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
- https://www.wireshark.org/docs/

## 9. Transparência do portfólio
Este repositório diferencia estudo, roteiro e execução prática. Não declare o laboratório como concluído até executar as etapas, validar os resultados e incluir evidências próprias. Se uma etapa não puder ser realizada, documente a limitação.

## Documentação anterior
[Consultar a versão original em `labs/`](../labs/LAB-002-Wireshark.md)

[Voltar ao portfólio principal](../README.md) · [Site profissional](https://nycolas5200.github.io/Nycolas/)
