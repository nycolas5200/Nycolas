# LAB-003 — Windows Server & Active Directory

> Portfólio técnico de Nycolas Borges · Segurança da Informação, Redes e Infraestrutura

**Área:** Infraestrutura · Identidade · Segurança Windows  
**Status atual:** GUIA PREPARADO — executar em ambiente virtual isolado

## 1. Objetivo
Criar um domínio de teste e compreender AD DS, DNS, usuários, grupos, OUs, GPOs e eventos de autenticação.

## 2. Pré-requisitos
- VM Windows Server de avaliação
- VM Windows 10/11 Pro como cliente
- Rede interna/host-only
- IP privado estático no servidor e DNS do cliente apontando para ele

## 3. Procedimento passo a passo
1. Instalar Windows Server em VM isolada e atualizar.
2. Definir hostname, IP privado e DNS.
3. Adicionar a função Active Directory Domain Services pelo Server Manager.
4. Promover o servidor a controlador de domínio de uma floresta de laboratório, por exemplo lab.local.
5. Validar DNS e registros do domínio.
6. Criar OUs para usuários, computadores e grupos.
7. Criar contas fictícias e grupos com privilégio mínimo.
8. Ingressar a VM cliente no domínio.
9. Criar GPO simples e vinculá-la à OU de teste.
10. Executar gpupdate /force e validar com gpresult /r.
11. Consultar logs de autenticação no Event Viewer.
12. Documentar criação, alteração e desativação de uma conta de teste.

## 4. Conceitos e pontos de atenção
Comandos de validação: `ipconfig /all`, `nslookup lab.local`, `gpupdate /force`, `gpresult /r`, `whoami /all`. Cmdlets `Get-ADUser` e `Get-ADGroup` exigem o módulo ActiveDirectory e permissões adequadas. Não use senhas reais nem conecte o domínio à rede corporativa.

## 5. Evidências a registrar
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`

Crie a pasta `evidencias/` somente quando tiver arquivos reais para adicionar. Remova dados pessoais, endereços públicos, nomes de clientes, tokens, credenciais e qualquer informação corporativa.

## 6. Resultado esperado
Explicar a relação entre identidade, autenticação, DNS e políticas de grupo, além de localizar eventos úteis para investigação.

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
- https://learn.microsoft.com/windows-server/identity/ad-ds/

## 9. Transparência do portfólio
Este repositório diferencia estudo, roteiro e execução prática. Não declare o laboratório como concluído até executar as etapas, validar os resultados e incluir evidências próprias. Se uma etapa não puder ser realizada, documente a limitação.

## Documentação anterior
[Consultar a versão original em `labs/`](../labs/LAB-003-Windows-Server-AD.md)

[Voltar ao portfólio principal](../README.md) · [Site profissional](https://nycolas5200.github.io/Nycolas/)
