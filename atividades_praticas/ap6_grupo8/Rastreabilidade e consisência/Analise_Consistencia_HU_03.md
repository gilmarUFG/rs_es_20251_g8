# ID – HU_03

**User Story: HU_03 - Sugestão de pontos críticos e melhorias com base em dados**

> **Como** agricultor/Gerente da Fazenda,  
> **Quero** receber sugestões de pontos críticos e melhorias com base nos dados coletados para que possa otimizar o manejo das minhas culturas e aumentar a produtividade, 
> **Para** otimizar o manejo das minhas culturas e aumentar a produtividade.

---

## Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a                | Descrição / Observações                                                                                   |
|------------------------|-----------------------------|------------------------------------------------------------------------------------------------------------|
| HU_03                  | R05 - Notificações no celular |                         | Envio de alertas diretamente ao agricultor, aumentando a eficiência da resposta a falhas ou anomalias.|
| HU_03                  | 	R06 - Coleta de dados do solo | Faz uso desses dados nas sugestões | Fonte primária de dados para detectar anomalias como baixa umidade ou pH fora do ideal.|
| HU_03                  | 	R02 - Relatórios sobre condições ambientais | Relatórios podem ser utilizados para sugestões melhores e/ou mais precisas |
| HU_03                  | 	R04 - Previsão e Otimização da produção agrícola com machine learning | Conceitos de machine learning podem ser reaproveitados para melhores sugestões |

## Análise de Consistência

- [x] Os dados coletados (solo, condições ambientais) são validades antes de serem usados para sugestões?
- [ ] As sugestões são personalizadas com base no tipo de cultura do agricultor?
- [ ] Existe um mecanismo para priorizar pontos críticos com base na severidade (e.g. baixa umidade crítica vs. pH ligeiramente fora do ideal)?
- [ ] As notificações enviadas ao agricultor são claras e acionáveis (incluem passos específicos para mitigação)?
- [ ] Há feedback do agricultor sobre a eficácia das sugestões para refinamento futuro?

### Recomendações HU_03:
- Implementar validação de dados de entrada (e.g., umidade, pH) no backend para garantir que apenas dados confiáveis sejam usados nas sugestões.
- Personalizar sugestões com base no tipo de cultura e nas condições específicas da fazenda, utilizando metadados do agricultor.
- Definir uma política de priorização para pontos críticos, como alertas baseados em thresholds configuráveis (e.g., umidade abaixo de 20% gera alerta de alta prioridade).
- Incluir nas notificações instruções claras e práticas (e.g., "Aumentar irrigação em 10% na área X devido à baixa umidade").
- Criar um mecanismo de feedback para que os agricultores avaliem as sugestões, permitindo ajustes no modelo de machine learning.
- Garantir que as notificações sejam enviadas em tempo real ou em horários configuráveis, com opção de escolha do canal (e.g., aplicativo, e-mail, SMS).