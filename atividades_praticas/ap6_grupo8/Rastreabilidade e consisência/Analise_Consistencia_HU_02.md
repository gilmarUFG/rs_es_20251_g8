# Rastreabilidade e Análise de Consistência – HU_02

**User Story: HU_02 - Relatórios sobre Condições Ambientais**

> **Como** Gerente da Fazenda ou Técnico Responsável,  
> **Quero** visualizar relatórios com informações sobre as condições do ambiente (como umidade, temperatura, pH, etc.) em um período definido, 
> **Para** monitorar a saúde do ambiente agrícola, tomar decisões baseadas em dados e melhorar o planejamento das atividades no campo.

---

## Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a                | Descrição / Observações                                                                                   |
|------------------------|-----------------------------|------------------------------------------------------------------------------------------------------------|
| HU_02 - Relatórios ambientais por período | R02 - Relatórios sobre as condições do ambiente em um determinado período.| Dados de sensores (umidade, temperatura, pH) são a base para os relatórios.|
| HU_02                  | 	R08 - Visualização interativa de dados | Os relatórios podem ser exibidos graficamente (linha do tempo, mapas de calor, comparações).|
| HU_02                 | 	R03 - Previsão e otimização da produção | Algoritmos de ML e estatística podem alimentar o sistema para produzir relatórios com bases em parametros de eficiência e falhas.|

## Análise de Consistência

- [x] O sistema coleta dados com frequência e precisão suficientes para compor os relatórios?
- [x] É possível filtrar os dados por período (diário, semanal, mensal, personalizado)? 
- [x] Os dados exibidos são provenientes de fontes confiáveis (sensores, registros manuais verificados)?
- [ ] Há suporte para exportar os relatórios em formatos como PDF ou Excel?
- [ ] O sistema oferece visualizações gráficas (ex: linha do tempo, média por dia)?
- [ ] Existe um painel histórico de relatórios já gerados?  
- [ ] Os relatórios podem ser gerados automaticamente ou agendados?

### Recomendações HU_02:

- Incluir filtros por área da fazenda, tipo de sensor e intervalo de tempo na interface do relatório.
- Exibir gráficos de linha, barras ou mapa de calor para facilitar a análise visual dos dados.
- Permitir exportação dos relatórios em formatos PDF, Excel e CSV.
- Adicionar médias, mínimas, máximas e variações por período no relatório.
- Implementar agendamento de geração automática de relatórios com envio por e-mail.
- Criar histórico acessível de relatórios para auditoria e comparação de dados entre períodos. 