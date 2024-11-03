## 1. Visão Geral do Sistema
Objetivo: Criar uma experiência de uso prática e agradável, permitindo que os usuários gerenciem seus livros sem dificuldades, minimizando desistências devido a processos complexos. O sistema oferecerá ao administrador uma plataforma de controle completo para gerenciamento de livros, usuários, empréstimos, devoluções e notificações de atrasos.

Funcionalidades Principais:
- Navegação de fácil identificação
- Carteira e histórico de livros solicitados
- Reserva online
- Notificações de atraso
- Pagamento Seguro: Integração de um sistema de pagamento que garante transações seguras para usuários ao realizar reservas ou pagar por multas.

## 2. Componentes do Sistema
1. **Frontend (React):**
   - O React será utilizado para construir a interface do usuário, oferecendo uma interface interativa e amigável, com componentes reutilizáveis.

2. **Backend (Node.js com Express.js):**
   - O backend será construído em Node.js, utilizando o framework Express.js para criar uma API robusta.

3. **Banco de Dados (MySQL com Sequelize):**
   - Usaremos o MySQL como sistema de gerenciamento de banco de dados relacional, com Sequelize como ORM para facilitar o acesso e manipulação de dados.

4. **Testes da API (Postman/Insomnia):**
   - Utilizaremos Postman e Insomnia para testar a API, garantindo que todas as rotas funcionem corretamente.

5. **Controle de Versão (Git e GitHub):**
   - O Git será usado para controle de versão e o GitHub para colaboração entre os membros da equipe.

6. **Transporte por Terceiros:**
   - Integração com serviços de transporte, permitindo que os usuários solicitem o transporte de itens e rastreiem suas encomendas.

7. **Gerenciamento:**
   - Interface dedicada para gerenciar usuários, empréstimos, reservas e transportes, com funcionalidades para administração de usuários.

8. **Pagamento Seguro:**
   - Integração de uma solução de pagamento que permite transações seguras para reservas de livros e pagamentos de multas.

## 3. Interações entre Componentes
- O usuário abre o site e acessa a página inicial.
- O usuário realiza uma pesquisa; o frontend solicita dados ao backend.
- O backend retorna livros disponíveis, que são exibidos no frontend.
- O usuário seleciona um livro e solicita a reserva.
- O backend verifica a disponibilidade e atualiza o banco de dados.
- O usuário realiza o pagamento seguro da reserva ou multa.
- O sistema envia alertas sobre livros atrasados.
- O administrador registra novos livros e gerencia usuários.
- Coleta de opiniões para melhorar a experiência.

## 4.1 Frontend
Decisão: Usar React como framework para o frontend.
Justificativa: O React permite a criação de interfaces dinâmicas e interativas, melhorando a experiência do usuário.

## 4.2 Backend
Decisão: Utilizar Node.js com Express.js para o backend.
Justificativa: Essa combinação é ideal para construir APIs escaláveis e robustas.

## 4.3 Banco de Dados
Decisão: Optar pelo MySQL como banco de dados relacional.
Justificativa: O MySQL garante a integridade dos dados e é confiável para gerenciar relações complexas.

## 4.4 ORM
Decisão: Utilizar Sequelize como ORM.
Justificativa: O Sequelize simplifica a interação com o banco de dados, permitindo que os desenvolvedores trabalhem com objetos.

## 4.5 Testes de API
Decisão: Escolher Postman e Insomnia para testes de API.
Justificativa: Ambas as ferramentas são intuitivas e eficazes para validar se todas as rotas da API estão funcionando corretamente.

## 4.6 Controle de Versão
Decisão: Usar Git e GitHub para controle de versão.
Justificativa: O Git permite gerenciar as alterações no código de forma eficiente.

## 4.7 Integração com Serviços de Transporte
Decisão: Integrar serviços de transporte no sistema.
Justificativa: Isso permitirá que os usuários solicitem transporte de itens e rastreiem suas encomendas.

## 4.8 Gerenciamento de Usuários
Decisão: Criar uma interface dedicada para o gerenciamento de usuários.
Justificativa: Essa interface é crucial para permitir que administradores gerenciem permissões.

## 4.9 Pagamento Seguro
Decisão: Integrar uma solução de pagamento seguro, como PayPal ou Stripe.
Justificativa: Isso oferece segurança nas transações financeiras e aumenta a confiança dos usuários.

## 5. Requisitos e Restrições
### Requisitos Funcionais:
- O sistema deve permitir que administradores cadastrem livros e usuários, além de gerenciar suas informações.
- Deve facilitar a realização de empréstimos e reservas de livros, com atualizações automáticas de disponibilidade.
- É necessário enviar notificações sobre atrasos e permitir pagamentos seguros de multas.
- O sistema deve fornecer acesso a relatórios e estatísticas sobre o uso, como empréstimos e reservas.

### Requisitos Não Funcionais:
- O sistema deve garantir que operações críticas sejam concluídas em até 2 segundos, suportando até 100 usuários simultâneos.
- É fundamental proteger dados sensíveis com criptografia e implementar autenticação robusta.
- A interface deve ser amigável e intuitiva, facilitando a navegação dos usuários.
- O sistema deve ser escalável e compatível com diferentes dispositivos e navegadores, assegurando uma experiência consistente.

## Diretrizes para Documentação
- **Consistência:** A documentação deve ser escrita de forma consistente para facilitar o entendimento.
- **Atualização Contínua:** A documentação deve acompanhar as mudanças no software. Se o sistema evolui, a documentação deve refletir essas mudanças.
- **Modularidade:** Documente cada parte do sistema de forma modular e coesa, facilitando a leitura e manutenção.
