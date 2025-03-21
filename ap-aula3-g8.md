Escolha um dos requisitos funcionais apresentados e
elabore uma especificação do mesmo destacando:

Requisito funcional: 
Coletar dados ambientais (temperatura, umidade, nível de irrigação) em tempo real.

1. Uma descrição detalhada do requisito;
  - Para realizar a coleta de dados do ambiente será necessário, implementar uma estação de coleta de dados. Essa estação 
será composta por sensores, GPS e outros perifericos para realizar a coleta de temperatura, umidade, nível de irrigação, 
condições do solo. Esses sensores ou equipamento enviam dados para a estação de coleta em tempo real, os dados são 
armazenados em um banco de dados não relacional.

2. Identificação das fontes dos requisitos;
  - Funcionários e proprietários de Fazendas, Gestores Agrícolas, 

3. Fluxos de execução;
  - Inicialização do sensor, ao primeiro uso ou em caso de reinicialização;
  - A coleta será feita em tempo real, sem intervalos ou interrupção;
  - O microcontrolador pode filtrar ruídos e detectar anomalias;
  - Envio imediato para a estação base, servidor ou nuvem via protocolo HTTP;
  - Armazenamento no banco de dados;
  - Processamento em tempo real, pode incluir análise de tendências e detecção de padrões;
  - Visualização dos dados em um dashboard web ou aplicativo;

4. Perfis de usuários com permissão de execução
  - Administrador(ao ligar o sensor)
