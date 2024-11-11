
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

## Protótipos das telas:
O protótipo das telas pode ser visto completo pelo link https://www.figma.com/design/befodt7Ky1r8lM3r6BqnJK/Untitled?node-id=0-1&t=ENKD2YDepCA64rRP-1
Abaixo, seguem exemplos feitos.

![Login](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Login.png)

![Cadastro](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Cadastro.png)

![Validação](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Validar_Documento_Pessoa.png)

![Dashboard](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Dashboard.png)

![Detalhe_Sala](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Detalhe_sala.png)

![Agenda](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Agenda.png)

![Acesso](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Acesso.png)

![Checkout](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Checkout.png)

![Checkout](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Checkout-1.png)

![Review](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Telas/Review.png)

## **Requisitos de Software por meio de Histórias de Usuários:**

- **Como um usuário**, eu quero me cadastrar na plataforma fornecendo minhas informações pessoais e documentos profissionais, **para que** eu possa reservar salas e utilizar os serviços oferecidos.
    
    **Requisitos**:
    
    - O sistema deve permitir que o usuário insira nome, e-mail, telefone, senha e profissão.
    - O sistema deve permitir o upload de documentos (RG, CRM, OAB, etc.) para verificação.
    - O sistema deve validar os documentos do usuário e notificá-lo sobre a aprovação ou rejeição.
    - O usuário deve ser notificado via e-mail ou SMS para confirmar sua conta.

- **Como um usuário registrado**, eu quero fazer login na plataforma utilizando meu e-mail e senha, **para que** eu possa acessar minhas reservas e gerenciar minhas informações.
    
    **Requisitos**:
    
    - O sistema deve autenticar o usuário com e-mail e senha.
    - O sistema deve permitir a recuperação de senha caso o usuário esqueça.
    - O sistema deve manter o usuário logado durante a sessão ativa e permitir logout seguro.

- **Como um usuário logado**, eu quero pesquisar e reservar uma sala com base nas minhas necessidades (localização, recursos e disponibilidade), **para que** eu possa garantir um espaço adequado para o meu trabalho.
    
    **Requisitos**:
    
    - O sistema deve exibir uma lista de salas com filtros de pesquisa (localização, tipo de sala, preço, recursos, datas disponíveis).
    - O sistema deve permitir que o usuário visualize detalhes da sala, como fotos, descrição, preço e avaliações.
    - O sistema deve permitir que o usuário selecione a data e hora de reserva no calendário.
    - O sistema deve calcular o preço total com base na duração da reserva e gerar um resumo antes da confirmação.
    - O sistema deve processar o pagamento de forma segura e confirmar a reserva.

- **Como um usuário logado**, eu quero realizar o pagamento online da reserva de uma sala, **para que** minha reserva seja confirmada e eu possa utilizar o espaço.
    
    **Requisitos**:
    
    - O sistema deve oferecer opções de pagamento, como cartão de crédito, PayPal, Pix, etc.
    - O sistema deve garantir transações seguras.
    - O sistema deve enviar uma confirmação de pagamento ao usuário e gerar um recibo eletrônico.
    - O sistema deve começar o processamento  do QR code ou da liberação da biometria assim que o pagamento for confirmado.

- **Como um usuário logado e com reserva confirmada**, eu quero acessar a sala no horário reservado utilizando QR code ou biometria, **para que** eu possa usar o espaço de forma segura e eficiente.
    
    **Requisitos**:
    
    - O sistema deve liberar o uso de um QR code ou da configuração do acesso por biometria com antecedência ao período solicitado.
    - O sistema deve permitir o acesso à sala apenas durante o horário reservado.
    - O sistema deve monitorar e registrar os acessos às salas.
    - O sistema deve desativar automaticamente o acesso após o término do período reservado.

