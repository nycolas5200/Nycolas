# LAB-002 — Wireshark: análise de tráfego

**Área:** Network Security · Análise de pacotes  
**Status:** prática parcial; consolidar capturas sanitizadas e relatório.

## Objetivo
Interpretar tráfego próprio de laboratório e reconhecer DNS, ICMP, TCP e TLS/HTTPS por meio de filtros de exibição.

## Escopo e segurança
Capture apenas tráfego do seu computador, VMs próprias ou redes para as quais tenha autorização. Não intercepte tráfego de terceiros.

## Roteiro
1. Abrir o Wireshark e selecionar a interface de laboratório.
2. Iniciar a captura e gerar tráfego de teste.
3. Aplicar o filtro `dns` e observar consultas e respostas.
4. Aplicar `icmp` e observar echo request/reply, quando houver ping.
5. Aplicar `tcp` e analisar portas, flags e estabelecimento de conexão.
6. Aplicar `tls` para observar metadados da negociação TLS.
7. Selecionar pacotes e registrar origem, destino, protocolo, portas e horário.
8. Salvar apenas uma captura reduzida e sanitizada, se apropriado.
9. Elaborar relatório explicando o que foi observado e o que permaneceu criptografado.

## Filtros úteis
```text
dns
icmp
tcp
tls
tcp.flags.syn == 1
ip.addr == 192.0.2.10
```
O IP acima é reservado para documentação. Substitua por endereço do seu laboratório.

## Perguntas de análise
- Qual consulta DNS foi observada? Houve resposta?
- Qual protocolo transportou os dados?
- Quais portas aparecem?
- O handshake TCP foi concluído?
- O que é possível observar no TLS?
- Há retransmissões, resets ou erros? Qual evidência sustenta a hipótese?

## Evidências
- `01-interface.png`
- `02-dns-filter.png`
- `03-icmp-filter.png`
- `04-tls-overview.png`
- `05-analysis-report.md`

## Resultado esperado
Relacionar pacotes aos protocolos de rede e explicar por que o conteúdo HTTPS não fica legível apenas por observar uma captura comum.

## Referências
- https://www.wireshark.org/docs/
- https://www.rfc-editor.org/
