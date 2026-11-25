# LAB-006-MDT-Deployment

> Portfólio técnico de Nycolas Borges · Segurança da Informação, Redes e Infraestrutura

**Área:** Infraestrutura · Automação · Preparação de endpoints  
**Status atual:** ROTEIRO PREPARADO — validar compatibilidade antes da execução

## 1. Objetivo
Estudar implantação padronizada do Windows em VMs e compreender Deployment Share, imagens, drivers, aplicações, Task Sequence e Windows PE.

## 2. Pré-requisitos
- VirtualBox
- VM Windows Server para serviços/compartilhamento
- VM cliente para teste
- Mídia Windows obtida de fonte oficial
- Windows ADK e Windows PE Add-on compatíveis com a versão selecionada

## 3. Procedimento passo a passo
1. Conferir compatibilidade e suporte atual das versões antes da instalação.
2. Preparar a VM servidora e o compartilhamento.
3. Instalar componentes conforme a documentação oficial aplicável.
4. Criar Deployment Share com permissões mínimas.
5. Importar o sistema operacional de teste.
6. Organizar drivers por modelo e arquitetura.
7. Adicionar aplicativos de laboratório.
8. Criar Task Sequence para instalação padrão.
9. Atualizar Deployment Share e gerar imagem de boot.
10. Inicializar a VM cliente pelo método suportado.
11. Executar implantação e validar sistema, drivers e aplicações.
12. Registrar erros e correções.

## 4. Conceitos e pontos de atenção
ADK reúne ferramentas de avaliação e implantação; WinPE fornece ambiente mínimo de inicialização; Deployment Share organiza conteúdo; Task Sequence automatiza etapas. MDT é tecnologia legada: confirme compatibilidade e suporte antes de investir no laboratório. Não publique senhas ou exponha compartilhamentos à internet.

## 5. Evidências a registrar
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`

Crie a pasta `evidencias/` somente quando tiver arquivos reais para adicionar. Remova dados pessoais, endereços públicos, nomes de clientes, tokens, credenciais e qualquer informação corporativa.

## 6. Resultado esperado
Compreender o fluxo de implantação padronizada e sua relação com configuração segura e gestão de endpoints.

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
- https://learn.microsoft.com/windows/deployment/

## 9. Transparência do portfólio
Este repositório diferencia estudo, roteiro e execução prática. Não declare o laboratório como concluído até executar as etapas, validar os resultados e incluir evidências próprias. Se uma etapa não puder ser realizada, documente a limitação.

## Documentação anterior
[Consultar a versão original em `labs/`](../labs/LAB-006-MDT-Deployment.md)

[Voltar ao portfólio principal](../README.md) · [Site profissional](https://nycolas5200.github.io/Nycolas/)