- **Como um usuário logado**, eu quero visualizar, alterar ou cancelar minhas reservas, **para que** eu possa gerenciar meu uso das salas de acordo com minhas necessidades.
    
    **Requisitos**:
    
    - O sistema deve exibir uma lista de reservas ativas e passadas.
    - O sistema deve permitir que o usuário visualize detalhes da reserva, como QR code, horário e data.
    - O sistema deve permitir o cancelamento de reservas e calcular o reembolso, de acordo com a política de cancelamento aplicável.
    - O sistema deve notificar o usuário sobre alterações ou cancelamentos.

- **Como um usuário**, eu quero avaliar a sala após usá-la, **para que** eu possa compartilhar minha experiência e ajudar outros usuários a fazerem escolhas informadas.
    
    **Requisitos**:
    
    - O sistema deve permitir que o usuário avalie a sala (de 1 a 5 estrelas) e deixe comentários.
    - O sistema deve enviar uma solicitação de avaliação ao usuário após o uso da sala.
    - O sistema deve armazenar as avaliações e exibi-las na página de cada sala.

- **Como um usuário logado**, eu quero solicitar serviços de manutenção ou limpeza após usar a sala, **para que** o espaço seja mantido em boas condições para o próximo usuário.
    
    **Requisitos**:
    
    - O sistema deve permitir que o usuário registre uma solicitação de limpeza ou manutenção vinculada a uma reserva específica.
    - O sistema deve notificar a equipe de suporte sobre a solicitação.
    - O sistema deve permitir que o usuário acompanhe o status da solicitação.

- **Como um usuário logado**, eu quero editar minhas informações pessoais e gerenciar minhas notificações, **para que** meus dados estejam sempre atualizados e eu receba informações relevantes.
    
    **Requisitos**:
    
    - O sistema deve permitir que o usuário edite seus dados pessoais, como nome, telefone, e-mail e senha.
    - O sistema deve permitir que o usuário configure preferências de notificação (e-mail, SMS, push notifications).
    - O sistema deve permitir que o usuário visualize seu histórico de pagamentos e faturas.

- **Como um usuário locador**, eu quero cadastrar minhas salas na plataforma com todos os detalhes e documentação necessária, **para que** eu possa disponibilizá-las para aluguel e gerenciar as reservas.
    
    **Requisitos**:
    
    - O sistema deve permitir que o locador insira informações detalhadas sobre a sala (nome, tipo, localização, capacidade, descrição).
    - O sistema deve permitir o upload de fotos da sala.
    - O sistema deve permitir o upload de documentos de posse ou autorização de aluguel.
    - O sistema deve verificar e aprovar os documentos do locador antes da sala ser disponibilizada.

- **Como um usuário locador**, eu quero definir a disponibilidade das minhas salas e visualizar as reservas feitas, **para que** eu possa gerenciar os horários em que elas estão livres ou ocupadas.
    
    **Requisitos**:
    
    - O sistema deve permitir que o locador defina a disponibilidade das salas em um calendário.
    - O sistema deve permitir que o locador visualize um painel com todas as reservas, incluindo detalhes como nome do profissional, horário e status de pagamento.
    - O locador deve poder bloquear ou liberar horários específicos para manutenção ou uso pessoal.
    - O sistema deve notificar o locador quando uma nova reserva for feita.

- **Como um usuário locador**, eu quero configurar o preço por hora ou dia para as salas, **para que** eu possa ajustar o valor de acordo com a demanda e os custos de manutenção.
    
    **Requisitos**:
    
    - O sistema deve permitir que o locador defina o preço por hora, dia ou período personalizado para cada sala.
    - O sistema deve permitir a aplicação de tarifas diferenciadas por períodos de maior ou menor demanda.
    - O sistema deve gerar relatórios financeiros com base nas reservas e nas tarifas aplicadas.

- **Como um usuário locador**, eu quero receber o pagamento pelas reservas feitas nas minhas salas de forma segura e transparente, **para que** eu possa acompanhar meus ganhos e despesas.
    
    **Requisitos**:
    
    - O sistema deve processar e transferir automaticamente o pagamento para a conta do locador após a conclusão da reserva.
    - O sistema deve gerar relatórios financeiros detalhados, incluindo os valores recebidos e as taxas aplicadas pela plataforma.
    - O locador deve receber uma notificação sempre que um pagamento for processado.

