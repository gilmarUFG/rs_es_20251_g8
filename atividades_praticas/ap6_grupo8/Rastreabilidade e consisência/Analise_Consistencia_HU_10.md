# Rastreabilidade e Análise de Consistência – HU_10

**User Story: HU_10 - Registro e Rastreamento de Insumos Agrícolas**

> **Como** Agricultor/Gerente da Fazenda,  
> **Quero** registrar e rastrear o uso de insumos (como fertilizantes, defensivos, sementes) por talhão ou zona de manejo específica para que possa gerenciar os custos de produção de forma eficaz,  
> **Para** otimizar a aplicação de insumos e garantir a conformidade com regulamentações agrícolas e certificações.

---

## Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a                | Descrição / Observações                                                                                   |
|------------------------|-----------------------------|------------------------------------------------------------------------------------------------------------|
| HU_10 - Registro e Rastreamento de Insumos | R10 - Registro e rastreamento de insumos| Requisito funcional principal para gestão de insumos por talhão.|
| HU_10                  | Módulo de cadastro de talhões/zonas de manejo| Fundamental para associar registros de insumos a áreas específicas.|
| HU_10                  | Módulo de controle de estoque de insumos| Atualiza estoque com base nas aplicações registradas.|
| HU_10                  | Funcionalidade de geração de relatórios| Permite visualização e análise dos custos e uso de insumos.|

## Análise de Consistência

- [x] O registro de insumos está vinculado corretamente a talhões e lotes?  
- [x] O sistema atualiza o estoque automaticamente após registro?  
- [x] A geração de relatórios detalhados está contemplada?  
- [ ] Há tratamento de exceções para dados incorretos ou incompletos?
- [ ] Existe controle de permissões para quem pode registrar e editar aplicações? 
- [ ] A possibilidade de anexar documentos está prevista e funcional?  

### Recomendações HU_10:

- Implementar validação e tratamento de erros para garantir integridade dos dados.  
- Definir regras de permissão para garantir segurança e confiabilidade no registro de insumos.  
- Garantir funcionalidade robusta para anexar e consultar documentos relacionados às aplicações.  
