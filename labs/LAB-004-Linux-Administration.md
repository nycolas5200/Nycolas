# LAB-004 — Linux Administration

**Área:** Sistemas operacionais · Linux · Fundamentos Blue Team  
**Repositório relacionado:** https://github.com/nycolas5200  
**Status:** consolidar este roteiro com o conteúdo e evidências do repositório de estudos.

## Objetivo
Praticar navegação, arquivos, permissões, usuários, processos, serviços, rede e análise básica de logs.

## Módulos e comandos
| Tema | Comandos |
|---|---|
| Sistema | `cat /etc/os-release`, `uname -a`, `hostnamectl` |
| Arquivos | `pwd`, `ls -la`, `cd`, `cp`, `mv`, `find` |
| Texto | `cat`, `less`, `head`, `tail`, `grep` |
| Permissões | `chmod`, `chown`, `umask` |
| Identidades | `id`, `whoami`, `groups`, `getent passwd` |
| Processos | `ps aux`, `top`, `pgrep` |
| Serviços | `systemctl status`, `start`, `stop` |
| Rede | `ip addr`, `ip route`, `ss -tulpen`, `ping` |
| Logs | `journalctl`, leitura autorizada de `/var/log` |
| Integridade | `sha256sum arquivo.txt` |

## Exercícios seguros
1. Criar usuário fictício e grupo de laboratório.
2. Criar diretório de teste e ajustar permissões.
3. Localizar processo e identificar seu usuário.
4. Consultar logs de inicialização e autenticação disponíveis.
5. Calcular hash de um arquivo, modificá-lo e comparar os hashes.

## Evidências
Registrar distribuição e versão, comando executado, finalidade e saída sanitizada. Não publicar hostname real, IP público ou dados privados.

## Resultado esperado
Demonstrar familiaridade com administração Linux e comandos úteis para troubleshooting, hardening e análise de eventos.

## Referências
- https://www.gnu.org/software/bash/manual/
- https://man7.org/linux/man-pages/