- **Como um usuário locador**, eu quero receber feedback dos profissionais que utilizaram minhas salas, **para que** eu possa melhorar a experiência e garantir um bom serviço.
    
    **Requisitos**:
    
    - O sistema deve permitir que o locador visualize as avaliações e comentários dos usuários após cada reserva.
    - O sistema deve enviar um resumo mensal de feedbacks para que o locador possa acompanhar a satisfação dos profissionais.
    - O locador deve poder responder aos comentários ou contestar avaliações, se necessário.

### **Manutenção e Limpeza das Salas**

- **Como um usuário locador**, eu quero gerenciar as solicitações de manutenção ou limpeza feitas pelos profissionais que utilizam minhas salas, **para que** eu possa garantir que elas estejam sempre em boas condições.
    
    **Requisitos**:
    
    - O sistema deve permitir que o locador visualize e acompanhe as solicitações de manutenção ou limpeza relacionadas às suas salas.
    - O locador deve poder marcar horários para manutenção e bloquear a disponibilidade da sala durante esse período.
    - O sistema deve notificar o locador sobre problemas recorrentes ou críticos que possam afetar a qualidade do espaço.

### **Os Requisitos não Funcionais presentes são:**
**Segurança**:
    - O sistema deve implementar autenticação segura, criptografia de dados e garantir que as transações financeiras sejam realizadas em ambiente seguro.

**Usabilidade**:
    - O sistema deve oferecer uma interface de usuário simples e intuitiva, com navegação clara e acessível tanto em desktop quanto em dispositivos móveis.

**Desempenho**:
    - O sistema deve garantir tempos de resposta rápidos em todas as operações críticas, como login, reserva e processamento de pagamentos.

**Escalabilidade**:
    - O sistema deve ser escalável para suportar um grande número de usuários simultâneos, especialmente em possíveis horários de pico.

**Controle de Disponibilidade**:
    - O sistema deve garantir que as salas não sejam reservadas para mais de um usuário ao mesmo tempo, e o locador possa ajustar a disponibilidade em tempo real.

**Relatórios Financeiros**:
    - O sistema deve fornecer ao locador um painel financeiro que exibe ganhos por período, taxas aplicadas e histórico de transações.

**Suporte a Ajustes de Preços**:
    - O sistema deve permitir ajustes dinâmicos de preços, inclusive descontos promocionais e valores personalizados por horários.

## Diagrama de Caso de Uso:

