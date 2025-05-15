### História de Usuário 1
ID
HU-010

### Título
Registro e Rastreamento de Insumos Agrícolas 

### Descrição

Como **Agricultor/Gerente da Fazenda**, eu quero registrar e rastrear o uso de insumos (como fertilizantes, defensivos, sementes) por talhão ou zona de manejo específica para que possa gerenciar os custos de produção de forma eficaz, otimizar a aplicação de insumos e garantir a conformidade com regulamentações agrícolas e certificações.

### Critérios de Aceitação
### Cenário 1: Registro de uma nova aplicação de insumo

**Dado que** o usuário (Agricultor/Gerente) está logado no sistema
**Quando** ele selecionar a opção de registrar uma nova aplicação de insumo
**E**preencher as informações requeridas (tipo de insumo, quantidade, data da aplicação, talhão/zona de manejo, custo unitário/total, responsável pela aplicação)
**Então** o sistema deve salvar o registro da aplicação no banco de dados.
**E** o sistema deve exibir uma mensagem de confirmação do registro.
**E** o estoque do insumo utilizado (se o controle de estoque estiver ativo) deve ser atualizado.

###Cenário 2: Visualização do histórico de uso de insumos por talhão
**Dado que** o usuário está logado no sistema
**Quando** ele selecionar um talhão específico e solicitar o histórico de insumos aplicados
**Então** o sistema deve exibir uma lista ou relatório detalhando todas as aplicações de insumos naquele talhão, incluindo data, 
tipo de insumo, quantidade e custo.

### Cenário 3: Rastreamento de lote de insumo
**Dado que** foi registrado o uso de um insumo com informação de lote
**Quando** o usuário pesquisar por um lote específico de insumo
**Então** o sistema deve listar todos os talhões e datas em que aquele lote de insumo foi aplicado.

### Cenário 4: Geração de relatório de custos de insumos
**Dado que** existem registros de aplicação de insumos com informações de custo
**Quando**  usuário solicitar um relatório de custos de insumos para um período específico (e opcionalmente por talhão ou tipo de insumo)
**Então** o sistema deve gerar e apresentar um relatório sumarizando os custos totais e detalhados conforme os filtros aplicados.

### Prioridade
Alta

### Dependências
- Módulo de cadastro de talhões/zonas de manejo.
- Módulo de cadastro de tipos de insumos (com opção de unidade, custo, etc.).
- *Módulo de controle de estoque de insumos*.
- Funcionalidade de geração de relatórios.


### Notas/Comentários Adicionais
O sistema deve permitir anexar documentos aos registros de aplicação (ex: notas fiscais, recomendações agronômicas).
Considerar a integração com dados de planejamento de safra para prever o uso de insumos.
Facilitar o registro em campo, possivelmente através de um aplicativo móvel.
Permitir a exportação dos dados de uso de insumos (ex: para planilhas).
