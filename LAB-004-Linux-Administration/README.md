# LAB-004 — Linux Administration

> Portfólio técnico de Nycolas Borges · Segurança da Informação, Redes e Infraestrutura

**Área:** Sistemas operacionais · Linux · Fundamentos Blue Team  
**Status atual:** CONTEÚDO EM CONSOLIDAÇÃO — adicionar evidências próprias

## 1. Objetivo
Praticar navegação, arquivos, permissões, usuários, processos, serviços, rede e análise básica de logs.

## 2. Pré-requisitos
- Distribuição Linux em VM ou ambiente próprio
- Terminal com usuário autorizado
- Arquivos fictícios para os exercícios

## 3. Procedimento passo a passo
1. Identificar a distribuição com cat /etc/os-release, uname -a e hostnamectl.
2. Navegar por diretórios usando pwd, ls -la e cd.
3. Criar, copiar, mover e localizar arquivos com touch, cp, mv e find.
4. Consultar conteúdo com cat, less, head, tail e grep.
5. Praticar permissões com chmod, chown e umask em arquivos de teste.
6. Consultar identidades com id, whoami, groups e getent passwd.
7. Inspecionar processos com ps aux, top e pgrep.
8. Consultar serviços com systemctl status.
9. Verificar rede com ip addr, ip route e ss -tulpen.
10. Consultar logs com journalctl e arquivos autorizados em /var/log.
11. Calcular hash com sha256sum, modificar o arquivo e comparar os resultados.

## 4. Conceitos e pontos de atenção
Comandos úteis: `cat /etc/os-release`, `ls -la`, `grep`, `chmod`, `id`, `ps aux`, `systemctl`, `ip addr`, `ss -tulpen`, `journalctl`, `sha256sum`. Execute comandos administrativos somente quando compreender o efeito e tiver autorização.

## 5. Evidências a registrar
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`

Crie a pasta `evidencias/` somente quando tiver arquivos reais para adicionar. Remova dados pessoais, endereços públicos, nomes de clientes, tokens, credenciais e qualquer informação corporativa.

## 6. Resultado esperado
Demonstrar familiaridade com administração Linux e comandos úteis para troubleshooting, hardening e análise de eventos.

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
- https://man7.org/linux/man-pages/

## 9. Transparência do portfólio
Este repositório diferencia estudo, roteiro e execução prática. Não declare o laboratório como concluído até executar as etapas, validar os resultados e incluir evidências próprias. Se uma etapa não puder ser realizada, documente a limitação.

## Documentação anterior
[Consultar a versão original em `labs/`](../labs/LAB-004-Linux-Administration.md)

[Voltar ao portfólio principal](../README.md) · [Site profissional](https://nycolas5200.github.io/Nycolas/)