![Casos de Uso](https://github.com/nullifidianz/engenharia-de-software/blob/main/imgs/Diagramas/Diagrama-Casos-de-Uso.png)

## Diagrama de Domínio:
[![](https://mermaid.ink/img/pako:eNqtV9tu2zAM_RVDTxvaFLk2q9-KdgUKrEW37gJs2QMjMYkQWwwkuWhX9JP2Ffux0UmciyO76boAAWTxiJQOeSj7UUhSKGLRaDQGdmC89gnG0bmGsYUUIoXROaV_fhtN0Tey02u8z1wOXOLzv0zAueWK_Dni33wu-uIysLzysZjOfw2t4kgbvzVnKOWwzlttxlsGTEEnQYtDM4GgxWOCIzJhh17PKGhQJLMUjaevkJCth3zex4lWjBkSJQhme-cefOaCtgMJCtgv2Ddvt-YTGmtTmmMvHOUX2HNQ5EpGiwpH2mh7m_NUMjpKtNQe7BWYzKORQGXfd-wa7C0kG2ufipSvU_yBJPDqPVKcLYohLqpimxKOE0d5tG06wcOl4a3yMh7jjvFCpwHL3SKDo4TAB5kPZI51oMd0KtG5cGpp6NDegSQMOmDC5_Zy4iQYicnO9Bg5xx8_nbH6SpaZpfkmziYop5T5Wvpzxl4jL4VOWs0JfJlWJMxAagUKd2MlXBF5VVY5tSgz62hF4o-fW-YZ2ymUO6XdjIwe6mQZONQTqvO7UmZV4DVgod2wQBs6hTGaCieV8l1LdfsUJdhSsjc5B7V5v4ExzDe7R_KThUTjQqv7SSVFT4pWcV5MN4vzZlHJhYMdmTJPxuU7ulRBRS2VsEMmOk_WbE4HGLpAVEOQ09cSVNu2DHnY9ScpP_FiVQU1781dsKdxE5mR88F77QB50Q4Z8xVGYT0b1-T1SP-XVl3ZFPjQjrWRVh46cN5cBWGdcd-EZC8aAsddX2uvTX9xUxqPL6TjGXFUXGinvG2lqxTz3B20utd32g_WlEjxmjYQrYGIGg0eXPOgREcFqtDZM7CNAiyQxavDBjIfbL4EVEBWXakGlwddl0EBnN-X9edct9ZS1BJu1WD-DVaqpU2B1iM3ars-cjVw6VEcihQtv2Ar_gB4zBcNhJ9gigMR81CBnQ7EwDwxDjJPtw9GitjbDA-FpWw8EfEIEsdP2Syv1OUnQAGZgflOtPko4kdxL-LWceeo0-21TnrNTqfZf9fvH4oHETc6J0fN_nG73er3Trr9Vr_7dCh-zT20jjrHzVa33eTpbq_Ta_MKVJpvgavF18v8I-bpLwsY4ok?type=png)](https://mermaid.live/edit#pako:eNqtV9tu2zAM_RVDTxvaFLk2q9-KdgUKrEW37gJs2QMjMYkQWwwkuWhX9JP2Ffux0UmciyO76boAAWTxiJQOeSj7UUhSKGLRaDQGdmC89gnG0bmGsYUUIoXROaV_fhtN0Tey02u8z1wOXOLzv0zAueWK_Dni33wu-uIysLzysZjOfw2t4kgbvzVnKOWwzlttxlsGTEEnQYtDM4GgxWOCIzJhh17PKGhQJLMUjaevkJCth3zex4lWjBkSJQhme-cefOaCtgMJCtgv2Ddvt-YTGmtTmmMvHOUX2HNQ5EpGiwpH2mh7m_NUMjpKtNQe7BWYzKORQGXfd-wa7C0kG2ufipSvU_yBJPDqPVKcLYohLqpimxKOE0d5tG06wcOl4a3yMh7jjvFCpwHL3SKDo4TAB5kPZI51oMd0KtG5cGpp6NDegSQMOmDC5_Zy4iQYicnO9Bg5xx8_nbH6SpaZpfkmziYop5T5Wvpzxl4jL4VOWs0JfJlWJMxAagUKd2MlXBF5VVY5tSgz62hF4o-fW-YZ2ymUO6XdjIwe6mQZONQTqvO7UmZV4DVgod2wQBs6hTGaCieV8l1LdfsUJdhSsjc5B7V5v4ExzDe7R_KThUTjQqv7SSVFT4pWcV5MN4vzZlHJhYMdmTJPxuU7ulRBRS2VsEMmOk_WbE4HGLpAVEOQ09cSVNu2DHnY9ScpP_FiVQU1781dsKdxE5mR88F77QB50Q4Z8xVGYT0b1-T1SP-XVl3ZFPjQjrWRVh46cN5cBWGdcd-EZC8aAsddX2uvTX9xUxqPL6TjGXFUXGinvG2lqxTz3B20utd32g_WlEjxmjYQrYGIGg0eXPOgREcFqtDZM7CNAiyQxavDBjIfbL4EVEBWXakGlwddl0EBnN-X9edct9ZS1BJu1WD-DVaqpU2B1iM3ars-cjVw6VEcihQtv2Ar_gB4zBcNhJ9gigMR81CBnQ7EwDwxDjJPtw9GitjbDA-FpWw8EfEIEsdP2Syv1OUnQAGZgflOtPko4kdxL-LWceeo0-21TnrNTqfZf9fvH4oHETc6J0fN_nG73er3Trr9Vr_7dCh-zT20jjrHzVa33eTpbq_Ta_MKVJpvgavF18v8I-bpLwsY4ok)

## Descrição das Classes de Domínio:

| Classe | Descrição |
|--------|-----------|
| Usuario | Esta classe armazena as informações respectivas ao cadastro e autenticação dos usuários da plataforma, incluindo seus dados pessoais, documentos e credenciais de acesso, permitindo a interação com as funcionalidades de locação, avaliação e manutenção do sistema. |
| Sala | Esta classe armazena as informações respectivas aos espaços disponíveis para locação, contemplando suas características físicas, recursos oferecidos, precificação e disponibilidade, possibilitando o gerenciamento completo dos ambientes ofertados. |
| Locacao | Esta classe armazena as informações respectivas às reservas realizadas, estabelecendo a relação entre usuários e salas, com controle de períodos, valores, status e códigos de acesso, centralizando todo o processo de aluguel. |
| Pagamento | Esta classe armazena as informações respectivas às transações financeiras das locações, controlando valores, métodos de pagamento, status de processamento e registros das operações realizadas. |
| Feedback | Esta classe armazena as informações respectivas às avaliações feitas pelos usuários sobre as locações realizadas, incluindo notas, comentários e possíveis respostas, permitindo o monitoramento da satisfação. |
| Notificacao | Esta classe armazena as informações respectivas às comunicações enviadas aos usuários, gerenciando tipos de mensagens, status de leitura e canais de envio para manter os usuários informados. |
| Manutencao | Esta classe armazena as informações respectivas às solicitações de manutenção das salas, controlando tipos de problemas, status de atendimento e acompanhamento das resoluções necessárias. |

## Projeto de Arquitetura:

### Casos de Uso (interações do usuário):

Cadastro e Autenticação de Usuários
Gerenciamento de Salas (Cadastro, Disponibilidade, Precificação)
Reserva de Salas (Pesquisa, Seleção, Pagamento)
Acesso às Salas (QR Code, Biometria)
Gerenciamento de Reservas (Visualização, Alteração, Cancelamento)
Avaliação de Salas
Solicitação de Manutenção e Limpeza
Configuração de Perfil e Notificações
Relatórios Financeiros e de Desempenho (Locatários)


### Protótipos (telas do sistema):

- Tela de Login/Cadastro
- Tela de Busca e Seleção de Salas
- Tela de Detalhes da Sala
- Tela de Reserva e Checkout
- Tela de Acesso à Sala (QR Code/Biometria)
- Tela de Gerenciamento de Reservas
- Tela de Avaliação da Sala
- Tela de Solicitação de Manutenção
- Tela de Configurações de Perfil
- Painel de Controle (Locatários)


### Modelo de Domínio (classes do sistema):

- Usuário
- Sala
- Locação
- Pagamento
- Feedback
- Notificação
- Manutenção
- Documento



### Arquitetura do Sistema:
A arquitetura do sistema será baseada em uma abordagem de microsserviços, onde cada uma das principais funcionalidades será implementada como um serviço independente. Isso permitirá maior escalabilidade, flexibilidade e autonomia no desenvolvimento e manutenção do sistema.
Os principais serviços serão:

### Serviço de Autenticação e Perfil do Usuário:

Responsável pelo cadastro, autenticação e gerenciamento de perfil dos usuários.
Integrará com serviços de verificação de documentos.


### Serviço de Gerenciamento de Salas:

Responsável pelo cadastro, atualização e controle das informações das salas.
Incluirá a gestão de disponibilidade, precificação e documentação.


### Serviço de Reservas:

Responsável pela criação, modificação e cancelamento de reservas.
Integrará com o serviço de pagamentos e liberação de acesso.


### Serviço de Pagamentos:

Responsável pelo processamento seguro de transações financeiras.
Integrará com provedores de pagamento externos.


### Serviço de Feedbacks e Avaliações:

Responsável pela coleta, armazenamento e exibição de feedbacks dos usuários.
Permitirá a resposta dos locatários aos comentários.


### Serviço de Notificações:

Responsável pelo envio de notificações aos usuários (e-mail, SMS, push).
Integrará com serviços de comunicação externos.


### Serviço de Manutenção:

Responsável pelo registro e acompanhamento de solicitações de manutenção.
Permitirá a programação de intervenções nos imóveis.


### Serviço de Relatórios e Business Intelligence:

Responsável pela geração de relatórios financeiros e de desempenho.
Integrará dados dos demais serviços para análises estratégicas.



### De maneira detalhada, utilizaremos:

1. **Linguagem e Frameworks**:
   - Utilizaremos Java como linguagem de programação para a construção dos microsserviços.
    - Como framework principal, adotaremos o Spring Boot, que fornece recursos robustos para desenvolvimento de aplicações baseadas em microsserviços.
   - Para o front-end, adotaremos o React.js com o framework Next.js, que fornece recursos de renderização do lado do servidor (SSR) e otimização para SEO.

2. **Containers e Orquestração**:
   - Os microsserviços serão empacotados em contêineres Docker para garantir a portabilidade e a consistência do ambiente de execução.
   - A orquestração dos contêineres será realizada pelo Kubernetes, que oferece recursos avançados de escalabilidade, balanceamento de carga e gerenciamento de ciclo de vida.

3. **Banco de Dados**:
   - Utilizaremos o MongoDB como banco de dados NoSQL para armazenar os dados semi-estruturados do sistema, como informações de usuários, salas, reservas e feedbacks.
   - Para os dados financeiros e transações, adotaremos o PostgreSQL como banco de dados relacional, oferecendo integridade e consistência dos dados.

4. **Mensageria e Integração**:
   - O barramento de mensagens será implementado usando o Apache Kafka, que fornece alta escalabilidade, tolerância a falhas e processamento de eventos em tempo real.
   - Essa abordagem permitirá a comunicação assíncrona entre os microsserviços, facilitando a integração e o desacoplamento.

5. **API Gateway**:
   - Implementaremos um API Gateway usando o NGINX, que atuará como ponto de entrada único para todas as requisições do sistema.
   - O API Gateway será responsável por roteamento, balanceamento de carga, autenticação e autorização das chamadas entre os microsserviços e o front-end.

6. **Segurança**:
   - Utilizaremos o Keycloak como provedor de identidade, responsável pela autenticação e autorização dos usuários.
   - O Keycloak integrará com os microsserviços por meio de tokens JWT, garantindo a segurança das comunicações.

7. **Monitoramento e Observabilidade**:
   - Implementaremos um conjunto de ferramentas de monitoramento, incluindo Prometheus para métricas, Grafana para painéis de monitoramento e Elasticsearch/Kibana para logs.
   - Essa stack de observabilidade nos permitirá acompanhar o desempenho, a saúde e a integridade dos microsserviços em tempo real.

8. **Implantação e CI/CD**:
   - Adotaremos uma abordagem de Entrega Contínua (CI/CD) usando ferramentas como GitLab CI/CD ou GitHub Actions.
   - Isso nos permitirá automatizar o processo de build, teste e implantação dos microsserviços, garantindo a entrega rápida e segura de novas funcionalidades.

9. **Infraestrutura em Nuvem**:
   - Hospedamos toda a infraestrutura do sistema na nuvem da AWS, aproveitando os serviços gerenciados, como EC2 para execução dos contêineres, Amazon EKS para orquestração do Kubernetes, Amazon RDS para os bancos de dados, Amazon MSK para o Apache Kafka, entre outros.
   - Essa estratégia nos permite escalar rapidamente, reduzir a sobrecarga de gerenciamento de infraestrutura e aproveitar os recursos de alta disponibilidade e resiliência oferecidos pela AWS.


