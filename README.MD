
# WorkNexus - Plataforma de Aluguel de Salas
A flexibilidade no uso de espaços de trabalho é uma demanda crescente, especialmente para profissionais autônomos ou pequenos negócios. A utilização de tecnologia para mediar e controlar o acesso às salas individuais de forma fácil e segura durante o período contratado é essencial para oferecer conveniência e segurança aos usuários. Com isso, oferecemos um serviço que conecta locatários com imóveis perfeitos para a demanda de cada profissional.

## Identificação dos Processos

### Cadastro e Verificação de Usuários
- Criação de contas para profissionais com verificação de identidade.
- Validação de documentos como CRM, OAB, entre outros.

### Cadastro e Verificação das Locações
- Verificação dos imóveis.
- Validação dos documentos da residência.

### Reserva de Salas
- Navegação e seleção de salas disponíveis no app ou site por necessidade e disponibilidade.
- Reserva da sala por um período específico, com pagamento antecipado.
- Emissão de QR code ou configuração de acesso biométrico para o horário reservado.

### Gerenciamento de Acessos e Segurança
- Controle de acesso à sala via QR code ou biometria, ativado apenas durante o período de reserva.
- Monitoramento em tempo real do uso da sala e desativação automática do acesso após o término do período.
- Retenção de um documento do profissional e do visitante durante a permanência.

### Pagamentos e Faturamento
- Processamento de pagamentos online para reservas de salas.
- Emissão de faturas digitais e gestão de políticas de cancelamento.

### Política de Cancelamento
- Gestão de reembolsos ou créditos em caso de cancelamento dentro do prazo permitido.
- Reembolso varia de acordo com cada locatário.

### Manutenção, Suporte e Limpeza
- Solicitação de serviços de manutenção ou limpeza após o uso da sala (equipes do locatário ou mediante a pagamento de taxas com equipe do app).
- Monitoramento da qualidade das salas com inspeções regulares.
- Suporte técnico para problemas com o sistema de acesso.

### Avaliações e Feedback dos Usuários
- Sistema de avaliação das salas e da experiência geral, com feedback focado em segurança, limpeza e conforto a cada vez que for locado o espaço.
- Sistema de avaliação a longo prazo com 30, 60 e 90 dias.
- Utilização do feedback para melhorar continuamente os serviços oferecidos.

![Diagrama](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Diagramas/WorkNexus.jpg)

### Modelo de Desenvolvimento

**Kanban**

Kanban é um termo japonês que significa “cartão” ou “sinalização”. Assim, o método Kanban se resume a uma forma de gestão visual que irá controlar o fluxo de trabalho através da utilização de cartões e colunas coloridas.

A ideia é que, conforme as atividades forem executadas, os cartões são movidos de coluna, permitindo ao gestor acompanhar o progresso do projeto e identificar a capacidade de novas demandas.

Dessa forma, escolhemos essa metodologia para desenvolvermos nosso negócio pois é flexivel e adaptável, permitindo ajustes contínuos e conforme necessário. Junto a isso, o método impõe limites ao numero de tarefas em progresso visando evitar sobrecargas e melhorar a eficiência.

### Stakeholders

**Internos:**
1. **Equipe de Desenvolvimento**: Responsável pela criação e manutenção da plataforma.
2. **Equipe de Suporte Técnico**: Responsável por resolver problemas técnicos e garantir que a plataforma esteja funcionando adequadamente.
3. **Equipe de Atendimento ao Cliente**: Auxilia os usuários com questões relacionadas a reservas, pagamentos e outros problemas.
4. **Equipe de Operações e Manutenção**: Gerencia a manutenção dos imóveis e a limpeza das salas.
5. **Equipe de Marketing e Vendas**: Trabalha na promoção da plataforma e na aquisição de novos locatários e profissionais.

**Externos:**
1. **Locatários**: Proprietários ou gestores de imóveis que disponibilizam salas para alugar.
2. **Profissionais e Usuários**: Pessoas que alugam as salas para seus trabalhos ou reuniões.
3. **Prestadores de Serviços de Limpeza e Manutenção**: Fornecedores que cuidam da manutenção e limpeza das salas.
4. **Entidades de Verificação**: Organizações responsáveis pela validação de documentos e identidade dos usuários.

## Requisitos Funcionais e Não Funcionais

### Requisitos Funcionais

