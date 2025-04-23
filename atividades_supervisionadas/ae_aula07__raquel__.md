\*\*Discente:\*\* \[202200031\_Raquel\]    
\*\*Disciplina:\*\* Requisitos de Software

\# Técnicas para Especificação de Requisitos

\#\# 1\. Pesquisa 

\#\#\# Técnica 1: Casos de Uso (Use Cases)

\*\*Descrição:\*\*    
Casos de uso são uma técnica de modelagem que descreve a interação entre atores (usuários ou sistemas externos) e o sistema, com o objetivo de alcançar um resultado específico. Cada caso de uso representa um fluxo de eventos que o sistema deve suportar.

\*\*Cenários de Aplicação:\*\*    
Muito utilizada em sistemas que envolvem múltiplas interações com usuários ou dispositivos, como sistemas de controle e monitoramento em tempo real, típicos de aplicações com IoT.

\*\*Vantagens:\*\*  
\- Facilita a comunicação com os stakeholders;  
\- Organiza os requisitos de forma clara e orientada a objetivos;  
\- Ajuda na definição de testes funcionais.

\*\*Desvantagens:\*\*  
\- Requer detalhamento adicional para cobrir requisitos não funcionais;  
\- Pode não ser suficiente sozinho em sistemas com lógica de negócios complexa.

\---

\#\#\# Técnica 2: Requisitos Funcionais em Linguagem Natural Estruturada

\*\*Descrição:\*\*    
Consiste na descrição dos requisitos utilizando linguagem natural, com frases padronizadas que indicam ações esperadas do sistema, como "O sistema deve..." ou "O sistema deverá...".

\*\*Cenários de Aplicação:\*\*    
Adequada em projetos onde há comunicação frequente com clientes e stakeholders não técnicos, sendo útil tanto em sistemas de gestão quanto em automação.

\*\*Vantagens:\*\*  
\- Fácil entendimento por todos os envolvidos no projeto;  
\- Rápida documentação;  
\- Útil para versões iniciais de requisitos.

\*\*Desvantagens:\*\*  
\- Pode ser ambígua se não for bem estruturada;  
\- Pouco formal para sistemas críticos ou altamente regulados.

\---

\#\# 2\. Especificação de Requisitos dos Cenários

\#\#\# Requisito A (Técnica: Casos de Uso)

\*\*Cenário:\*\* Sistema de Agricultura Inteligente com IoT

\*\*Nome:\*\* Monitoramento de Umidade do Solo

\*\*Ator Principal:\*\* Sensor IoT / Agricultor

\*\*Descrição:\*\*    
Este caso de uso descreve como o sistema de agricultura inteligente coleta dados de umidade do solo a partir de sensores IoT, e disponibiliza essas informações ao agricultor em tempo real.

\*\*Fluxo Principal:\*\*  
1\. O sensor coleta os dados de umidade em intervalos regulares.  
2\. Os dados são enviados ao sistema central via rede sem fio.  
3\. O sistema armazena e processa os dados recebidos.  
4\. O agricultor acessa o sistema por meio de um aplicativo ou plataforma web.  
5\. O sistema exibe os níveis atuais de umidade do solo por região monitorada.

\*\*Fluxo Alternativo:\*\*  
\- 2a. Se o sensor não conseguir enviar os dados, o sistema exibe um alerta de falha de comunicação.

\---

\#\#\# Requisito B (Técnica: Linguagem Natural Estruturada)

\*\*Cenário:\*\* Sistema de Gestão de Energia Inteligente

\*\*Requisito:\*\*    
O sistema deve permitir que o usuário acompanhe, em tempo real, o consumo de energia elétrica de cada equipamento conectado, exibindo gráficos comparativos por período (hora, dia, semana) e alertas de consumo excessivo.

\---

