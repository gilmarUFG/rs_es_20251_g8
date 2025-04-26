Técnicas para Especificação de Requisitos

1. Casos de Uso (Use Cases)
A técnica de Casos de Uso, faz uso de  narrativas que descrevem como os usuários (ou atores) interagem com o 
sistema para atingir um objetivo específico. É uma especificação ideal para entender e comunicar como o sistema
será utilizado no dia a dia, especialmente em sistemas com forte interação usuário-sistema ou sistema-sistema.

Sua princípal vantagem é o relacionamento que promove um  entendimento claro entre desenvolvedores
e stakeholders. Ajudando a identificar interações completas, incluindo exceções e fluxos alternativos. Sua principal 
desvantagem é :  Pouco eficiente para detalhar requisitos não-funcionais e pode se tornar complexo em sistemas muito 
grandes.

2. Especificação por Requisitos Funcionais (IEEE 830)
A técnica descreve requisitos funcionais de forma clara, estruturada e numerada, geralmente em linguagem natural 
e formalizada. Fonece uma boa documentação formal, rastreabilidade e comunicação entre equipes técnicas e é muito 
fácil de escrever e compreender. Permite boa organização e rastreamento de mudanças, se bem estruturado reduz a 
ambiguidade. Sua principal desvantagem é : Pode ser ambígua se mal escrita e menos intuitiva para usuários não 
técnicos.

Especificação de Requisitos – Cenário: Sistema de Agricultura Inteligente com IoT

Requisito A – Técnica: Casos de Uso
Caso de Uso: Identificar Pragas via Aerolevantamento
Ator Primário: Drone com câmera multiespectral
Descrição: Este caso de uso descreve como o sistema realiza aerolevantamento com drones e aplica técnicas de 
fotogrametria para identificar pragas localizadas nas plantações.

Fluxo Principal:

O usuário agenda uma missão de sobrevoo no sistema.
O drone realiza o voo autônomo sobre a plantação.
Durante o voo, o drone captura imagens com câmera multiespectral.
O sistema processa as imagens aplicando fotogrametria e algoritmos de detecção de pragas.
O sistema identifica áreas com possíveis pragas e atualiza o mapa da plantação com essas informações.

Fluxos Alternativos:

2a. Caso o drone não decole por problemas técnicos, o sistema notifica o usuário.
4a. Se as imagens estiverem corrompidas ou com baixa qualidade, o sistema solicita novo sobrevoo.


Requisito B – Técnica: Especificação por Requisitos Funcionais (IEEE 830)
Especificação por Requisitos Funcionais: Previsão de Pragas e Otimização Agrícola
Descrição: O sistema deve utilizar algoritmos de inteligência artificial para prever
a incidência de pragas com base em dados históricos, condições climáticas e imagens capturadas,
além de recomendar práticas agrícolas otimizadas e estratégias de irrigação eficientes.

Justificativa: Reduz prejuízos com infestações e aumenta a eficiência no uso de recursos.
Prioridade: Alta
Critério de Aceitação:

O sistema deve apresentar previsões com pelo menos 80% de acurácia em testes com dados reais.

As recomendações devem estar disponíveis em painel para o usuário após o processamento dos dados.
Dependências: RF-05 (Coleta de dados climáticos e históricos).