- **RF01 - Cadastro e Verificação de Usuários:**
  - **RF01.01**: O sistema deve permitir a criação de contas para novos usuários, exigindo informações pessoais e profissionais.
  - **RF01.02**: O sistema deve validar a identidade dos usuários enviando um código de verificação para o e-mail ou telefone fornecido.
  - **RF01.03**: O sistema deve solicitar e verificar documentos de identidade e registros profissionais, como CRM ou OAB.

- **RF02 - Cadastro e Verificação das Locações:**
  - **RF02.01**: O sistema deve permitir que locatários registrem novos imóveis para aluguel, incluindo detalhes do imóvel e documentos de propriedade.
  - **RF02.02**: O sistema deve realizar a verificação dos imóveis cadastrados, validando os documentos de posse ou autorização para locação.

- **RF03 - Reserva de Salas:**
  - **RF03.01**: O sistema deve exibir uma lista de salas disponíveis com base nas necessidades e disponibilidade especificadas pelo usuário.
  - **RF03.02**: O sistema deve permitir que o usuário selecione uma sala e realize a reserva para um período específico.
  - **RF03.03**: O sistema deve processar o pagamento antecipado da reserva e emitir um QR code ou configurar o acesso biométrico para o período reservado.

- **RF04 - Gerenciamento de Acessos e Segurança:**
  - **RF04.01**: O sistema deve permitir o controle de acesso às salas por meio de QR code ou biometria, ativado somente durante o período reservado.
  - **RF04.02**: O sistema deve monitorar em tempo real o uso da sala e desativar automaticamente o acesso após o término da reserva.
  - **RF04.03**: O sistema deve exigir a retenção de um documento de identidade do profissional e do visitante durante a permanência na sala.

- **RF05 - Pagamentos e Faturamento:**
  - **RF05.01**: O sistema deve processar pagamentos online para reservas de salas utilizando métodos de pagamento seguros.
  - **RF05.02**: O sistema deve emitir e enviar faturas digitais para as transações realizadas.
  - **RF05.03**: O sistema deve gerenciar políticas de cancelamento e emitir reembolsos ou créditos conforme as políticas aplicáveis.

- **RF06 - Política de Cancelamento:**
  - **RF06.01**: O sistema deve permitir o cancelamento de reservas dentro do prazo permitido para reembolso.
  - **RF06.02**: O sistema deve calcular e processar reembolsos conforme as políticas de cancelamento definidas por cada locatário.

- **RF07 - Manutenção, Suporte e Limpeza:**
  - **RF07.01**: O sistema deve permitir a solicitação de serviços de manutenção ou limpeza após o uso da sala.
  - **RF07.02**: O sistema deve oferecer a opção de contratar serviços de manutenção e limpeza diretamente por meio da plataforma.
  - **RF07.03**: O sistema deve monitorar a qualidade das salas com inspeções regulares e oferecer suporte técnico para problemas com o sistema de acesso.

- **RF08 - Avaliações e Feedback dos Usuários:**
  - **RF08.01**: O sistema deve solicitar e coletar avaliações das salas e da experiência geral após cada reserva.
  - **RF08.02**: O sistema deve permitir a coleta de feedback a longo prazo em intervalos de 30, 60 e 90 dias.
  - **RF08.03**: O sistema deve utilizar o feedback dos usuários para implementar melhorias contínuas nos serviços oferecidos.

### Requisitos Não Funcionais

- **RNF01 - Segurança:**
  - Proteção de dados dos usuários e transações.
  - Controle de acesso seguro e autenticação.

- **RNF02 - Desempenho:**
  - Resposta rápida nas interações com a plataforma.
  - Processamento eficiente de pagamentos e reservas.

- **RNF03 - Interoperabilidade:**
  - Integração com sistemas de pagamento e serviços de verificação de identidade.

- **RNF04 - Confiabilidade:**
  - Alta disponibilidade e mínima interrupção do serviço.
  - Backup regular dos dados.

- **RNF05 - Usabilidade:**
  - Interface intuitiva e fácil de usar para todos os usuários.
  - Suporte técnico acessível e eficiente.

- **RNF06 - Implementação:**
  - Facilidade na atualização e manutenção da plataforma.
  - Compatibilidade com diferentes dispositivos e navegadores.

## Regras de Negócio

1. **Cadastro de Usuários:**
   - Usuários devem fornecer documentos de identidade válidos e comprovantes de registro profissional (se aplicável).
   - A verificação de documentos deve ser concluída antes da aprovação da conta.

