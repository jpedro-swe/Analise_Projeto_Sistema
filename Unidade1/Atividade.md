20/08
Introdução à Análise e Projeto de Sistemas de Informação
Conceitos e elementos fundamentais da engenharia de software - definição, características e tipos de
modelagens. Ferramentas Case de apoio ao desenho dos diagramas UML.
# Ficha de Requisitos — Aula 02

## Análise e Projeto de Sistemas

**Unidade:** II — Introdução à Análise e Projeto de Sistemas  
**Atividade:** Transformação do levantamento do sistema em requisitos funcionais e não funcionais  
**Objetivo:** Registrar, de forma estruturada, o que o sistema deve fazer e quais características de qualidade deve atender.

---

## 1. Identificação do Sistema

| Campo | Preenchimento |
|---|---|
| Nome do sistema | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo | Conectar pessoas que desejam adotar plantas com doadores, facilitando a adoção responsável através de um matching de perfil, gestão de anúncios de plantas e comunicação entre usuários. |
| Público-alvo | Entusiastas de plantas, jardineiros, doadores de plantas e interessados em adoção sustentável. |
| Responsável pelo levantamento |[João Pedro Alves De Sousa](https://github.com/jpedro-swe)[Hélter Brandão De Oliveira](https://github.com/brandao395)[Davi Gonçalves Castro](https://github.com/MF-DAVI)[Jorge Luis Soares do Santos](https://github.com/7deo)|
| Versão | 1.0 |

---

# 2. Requisitos Funcionais

> Requisitos funcionais descrevem **funcionalidades ou serviços que o sistema deve oferecer**.

## RF01 — Cadastrar usuário

| Campo | Descrição |
|---|---|
| **Identificação** | RF01 |
| **Descrição** | O sistema deve permitir que novos usuários se cadastrem na plataforma informando seus dados pessoais e preferências de plantas. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir informar nome, e-mail, telefone, senha e localização geográfica. 2. Deve impedir o cadastro sem nome, e-mail e telefone. 3. Deve validar formato de e-mail. 4. Deve informar ao usuário quando o cadastro for concluído com sucesso. |
| **Exemplo** | O usuário preenche seus dados e preferências de plantas na tela de cadastro e clica em Salvar. O sistema valida as informações e registra a nova conta. |

## RF02 — Anunciar planta para adoção

| Campo | Descrição |
|---|---|
| **Identificação** | RF02 |
| **Descrição** | O sistema deve permitir que usuários anunciem plantas disponíveis para adoção com detalhes sobre a espécie e cuidados necessários. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir informar nome da planta, espécie, tamanho, condições de saúde e requisitos de cuidado. 2. Deve impedir o cadastro sem nome e espécie. 3. Deve permitir upload de fotos. 4. Deve apresentar confirmação após o anúncio ser criado. |
| **Exemplo** | Um doador cadastra uma planta Suculenta, especifica que está em bom estado e requer pouca água. O sistema registra o anúncio com as fotos fornecidas. |

## RF03 — Buscar e filtrar plantas

| Campo | Descrição |
|---|---|
| **Identificação** | RF03 |
| **Descrição** | O sistema deve permitir que usuários busquem plantas disponíveis para adoção usando filtros como espécie, tamanho e localização. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir pesquisar por nome, espécie ou características. 2. Deve filtrar por localização geográfica do doador. 3. Deve mostrar distância entre usuário e doador. 4. Deve listar resultados com foto, nome e disponibilidade. |
| **Exemplo** | O usuário busca por "Suculenta" e filtra por plantas em sua região. O sistema exibe 12 resultados com fotos e informações dos doadores. |

## RF04 — Enviar pedido de adoção

| Campo | Descrição |
|---|---|
| **Identificação** | RF04 |
| **Descrição** | O sistema deve permitir que interessados em adotar enviem pedidos formais ao doador da planta. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve registrar o pedido de adoção com data e hora. 2. Deve notificar o doador sobre novo pedido. 3. Deve permitir que o doador aceite ou rejeite o pedido. 4. Deve manter histórico de pedidos. |
| **Exemplo** | Um usuário interessado clica em "Solicitar Adoção" para uma planta. O doador recebe a notificação e pode aceitar ou recusar o pedido. |

## RF05 — Comunicação entre usuários

| Campo | Descrição |
|---|---|
| **Identificação** | RF05 |
| **Descrição** | O sistema deve permitir troca de mensagens entre doador e adotante para discussão dos detalhes da entrega. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Deve permitir envio e recebimento de mensagens em tempo real ou próximo. 2. Deve manter histórico de conversas. 3. Deve notificar sobre novas mensagens. 4. Deve impedir mensagens ofensivas ou spam. |
| **Exemplo** | Após aceitar o pedido, doador e adotante conversam sobre horário e local de entrega da planta. |

## RF06 — Avaliar e comentar

| Campo | Descrição |
|---|---|
| **Identificação** | RF06 |
| **Descrição** | O sistema deve permitir que usuários avaliem doadores e adotantes após a conclusão da adoção. |
| **Prioridade** | Média |
| **Critérios de aceitação** | 1. Deve permitir atribuir nota de 1 a 5 estrelas. 2. Deve permitir escrever comentário sobre a experiência. 3. Deve exibir histórico de avaliações no perfil do usuário. 4. Deve calcular média de avaliações. |
| **Exemplo** | Após receber a planta, o adotante avalia o doador com 5 estrelas e comenta sobre a qualidade da planta e prestatividade. |

## RF07 — Gerenciar perfil

| Campo | Descrição |
|---|---|
| **Identificação** | RF07 |
| **Descrição** | O sistema deve permitir que usuários atualizem seus dados pessoais, preferências e foto de perfil. |
| **Prioridade** | Média |
| **Critérios de aceitação** | 1. Deve permitir editar nome, e-mail, telefone e localização. 2. Deve permitir alterar foto de perfil. 3. Deve permitir atualizar preferências de plantas. 4. Deve manter histórico de alterações. |
| **Exemplo** | Um usuário atualiza sua foto de perfil e adiciona novas preferências de plantas para receber recomendações personalizadas. |

---

# 3. Requisitos Não Funcionais

> Requisitos não funcionais descrevem **características, restrições e condições de qualidade** que o sistema deve atender.

## RNF01 — Segurança

| Campo | Descrição |
|---|---|
| **Identificação** | RNF01 |
| **Descrição** | O sistema deve controlar o acesso às funcionalidades conforme o perfil do usuário e proteger dados pessoais. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Usuários devem autenticar-se antes de acessar funções sensíveis. 2. Senhas devem ser armazenadas de forma criptografada. 3. Dados pessoais devem estar protegidos conforme LGPD. 4. Apenas doadores podem anunciar plantas. |
| **Exemplo** | Um usuário não autenticado não consegue enviar pedidos de adoção. Dados pessoais são acessíveis apenas ao proprietário do perfil. |

## RNF02 — Usabilidade

| Campo | Descrição |
|---|---|
| **Identificação** | RNF02 |
| **Descrição** | A interface deve apresentar informações e comandos de forma clara, intuitiva e consistente. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Os campos devem possuir rótulos claros e descrições de ajuda. 2. Mensagens de erro devem orientar o usuário sobre o problema. 3. As ações principais devem ser facilmente identificáveis com ícones e cores. 4. Interface responsiva para dispositivos móveis. |
| **Exemplo** | Ao deixar o campo de espécie vazio, o sistema informa "Campo obrigatório: digite o nome ou espécie da planta". Botão de "Solicitar Adoção" está em destaque. |

## RNF03 — Desempenho

| Campo | Descrição |
|---|---|
| **Identificação** | RNF03 |
| **Descrição** | Buscas e consultas devem apresentar resposta em tempo adequado para proporcionar boa experiência do usuário. |
| **Prioridade** | Média |
| **Critérios de aceitação** | 1. Buscas de plantas devem retornar resultados em até 2 segundos. 2. Carregamento de fotos não deve ultrapassar 3 segundos. 3. Mensagens devem ser entregues em tempo real (até 1 segundo). |
| **Exemplo** | Ao pesquisar por "Cacto", o sistema exibe resultados em até 2 segundos. Ao enviar mensagem ao doador, é entregue imediatamente. |

## RNF04 — Disponibilidade

| Campo | Descrição |
|---|---|
| **Identificação** | RNF04 |
| **Descrição** | O sistema deve estar disponível 24/7 para consulta de plantas e interação entre usuários. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. O sistema deve ter disponibilidade mínima de 99% do tempo. 2. Manutenções devem ser agendadas em horários de baixo uso. 3. Deve haver backup automático dos dados. |
| **Exemplo** | Um usuário consegue acessar a plataforma a qualquer hora do dia para buscar plantas e enviar mensagens. |

## RNF05 — Integridade dos dados

| Campo | Descrição |
|---|---|
| **Identificação** | RNF05 |
| **Descrição** | O sistema deve preservar a consistência e confiabilidade dos dados registrados. |
| **Prioridade** | Alta |
| **Critérios de aceitação** | 1. Não deve permitir anúncio de planta sem informações essenciais. 2. Pedidos de adoção devem estar sempre associados a um usuário e uma planta válidos. 3. Não deve permitir excluir planta enquanto há pedidos pendentes. 4. Avaliações devem ser registradas apenas uma vez por adoção. |
| **Exemplo** | Ao tentar anunciar uma planta sem espécie, o sistema bloqueia a operação e solicita que o campo seja preenchido. Uma planta não pode ser deletada se existem pedidos pendentes. |

## RNF06 — Escalabilidade

| Campo | Descrição |
|---|---|
| **Identificação** | RNF06 |
| **Descrição** | O sistema deve suportar crescimento no número de usuários, plantas anunciadas e transações sem degradação de desempenho. |
| **Prioridade** | Média |
| **Critérios de aceitação** | 1. Deve suportar no mínimo 10.000 usuários simultâneos. 2. Infraestrutura deve permitir expansão horizontal. 3. Banco de dados deve ser otimizado para consultas em larga escala. |
| **Exemplo** | Mesmo com 5.000 usuários ativos buscando plantas simultaneamente, o sistema mantém tempo de resposta adequado. |

---

# 4. Modelo para preenchimento pelos estudantes

## Requisito Funcional

| Campo | Resposta do grupo |
|---|---|
| Identificação | RF__ |
| Descrição | |
| Prioridade | Alta / Média / Baixa |
| Critérios de aceitação | |
| Exemplo | |

## Requisito Não Funcional

| Campo | Resposta do grupo |
|---|---|
| Identificação | RNF__ |
| Descrição | |
| Prioridade | Alta / Média / Baixa |
| Critérios de aceitação | |
| Exemplo | |

---

# 5. Orientações para elaboração

Para cada requisito, o grupo deve verificar:

- **Identificação:** possui código único?
- **Descrição:** está claro o que o sistema deve fazer ou qual característica deve apresentar?
- **Prioridade:** é essencial, importante ou pode ser implementado posteriormente?
- **Critérios de aceitação:** é possível verificar objetivamente se o requisito foi atendido?
- **Exemplo:** existe uma situação concreta que demonstra o requisito?

## Regra prática

Um bom requisito deve ser:

**Claro + específico + verificável + relevante**

---

# 6. Entregável da atividade

O grupo deverá entregar:

1. Identificação do sistema;
2. Pelo menos **5 requisitos funcionais**;
3. Pelo menos **3 requisitos não funcionais**;
4. Prioridade de cada requisito;
5. Critérios de aceitação;
6. Exemplo de utilização;
7. Identificação dos integrantes do grupo.

**Próxima etapa:** os requisitos produzidos nesta ficha servirão de base para a identificação e especificação dos **casos de uso**.
