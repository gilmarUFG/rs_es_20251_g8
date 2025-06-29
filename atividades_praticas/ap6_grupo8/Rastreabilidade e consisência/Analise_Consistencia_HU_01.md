# Rastreabilidade e Análise de Consistência – HU_01

**User Story: HU_01 - Alerta de Anomalias em Aplicações de Insumos**

> **Como** Gerente da Fazenda ou Técnico Responsável,  
> **Quero** receber alertas automáticos quando forem detectadas anomalias nas aplicações de insumos (ex: dosagem incorreta, aplicação fora da área ou do período planejado), 
> **Para** agir rapidamente, evitar desperdícios, reduzir riscos ambientais e garantir conformidade com normas técnicas.

---

## Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a                | Descrição / Observações                                                                                   |
|------------------------|-----------------------------|------------------------------------------------------------------------------------------------------------|
| HU_01 - Sistema de detecção e alerta de anomalias | R01 - Sistema de detecção e alerta de anomalias| Requisito funcional principal para detecção e alerta de anomalias.|
| HU_01                  | R05 - Notificações no celular |                         | Envio de alertas diretamente ao agricultor, aumentando a eficiência da resposta a falhas ou anomalias.|
| HU_01                  | R07 - Personalização de alertas |Permite ao usuário ajustar os parâmetros de detecção e os tipos de notificação conforme cultura e perfil. |
| HU_01                  | 	R06 - Coleta de dados do solo |Funcionalidade de geração de relatórios| Fonte primária de dados para detectar anomalias como baixa umidade ou pH fora do ideal.|
| HU_01                  | 	R09 - Acionamento automático de irrigação | Pode ser consequência de um alerta de anomalia (ex: umidade crítica ativa irrigação automaticamente).|
| HU_01                  | 	R02 - Relatórios sobre condições ambientais | Apoio na validação de alertas por meio de relatórios com dados históricos e contexto temporal.|
| HU_01                  | 	R08 - Visualização interativa de dados | Exibição em tempo real de dados com destaque visual de anomalias detectadas.|
| HU_01                  | 	R04 - Sugerir pontos críticos/melhorias | Pode ser complementado por alertas automáticos com base em análise dos dados e aprendizado de máquina.|
| HU_01                  | 	R03 - Previsão e otimização da produção | Algoritmos de ML e estatística podem alimentar o sistema de detecção de anomalias com previsões mais precisas.|

## Análise de Consistência

- [x] O sistema possui base de dados suficiente (aplicações, doses, horários) para comparar com padrões esperados?
- [x] Há integração com sensores ou entrada manual estruturada para permitir análise confiável? 
- [x] Existem regras definidas para o que constitui uma “anomalia” (ex: tolerância de erro na dose)? 
- [ ] O sistema diferencia tipos de anomalias (críticas, leves)?
- [ ] O usuário pode configurar os parâmetros de alerta (ex: limites aceitáveis)? 
- [ ] Existem logs ou relatórios que documentem os alertas gerados?  
- [ ] O sistema impede notificações duplicadas ou falsas positivas de forma eficiente?

### Recomendações HU_01:

- Definir critérios e limiares claros de anomalias, com possibilidade de ajuste por tipo de cultura, insumo ou zona de manejo.
- Implementar sistema de níveis de alerta, com criticidade (ex: aviso, alerta urgente).
- Incluir painel de histórico de alertas e justificativas registradas, para rastreabilidade e auditoria.
- Garantir integração entre alertas e módulos de registro de insumos, para facilitar a verificação e correção dos problemas identificados.
- Adicionar filtros e opções de personalização de alertas para reduzir falsos positivos e melhorar a experiência do usuário.