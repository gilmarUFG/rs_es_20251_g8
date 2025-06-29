# Rastreabilidade e Análise de Consistência – HU_05

**User Story: HU_05 - Receber notificações sobre condições da plantação**

> **Como** agricultor usuário do sistema,  
> **Quero** receber notificações no meu celular sobre as condições da plantação, como temperatura e umidade,  
> **Para** poder agir rapidamente em caso de mudanças que possam afetar o cultivo.

## Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a          | Descrição / Observações                                         |
|------------------------|------------------------|------------------------------------------------------------------|
| HU_05 - Receber notificações sobre condições da plantação | HU_06 - Coleta de dados| HU_05 depende dos dados coletados para gerar notificações        |
| HU_05 - Receber notificações sobre condições da plantação             | UC - Monitoramento   | Notificações são geradas com base em condições monitoradas       |

## Análise de Consistência

- [x] Os dados estão disponíveis para envio das notificações?
- [x] O usuário pode configurar o tipo de notificação que deseja receber?
- [ ] Há fallback caso o celular esteja sem conexão?
- [ ] O sistema registra os envios de notificação?

### Recomendações:
- Definir mecanismos de envio em modo offline (ex: SMS).
- Criar histórico de notificações enviadas.