2. **Cadastro de Locações:**
   - Locatários devem fornecer documentação comprovativa de posse ou autorização para alugar os imóveis.
   - A verificação do imóvel deve ser realizada antes de ser listado na plataforma.

3. **Reserva de Salas:**
   - Pagamento antecipado é necessário para confirmar a reserva.
   - A reserva deve ser confirmada por meio de um QR code ou configuração de acesso biométrico.

4. **Acesso e Segurança:**
   - O acesso à sala deve ser restrito ao horário reservado.
   - O acesso deve ser desativado automaticamente após o término da reserva.

5. **Pagamentos e Faturamento:**
   - Todas as transações devem ser processadas de forma segura.
   - Faturas digitais devem ser emitidas e enviadas após o pagamento.

6. **Política de Cancelamento:**
   - Cancelamentos devem ser realizados dentro do prazo permitido para reembolso.
   - O valor do reembolso deve seguir as políticas de cancelamento definidas pelo locatário.

7. **Manutenção e Limpeza:**
   - Solicitações de manutenção ou limpeza devem ser registradas e gerenciadas adequadamente.
   - Inspeções regulares devem ser realizadas para garantir a qualidade dos imóveis.

8. **Avaliações e Feedback:**
   - Feedback deve ser coletado após cada reserva e a cada 30, 60 e 90 dias.
   - A utilização do feedback deve ser feita para melhorar continuamente o serviço.

Protótipos das telas:

![Login](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Login.png)

![Cadastro](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Cadastro.png)

![Validação](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Validar_Documento_Pessoa.png)

![Dashboard](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Dashboard.png)

![Detalhe_Sala](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Detalhe_sala.png)

![Agenda](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Agenda.png)

![Acesso](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Acesso.png)

## **Requisitos de Software por meio de Histórias de Usuários: **

### **Cadastro de Usuário**

- **Como um usuário**, eu quero me cadastrar na plataforma fornecendo minhas informações pessoais e documentos profissionais, para que eu possa reservar salas e utilizar os serviços oferecidos.

### 2. **Login e Acesso**

- **Como um usuário registrado**, eu quero fazer login na plataforma utilizando meu e-mail e senha, para que eu possa acessar minhas reservas e gerenciar minhas informações.


### 3. **Pesquisa e Reserva de Sala**

- **Como um profissional**, eu quero pesquisar e reservar uma sala com base nas minhas necessidades (localização, recursos e disponibilidade), para que eu possa garantir um espaço adequado para o meu trabalho.

### 4. **Pagamento**

- **Como um usuário**, eu quero realizar o pagamento online da reserva de uma sala, para que minha reserva seja confirmada e eu possa utilizar o espaço.

### 5. **Acesso à Sala**

- **Como um usuário com reserva confirmada**, eu quero acessar a sala no horário reservado utilizando QR code ou biometria, para que eu possa usar o espaço de forma segura e eficiente.


### 6. **Gerenciamento de Reservas**

- **Como um usuário**, eu quero visualizar, alterar ou cancelar minhas reservas, para que eu possa gerenciar meu uso das salas de acordo com minhas necessidades.

### 7. **Avaliação da Sala**

- **Como um usuário**, eu quero avaliar a sala após usá-la, para que eu possa compartilhar minha experiência e ajudar outros usuários a fazerem escolhas informadas.

### 8. **Solicitação de Limpeza ou Manutenção**

- **Como um usuário**, eu quero solicitar serviços de manutenção ou limpeza após usar a sala, para que o espaço seja mantido em boas condições para o próximo usuário.

### 9. **Perfil do Usuário**

- **Como um usuário**, eu quero editar minhas informações pessoais e gerenciar minhas notificações, para que meus dados estejam sempre atualizados e eu receba informações relevantes.

### **Portanto em resumo, o sistema deve conter: **
1. **Segurança**:
    - O sistema deve implementar autenticação segura, criptografia de dados e garantir que as transações financeiras sejam realizadas em ambiente seguro.
2. **Usabilidade**:
    - O sistema deve oferecer uma interface de usuário simples e intuitiva, com navegação clara e acessível tanto em desktop quanto em dispositivos móveis.
3. **Desempenho**:
    - O sistema deve garantir tempos de resposta rápidos em todas as operações críticas, como login, reserva e processamento de pagamentos.
4. **Escalabilidade**:
    - O sistema deve ser escalável para suportar um grande número de usuários simultâneos, especialmente em possíveis horários de pico.
