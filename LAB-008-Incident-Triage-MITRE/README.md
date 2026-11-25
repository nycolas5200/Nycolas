# LAB-008-Incident-Triage-MITRE

> Portfólio técnico de Nycolas Borges · Segurança da Informação, Redes e Infraestrutura

**Área:** SOC N1 · Triagem · Resposta inicial  
**Status atual:** ESTUDO DE CASO SINTÉTICO — não representa incidente real

## 1. Objetivo
Praticar triagem baseada em evidências, linha do tempo, hipóteses, classificação e escalonamento usando eventos fictícios.

## 2. Pré-requisitos
- Eventos sintéticos em CSV ou tabela
- Planilha ou editor de texto
- Referência MITRE ATT&CK

## 3. Procedimento passo a passo
1. Ler o conjunto de eventos fictícios.
2. Normalizar data e hora para UTC.
3. Agrupar eventos por host e usuário fictício.
4. Verificar quantidade e intervalo das falhas de autenticação.
5. Correlacionar as falhas com eventual evento de sucesso.
6. Considerar hipóteses alternativas, como erro de senha, automação ou tentativa indevida.
7. Listar informações adicionais necessárias para confirmar ou descartar hipóteses.
8. Mapear ATT&CK somente quando a técnica for sustentada pela evidência.
9. Classificar prioridade considerando impacto, probabilidade e criticidade do ativo.
10. Elaborar recomendação e escalonamento.

## 4. Conceitos e pontos de atenção
Cenário ilustrativo: falhas de autenticação em sequência seguidas de logon bem-sucedido. T1110 (Brute Force) pode ser uma hipótese de mapeamento, mas não deve ser atribuída sem evidência suficiente. Não confundir alerta com incidente confirmado.

## 5. Evidências a registrar
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`
- [ ] `evidencias/${x}`

Crie a pasta `evidencias/` somente quando tiver arquivos reais para adicionar. Remova dados pessoais, endereços públicos, nomes de clientes, tokens, credenciais e qualquer informação corporativa.

## 6. Resultado esperado
Produzir um relatório de triagem objetivo, distinguindo fatos confirmados, hipóteses, lacunas e ações recomendadas.

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
- https://attack.mitre.org/techniques/T1110/

## 9. Transparência do portfólio
Este repositório diferencia estudo, roteiro e execução prática. Não declare o laboratório como concluído até executar as etapas, validar os resultados e incluir evidências próprias. Se uma etapa não puder ser realizada, documente a limitação.

## Documentação anterior
[Consultar a versão original em `labs/`](../labs/LAB-008-Incident-Triage-MITRE.md)

[Voltar ao portfólio principal](../README.md) · [Site profissional](https://nycolas5200.github.io/Nycolas/)
