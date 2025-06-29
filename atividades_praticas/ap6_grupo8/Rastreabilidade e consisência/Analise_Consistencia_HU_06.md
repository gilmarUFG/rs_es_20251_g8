# Rastreabilidade e Análise de Consistência – HU_06

**User Story: HU_06 - Coleta de dados do solo**

> **Como** usuário do sistema de monitoramento agrícola,  
> **Quero** coletar dados do solo como umidade, pH e temperatura,  
> **Para** analisar as condições da plantação e apoiar ações corretivas ou preventivas.

## Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a          | Descrição / Observações                                         |
|------------------------|------------------------|------------------------------------------------------------------|
| HU_06 - Coleta de Dados| HU_05 - Receber notificações sobre condições da plantação   | Dados coletados são utilizados como gatilho para alertas         |
| HU_06 - Coleta de Dados| UC - Leitura de Sensores | Responsável pela obtenção das informações do solo            |

## Análise de Consistência

- [x] Os sensores usados são compatíveis com a plataforma?
- [ ] Há validação de dados coletados antes do uso?
- [ ] Existem políticas para dados faltantes ou inconsistentes?
- [ ] Os dados são armazenados com precisão temporal?

### Recomendações:
- Validar e armazenar dados com marcação de horário.
- Incluir lógica para lidar com falhas de sensores.
- Registrar erros de leitura para manutenção preventiva.