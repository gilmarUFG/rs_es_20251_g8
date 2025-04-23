# Área de Engenharia de Software

## Atividade Extraordinária - Aula 07: Técnicas para Especificação de Requisitos

### 1. Técnicas de Especificação de Requisitos

#### 1.1. Casos de Uso (Use Cases)

**Descrição:**
Casos de uso são uma técnica narrativa que descreve como os usuários finais (atores) interagem com o sistema para atingir um objetivo específico. Geralmente são representados com diagramas UML acompanhados de descrições textuais.

**Cenários de aplicação:**
Usado principalmente para sistemas interativos onde é importante documentar o comportamento do sistema a partir da perspectiva do usuário.

**Vantagens:**
- Fácil de entender por todos os stakeholders.
- Ajuda a identificar funcionalidades principais.
- Permite rastrear requisitos até os testes.

**Desvantagens:**
- Pode ser superficial para sistemas complexos.
- Pode se tornar repetitivo ou confuso se houver muitos casos similares.

#### 1.2. Especificação por Histórias de Usuário (User Stories)

**Descrição:**
É uma técnica comum em metodologias ágeis como o Scrum, onde os requisitos são descritos de forma simples e centrados no usuário. Seguem o formato: "Como [tipo de usuário], eu quero [objetivo] para que [benefício]".

**Cenários de aplicação:**
Projetos ágeis com entregas incrementais e iterações curtas.

**Vantagens:**
- Linguagem simples e acessível.
- Incentiva a colaboração entre desenvolvedores e stakeholders.
- Fácil de priorizar e estimar.

**Desvantagens:**
- Pode carecer de detalhamento técnico.
- Pode gerar interpretações diferentes se não houver validação.

---

### 2. Especificação de Requisitos do Cenário do Grupo

#### 2.1. Requisito A - Especificado com Casos de Uso

**Nome:** UC01 - Cadastro de Usuário

**Ator Principal:** Usuário visitante

**Descrição:** Permite que um novo usuário cadastre uma conta para acessar funcionalidades do sistema.

**Fluxo Principal:**
1. O usuário acessa a página de cadastro.
2. O sistema exibe o formulário.
3. O usuário preenche os dados obrigatórios (nome, email, senha).
4. O sistema valida os dados.
5. O sistema confirma o cadastro e redireciona para o login.

**Pós-condição:** O usuário está cadastrado no sistema.

#### 2.2. Requisito B - Especificado com História de Usuário

**ID:** US02

**História:**
> Como usuário autenticado, eu quero receber notificações de atualizações no sistema para que eu fique informado sobre novidades ou mudanças importantes.

**Critérios de aceitação:**
- O usuário deve poder ativar ou desativar as notificações.
- As notificações devem ser exibidas na interface e/ou enviadas por e-mail.

