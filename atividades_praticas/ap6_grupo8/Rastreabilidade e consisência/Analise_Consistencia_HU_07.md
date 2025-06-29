# Rastreabilidade e Análise de Consistência – HU_07

**User Story: HU_07 - Integrar visualização interativas com os dados coletados por sensores**
>**Como** Agricultor/Gerente da Fazenda  
> **Quero** visualizar em tempo real os dados dos sensores por meio de gráficos e mapas interativos
> **Para** tomar decisões rápidas e informadas com base nas condições do ambiente.

---

## Matriz de Rastreabilidade

## 📌 Matriz de Rastreabilidade

| **Requisito / User Story**                                   | **Relacionado a**             | **Descrição / Observações**                                                                 |
|--------------------------------------------------------------|-------------------------------|----------------------------------------------------------------------------------------------|
| HU-07 - Visualização de dados em tempo real                  | Cenário 1                     | Os gráficos e mapas devem refletir em tempo real os dados dos sensores. Requer uso de WebSockets ou MQTT e backend com timestamps confiáveis. |
| HU-07 - Mapa interativo com dados dos sensores               | Cenário 2                     | O usuário pode interagir com o mapa e visualizar localização, tipo e última leitura de cada sensor. Depende de geolocalização ativa e frontend com biblioteca de mapas. |
| HU-07 - Filtragem de dados por tipo, tempo e localização     | Cenário 3                     | Usuário pode aplicar filtros para refinar as visualizações. Requer backend preparado para consultas dinâmicas e frontend com atualização reativa. |
| HU-07 - Alerta de anomalias críticas via SMS ou e-mail       | Cenário 4                     | Ao detectar anomalias de alta severidade, o sistema deve enviar alertas em até 2 minutos. Requer sistema de detecção automatizada e integração com APIs de comunicação. |
| Requisito não funcional - Atualização em tempo real com baixa latência | Cenários 1, 2, 3         | Exige infraestrutura com baixa latência, idealmente com WebSocket/MQTT. Imprescindível para decisões rápidas. |
| Requisito não funcional - Responsividade em dispositivos móveis | Todos os cenários          | A interface deve ser acessível e funcional em smartphones e tablets, respeitando princípios de design responsivo. |
| Requisito não funcional - Escalabilidade do sistema          | Todos os cenários             | O sistema deve suportar crescimento no número de sensores, usuários e volume de dados, especialmente no pipeline de ingestão. |
| Requisito técnico - Banco de dados com suporte a séries temporais | Cenários 1 e 3             | Necessário para armazenar e consultar dados por período com eficiência. Facilita filtragens e visualizações. |
| Requisito técnico - Serviço de mapeamento geográfico         | Cenário 2                     | Fundamental para exibir corretamente a posição dos sensores no campo. Pode usar Mapbox, Leaflet, ou APIs de mapas. |
| Requisito técnico - Integração com serviços de notificação (SMS/email) | Cenário 4               | Obrigatório para envio de alertas em tempo hábil. Pode utilizar serviços como Twilio, SendGrid, etc. |




## Análise de Consistência

- [x] O objetivo de permitir decisões rápidas com dados em tempo real está bem definido? 
- [x] Todos os cenários (real-time, interação, filtro, anomalia) apoiam o objetivo da história? 
- [x] Cada critério pode ser validado por meio de testes funcionais e testes de integração? 
- [x] Os pré-requisitos (como conectividade dos sensores e uso de geolocalização) são condizentes com um sistema IoT?
- [x] A linguagem é clara; há uso de termos objetivos como "em tempo real", "última leitura", "dentro de 2 minutos".? 
- [ ] Requer validação se outras histórias cobrem o recebimento e armazenamento dos dados no backend. Pode haver dependência de outras funcionalidades‽
- [ ] Exige confirmação sobre suporte a WebSocket/MQTT no backend, integração com APIs de SMS/e-mail e escalabilidade do sistema? 
  

### Recomendações HU_07:

- Implementar WebSocket ou MQTT para streaming em tempo real, reduzindo a latência e evitando polling constante.  
- Utilizar um banco de dados com suporte a séries temporais (ex: InfluxDB, TimescaleDB) para otimizar consultas por período. 
- Aplicar bibliotecas de mapas como Leaflet ou Mapbox no frontend com integração dinâmica às localizações dos sensores.
- Adotar uma arquitetura orientada a eventos para detecção de anomalias e envio de alertas em tempo real.
- Manter documentação clara de APIs de visualização e alerta, com logs auditáveis para alertas críticos
