# Rastreabilidade e Análise de Consistência – HU_08

**User Story: HU_08 - Registro e Rastreamento de Insumos Agrícolas**

> **Como** Agricultor/Gerente da Fazenda,  
> **Quero**  personalizar os alertas e relatórios conforme o tipo de cultivo, fase da planta e meu perfil, 
> **Para** que eu possa tomar decisões rápidas e relevantes com base nas condições ambientais específicas.

---

## 📌 Matriz de Rastreabilidade - HU-08

| **Requisito / User Story**                                           | **Relacionado a**               | **Descrição / Observações**                                                                 |
|----------------------------------------------------------------------|----------------------------------|----------------------------------------------------------------------------------------------|
| HU-08 - Configuração de alertas personalizados                       | Cenário 1                        | Usuário define regras por cultivo, fase da planta e parâmetros ambientais. Requer sistema de regras dinâmicas. |
| HU-08 - Relatórios personalizados por perfil                         | Cenário 2                        | Relatórios são formatados de acordo com o tipo de usuário (ex: técnico ou agrônomo). Depende de perfis bem definidos. |
| HU-08 - Filtragem de dados                                           | Cenário 3                        | Usuário filtra por tipo de sensor, tempo e localização. Compartilhado com outras histórias; exige backend com filtros dinâmicos. |
| HU-08 - Notificações relevantes por perfil e configuração            | Cenário 4                        | Envio de alerta apenas a usuários com regras correspondentes. Requer lógica condicional associada a perfis e regras salvas. |
| Requisito técnico - Cadastro estruturado de cultivos e fases         | Cenários 1, 2, 4                 | Essencial para personalização baseada em cultura e fase. Deve ser estruturado e editável. |
| Requisito técnico - Sistema de perfis e permissões configuráveis     | Cenários 2 e 4                   | Usuários precisam ter perfis distintos e preferências salvas para customização de relatórios e alertas. |
| Requisito técnico - Armazenamento de configurações personalizadas    | Cenários 1, 4                    | Recomenda-se o uso de JSON em banco relacional ou NoSQL para regras flexíveis por usuário. |
| Requisito técnico - Sistema de notificações por múltiplos canais     | Cenário 4                        | Notificações devem suportar envio via e-mail, SMS ou push, conforme configuração do usuário. |
| Requisito não funcional - Escalabilidade da lógica de regras         | Todos os cenários                | O sistema deve ser capaz de lidar com centenas de regras simultâneas sem impacto em performance. |
| Requisito não funcional - Usabilidade da interface de configuração   | Cenários 1 e 2                   | A configuração de alertas e visualização de relatórios deve ser clara, intuitiva e acessível. |


## Análise de Consistência

- [x] O objetivo é personalizar alertas e relatórios conforme cultivo, fase da planta e perfil do usuário?  
- [x] Os quatro cenários tratam da personalização e entrega direcionada de informações?  
- [x] Todos os critérios podem ser testados funcionalmente (ex: regras de alerta, filtros, geração de relatórios)?  
- [x] A história é coerente e não entra em conflito com funcionalidades esperadas do sistema?
- [x] Requisitos como cadastro de cultivos, fases da planta, perfis e sistema de regras são indicados? 
- [ ] Exige estrutura flexível para armazenar regras dinâmicas (uso de JSON, banco NoSQL) e lógica condicional complexa para envio seletivo de notificações?
- [x] O cenário 3 é reutilizado, mas com foco diferente, reforçando a filtragem como requisito transversal.s?


### Recomendações HU_08:

- Permitir que usuários com permissões específicas gerenciem regras globais para suas equipes. 
- Registrar o envio de notificações para rastreamento de alertas e análise posterior.
- Permitir que o usuário escolha o canal preferido e defina limites de frequência.
- Defina perfis de usuário com permissões e formatos de relatórios específicos.
