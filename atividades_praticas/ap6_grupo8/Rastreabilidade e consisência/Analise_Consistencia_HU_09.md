# Rastreabilidade e Análise de Consistência – HU_09

**User Story: HU_09 - Acionamento Automático da Irrigação por Baixa Umidade**

> **Como** Agricultor,  
> **Quero** que o sistema de irrigação seja acionado automaticamente quando os níveis de umidade do solo estiverem abaixo do ideal para que minhas culturas sejam irrigadas de forma otimizada,  
> **Para** evitar o desperdicio hídrico garantindo a irrigação da area sem minha intervenção manual constante.

---

## Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a                | Descrição / Observações                                                                                   |
|------------------------|-----------------------------|------------------------------------------------------------------------------------------------------------|
| HU_09 - Acionamento Automático da Irrigação | R06 - Coleta de dados do solo (umidade)          | Depende da coleta dos dados de umidade para acionar a irrigação automaticamente.|
| HU_09                  | R09 - Acionamento automático do sistema de irrigação | Requisito funcional diretamente relacionado ao acionamento automático da irrigação baseado em umidade.|
| HU_09                  | R05 - Notificações no celular                         | Envio de alertas ao agricultor em caso de falha no acionamento da irrigação.|
| HU_09                  | Sistema de sensores e módulo de configuração          | Necessário para calibrar limites ideais de umidade e integração com sensores.|

## Análise de Consistência

- [x] A coleta de dados do sensor de umidade está contemplada e integrada?  
- [x] O sistema considera limites configuráveis por talhão/cultura?  
- [x] Existe tratamento para falhas no acionamento e notificações ao usuário?  
- [x] A integração com sistema de irrigação automatizado está prevista?  
- [ ] Há validação da calibração dos sensores antes do acionamento?  
- [ ] O registro do volume de água utilizado está previsto e validado?

### Recomendações HU_09:

- Implementar validação periódica da calibração dos sensores para garantir dados confiáveis.  
- Garantir registro do volume de água utilizado para controle.  
- Confirmar que alertas de falha sejam enviados em múltiplos canais conforme necessidade do usuário.
