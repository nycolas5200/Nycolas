# LAB-003 — Windows Server & Active Directory

**Área:** Infraestrutura · Identidade · Segurança Windows  
**Status:** guia preparado; executar em ambiente virtual isolado.

## Objetivo
Criar um domínio de teste e compreender AD DS, DNS, usuários, grupos, OUs, GPOs e eventos de autenticação.

## Topologia
- VM Windows Server de avaliação.
- VM Windows 10/11 Pro como cliente.
- Rede interna/host-only.
- IP privado estático no servidor e DNS do cliente apontando para o servidor.

## Etapas
1. Instalar Windows Server em VM isolada e atualizar.
2. Definir hostname, IP privado e DNS.
3. Adicionar a função Active Directory Domain Services pelo Server Manager.
4. Promover o servidor a controlador de domínio de uma floresta de laboratório (ex.: `lab.local`).
5. Validar DNS e registros do domínio.
6. Criar OUs para usuários, computadores e grupos.
7. Criar contas fictícias e grupos com privilégio mínimo.
8. Ingressar a VM cliente no domínio.
9. Criar uma GPO simples, vinculá-la à OU de teste e executar `gpupdate /force`.
10. Validar com `gpresult /r`.
11. Consultar logs de autenticação no Event Viewer.
12. Documentar criação, alteração e desativação de uma conta de teste.

## Comandos
```powershell
ipconfig /all
nslookup lab.local
gpupdate /force
gpresult /r
whoami /all
Get-ADUser -Filter *
Get-ADGroup -Filter *
```
Os cmdlets Get-AD exigem o módulo ActiveDirectory e permissões adequadas.

## Boas práticas
- Não usar senhas reais.
- Não conectar o domínio de laboratório à rede corporativa.
- Evitar utilizar Domain Admin em tarefas comuns.
- Registrar alterações e manter o ambiente isolado.

## Evidências
- `01-server-manager.png`
- `02-ad-users-and-computers.png`
- `03-domain-joined-client.png`
- `04-gpo-result.png`
- `05-event-viewer.png`

## Resultado esperado
Explicar a relação entre identidade, autenticação, DNS e políticas de grupo, além de localizar eventos úteis para investigação.

## Referências
- https://learn.microsoft.com/windows-server/identity/ad-ds/
- https://learn.microsoft.com/windows-server/administration/windows-commands/gpresult
