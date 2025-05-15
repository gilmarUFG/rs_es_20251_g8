### História de Usuário 09
ID: HU-009

### Título
Acionamento Automático da Irrigação por Baixa Umidade

### Descrição

Como **Agricultor**, eu quero que o sistema de irrigação seja acionado automaticamente quando os níveis de umidade do solo estiverem abaixo do ideal para que minhas culturas sejam irrigadas de forma otimizada, evitando o desperdicio hídrico e garantindo a irrigação da area sem minha intervenção manual constante.

### Critérios de Aceitação
### Cenário 1: Umidade do solo abaixo do limite ideal

**Dado que** os sensores de umidade do solo estão ativos e calibrados em um talhão ( talhão-> solo agrícola que  representa uma unidade mínima de cultivo de uma propriedade, geralmente definida em função de seu relevo e do planejamento da lavoura) específico.
E que o limite mínimo ideal de umidade para a cultura plantada nesse talhão está configurado no sistema
**Quando** o sensor detectar que o nível de umidade do solo está abaixo do limite ideal configurado
**Então** o sistema deve enviar um comando para acionar o sistema de irrigação correspondente àquele talhão ou zona de manejo.
E o sistema deve registrar o evento de acionamento (data, hora, talhão, nível de umidade detectado).

### Cenário 2: Sistema de irrigação acionado com sucesso
**Dado que** o sistema enviou um comando para acionar a irrigação
**Quando** o sistema de irrigação confirmar o início da operação
**Então** o sistema deve atualizar o status da irrigação para "Em andamento" para o talhão correspondente.
E o agricultor deve poder visualizar que a irrigação foi iniciada através da interface do sistema.

### Cenário 3: Umidade do solo atinge o nível ideal após irrigação
**Dado que** o sistema de irrigação está em funcionamento em um talhão
E que os sensores de umidade continuam monitorando o solo
**Quando** o sensor detectar que o nível de umidade do solo atingiu o patamar ideal (ou um limite superior configurado)
**Então** o sistema deve enviar um comando para desligar o sistema de irrigação correspondente.
E o sistema deve registrar o evento de desligamento e a duração da irrigação.

### Cenário 4: Falha no acionamento do sistema de irrigação
**Dado que** o sistema enviou um comando para acionar a irrigação
**Quando** o sistema de irrigação não confirmar o início da operação dentro de um tempo esperado (e.g., 5 minutos)
**Então** o sistema deve registrar a falha.

E o sistema deve enviar um alerta de falha ao agricultor (via SMS, e-mail ou notificação no app) informando sobre o problema no acionamento da irrigação no talhão específico.

### Prioridade
Alta

### Dependências
- Sensores de umidade do solo instalados e funcionando.
- Sistema de irrigação automatizado e integrado ao software de gestão.
- Módulo de configuração de limites ideais de umidade por cultura/talhão.
- Sistema de notificações para alertas de falha.

### Notas/Comentários Adicionais
O sistema deve permitir a configuração dos **níveis ideais de umidade (mínimo e máximo)** por talhão ou por tipo de cultura.
Considerar a possibilidade de o agricultor poder **desabilitar o acionamento automático** para talhões específicos temporariamente.
O sistema deve **registrar o volume de água utilizado em cada acionamento**, se o sistema de irrigação permitir essa medição.
