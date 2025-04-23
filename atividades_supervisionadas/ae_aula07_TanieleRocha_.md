# Técnicas para Especificação de Requisitos  
**Cenário:** Sistema de Agricultura Inteligente com IoT  

---
## 2. Técnicas de Especificação

### 2.1 Casos de Uso
Casos de Uso são representações que descrevem as interações entre atores (usuários ou sistemas) e o sistema em desenvolvimento para alcançar um objetivo.

#### Cenários de Aplicação
- Quando há necessidade de modelar fluxos complexos de interação
- Para sistemas com múltiplos atores e processos bem definidos
- Em projetos que requerem documentação formal para validação

#### Vantagens
- Fornece uma visão clara e estruturada das funcionalidades
- Facilita a identificação de requisitos não funcionais
- Ajuda na validação com stakeholders

#### Desvantagens
- Pode se tornar excessivamente detalhado para requisitos simples
- Requer manutenção contínua conforme o sistema evolui

### 2.2 Histórias de Usuário (User Stories)
São descrições concisas de funcionalidades escritas na perspectiva do usuário, seguindo o formato: "Como [ator], eu quero [ação] para que [benefício]".

#### Cenários de Aplicação
- Em metodologias ágeis como Scrum ou Kanban
- Quando se busca comunicação direta com a equipe de desenvolvimento
- Para priorização rápida de requisitos

#### Vantagens
- Fácil compreensão e priorização
- Flexível para adaptações durante o desenvolvimento
- Promove colaboração entre desenvolvedores e usuários

#### Desvantagens
- Pode faltar detalhamento em sistemas complexos
- Necessita de critérios de aceitação complementares

## 3. Aplicação das Técnicas

### 3.1 Caso de Uso: Detecção Automática de Pragas e Doenças
**Requisito:** O sistema deve permitir detecção de pragas e doenças: câmeras e sensores analisam padrões nas plantas e identificam problemas precocemente com IA.

**Ator Principal:** Agricultor  
**Pré-condições:** Câmeras e sensores IoT instalados na plantação  
**Fluxo Principal:**  
1. Sistema monitora plantas continuamente via sensores  
2. IA analisa padrões de cor e formato das folhas  
3. Em caso de anomalia, sistema registra ocorrência  
4. Agricultor recebe alerta no aplicativo  
**Fluxos Alternativos:**  
- Sem conexão: dados armazenados localmente e sincronizados posteriormente  
**Pós-condições:** Agricultor toma ações preventivas

### 3.2 História de Usuário: Irrigação Automatizada
**Requisito:** O sistema deve adaptar a irrigação do solo com base em previsões meteorológicas (umidade, chuva, seca).

**História:**  
"Como agricultor, quero que o sistema ajuste automaticamente a irrigação baseado na previsão do tempo para otimizar o uso de água e manter a saúde das plantas."

**Critérios de Aceitação:**  
- Consulta APIs meteorológicas diariamente  
- Reduz irrigação quando chuva é prevista  
- Aumenta irrigação em períodos de seca  
- Permite configuração manual de parâmetros  
- Notifica agricultor sobre ajustes realizados  
