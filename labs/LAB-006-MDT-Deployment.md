# LAB-006 — Microsoft Deployment Toolkit (MDT)

**Área:** Infraestrutura · Automação · Preparação de endpoints  
**Status:** roteiro preparado; validar compatibilidade antes de executar.

## Objetivo
Estudar implantação padronizada do Windows em VMs e compreender Deployment Share, imagens, drivers, aplicações, Task Sequence e Windows PE.

## Ambiente planejado
- VirtualBox.
- VM Windows Server para serviços/compartilhamento.
- VM cliente para teste.
- Mídia Windows obtida de fonte oficial.
- Windows ADK e Windows PE Add-on compatíveis com a versão escolhida.

## Componentes
- **Windows ADK:** ferramentas de avaliação e implantação.
- **Windows PE Add-on:** ambiente mínimo de inicialização.
- **Deployment Share:** estrutura central de arquivos e configurações.
- **Import Operating System:** importar os arquivos de instalação.
- **Out-of-Box Drivers:** organizar drivers.
- **Applications:** pacotes de aplicativos.
- **Task Sequence:** sequência de tarefas automatizadas.
- **Update Deployment Share:** atualizar arquivos e imagens de boot.

## Roteiro
1. Conferir compatibilidade e suporte atual das versões.
2. Preparar a VM servidora e o compartilhamento.
3. Instalar os componentes conforme documentação oficial.
4. Criar Deployment Share com permissões mínimas.
5. Importar o sistema operacional de teste.
6. Organizar drivers por modelo/arquitetura.
7. Adicionar aplicativos de laboratório.
8. Criar Task Sequence para instalação padrão.
9. Atualizar Deployment Share e gerar imagem de boot.
10. Inicializar a VM cliente pelo método suportado.
11. Executar implantação e validar sistema, drivers e aplicações.
12. Registrar erros e correções.

## Segurança e limitações
MDT é tecnologia legada. Confirme suporte e compatibilidade com as versões atuais antes de investir no laboratório. Não armazene senhas em scripts/configurações publicados e não exponha compartilhamentos à internet.

## Evidências
- `01-deployment-share.png`
- `02-task-sequence.png`
- `03-boot-image.png`
- `04-client-deployment.png`
- `05-validation.md`

## Resultado esperado
Compreender o fluxo de implantação padronizada e sua relação com configuração segura e gestão de endpoints.

## Referências
- https://learn.microsoft.com/windows/deployment/
- https://learn.microsoft.com/windows-hardware/get-started/adk-install
