Link do Template: https://miro.com/app/board/uXjVHo3jFqo=/

# 📋 Projeto de APS PlantTinder

## Levantamento e Priorização de Requisitos

**Etapa:** Levantamento de Requisitos (Utilizar a ficha dos requisitos levantados) 
**Técnica de Priorização:** MoSCoW  
**Data:** 10/09/2026
**Turma:** D2 - Engenharia de Software  

---

# 👥 1. Identificação do Grupo

| Integrante | Nome |
|---|---|
| 1 | [João Pedro Alves De Sousa](https:github/jpedro-swe)|
| 2 |[Hélter Brandão De Oliveira](https:github/brandao395)|
| 3 | [Davi Gonçalves Castro](https:github/MF-DAVI)|
| 4 | [Jorge Luis Soares do Santos](https://github.com/7deo)|

---

# 2. Identificação do Projeto

**Nome do projeto:**  
> Rede de Apoio para Adoção de Plantas (PlantTinder)

**Descrição resumida do projeto:**  
> O projeto consiste no desenvolvimento de uma plataforma digital focada em conectar pessoas interessadas em adotar plantas com doadores[cite: 4]. O objetivo principal é facilitar a adoção responsável por meio do matching de perfis, gerenciamento de anúncios e comunicação direta entre os usuários[cite: 4].

---

# 3. Problema Identificado

## 3.1 Qual problema será resolvido?

> Descreva o problema identificado pelo grupo.  
> Neste momento, concentre-se no problema e não na tecnologia que será utilizada.

**Resposta:**

> A dificuldade de encontrar destinos adequados para plantas que não podem mais ser cuidadas pelos seus atuais donos, bem como a dificuldade de entusiastas de plantas encontrarem espécies específicas para adoção de forma confiável e centralizada.

---

## 3.2 Quem é afetado pelo problema?

> Identifique os principais usuários, grupos ou organizações afetados.

**Resposta:**

> Entusiastas de plantas, jardineiros, pessoas que precisam doar suas plantas por falta de espaço ou tempo, e interessados em práticas de adoção sustentável[cite: 4].

---

## 3.3 Como o problema é resolvido atualmente?

> Explique como as pessoas realizam atualmente o processo ou atividade relacionada ao problema.

**Resposta:**

> Atualmente, as pessoas dependem de redes sociais genéricas, grupos de vizinhança ou doações boca a boca, o que dificulta o encontro entre doadores e pessoas com o perfil adequado para cuidar da planta específica, além de carecer de histórico ou garantias de cuidado.

---

## 3.4 Principais dificuldades encontradas

Liste pelo menos três dificuldades observadas.

1. Falta de uma plataforma centralizada e confiável para doação de plantas.
2. Dificuldade em encontrar pessoas com o conhecimento adequado para cuidar de espécies específicas.
3. Comunicação fragmentada e desorganizada entre doadores e adotantes.

---

# 🎯 4. Objetivo do Projeto

Descreva o resultado que o projeto pretende alcançar.

Utilize como referência:

> **Nosso projeto pretende [resultado] para [stakeholder], contribuindo para [benefício].**

**Objetivo:**

> Nosso projeto pretende criar uma plataforma centralizada e segura para doadores e adotantes de plantas, contribuindo para a adoção responsável e sustentável, facilitando o encontro de perfis compatíveis com as necessidades de cada espécie.

---

# 👤 5. Stakeholders

Identifique as pessoas, grupos ou organizações que possuem interesse ou participação no sistema.

| ID | Stakeholder | Papel | Necessidade/Interesse | Influência |
|---|---|---|---|---|
| ST01 | Doadores de Plantas | Usuário | Encontrar lares adequados para suas plantas de forma fácil e segura. | Alta |
| ST02 | Adotantes de Plantas | Usuário | Encontrar plantas disponíveis para adoção que se adequem ao seu perfil e localização. | Alta |
| ST03 | Administradores do Sistema | Manutenção/Suporte | Garantir o funcionamento, segurança e integridade da plataforma. | Média |

---

## Stakeholder principal

**Stakeholder:**

> Doadores e Adotantes de Plantas (Usuários Finais)

**Por que ele foi considerado o principal stakeholder?**

> Porque o sucesso e a utilidade da plataforma dependem inteiramente do engajamento e da interação entre esses dois grupos. Sem eles, o sistema não tem propósito.

---

# 🗣️ 6. Levantamento de Informações

Registre as principais informações obtidas durante o levantamento.

| Pergunta | Resposta |
|---|---|
| O que o usuário precisa fazer? | Cadastrar-se, anunciar plantas, buscar plantas, comunicar-se e avaliar a experiência[cite: 4]. |
| Qual problema enfrenta atualmente? | Dificuldade em encontrar e doar plantas de forma estruturada e confiável. |
| Quais informações precisa consultar? | Espécies disponíveis, detalhes e cuidados da planta, localização do doador e avaliações[cite: 4]. |
| Quais informações precisa cadastrar ou alterar? | Dados pessoais, preferências de plantas, fotos e detalhes dos anúncios de doação[cite: 4]. |
| Quais tarefas são repetitivas? | Responder a perguntas básicas sobre a planta anunciada (mitigado pelo preenchimento de detalhes no anúncio). |
| Quais tarefas consomem mais tempo? | Filtrar e encontrar a planta ideal ou o adotante ideal. |
| Quais erros acontecem atualmente? | Doações para pessoas sem perfil para cuidar da espécie, falta de informações sobre os cuidados necessários. |
| Precisa receber notificações? | Sim, para novos pedidos de adoção e novas mensagens recebidas[cite: 4]. |
| Precisa gerar documentos ou relatórios? | Não, o sistema é focado em matchmaking e comunicação. |
| Existem informações que precisam ser protegidas? | Sim, dados pessoais dos usuários, como e-mail, telefone e localização exata (proteção LGPD)[cite: 4]. |
| O sistema precisará se comunicar com outros sistemas? | Pode necessitar comunicação com APIs de mapas/geolocalização. |
| Existem regras obrigatórias que precisam ser respeitadas? | Lei Geral de Proteção de Dados (LGPD)[cite: 4]. |

---

# 💡 7. Necessidades Identificadas

Antes de escrever os requisitos, registre as necessidades identificadas durante o levantamento.

| ID | Stakeholder | Necessidade Identificada | Problema Relacionado |
|---|---|---|---|
| N01 | Todos os usuários | Criar uma conta para acessar a plataforma. | Falta de ambiente seguro e rastreável. |
| N02 | Doador | Publicar informações detalhadas sobre a planta disponível. | Falta de clareza sobre os cuidados que a planta exige. |
| N03 | Adotante | Pesquisar plantas por características específicas (ex: tamanho, espécie, local). | Dificuldade em encontrar plantas adequadas ao seu perfil e região. |
| N04 | Adotante | Demonstrar interesse formal em uma planta. | Falta de um processo claro de adoção. |
| N05 | Todos os usuários | Trocar mensagens para combinar a entrega. | Comunicação desorganizada em redes sociais diversas. |
| N06 | Todos os usuários | Segurança dos dados pessoais informados. | Exposição indevida de dados na internet. |

---

# ⚙️ 8. Requisitos Funcionais

Os requisitos funcionais representam as funcionalidades e os comportamentos esperados do sistema.

Utilize preferencialmente a estrutura:

> **O sistema deve...**

## Requisitos Funcionais do Projeto

| ID | Requisito Funcional | Stakeholder/Fonte | Necessidade | Prioridade |
|---|---|---|---|---|
| RF01 | O sistema deve permitir que novos usuários se cadastrem na plataforma informando seus dados pessoais e preferências de plantas[cite: 4]. | Todos os usuários | N01 | Alta |
| RF02 | O sistema deve permitir que usuários anunciem plantas disponíveis para adoção com detalhes sobre a espécie e cuidados necessários[cite: 4]. | Doadores | N02 | Alta |
| RF03 | O sistema deve permitir que usuários busquem plantas disponíveis para adoção usando filtros como espécie, tamanho e localização[cite: 4]. | Adotantes | N03 | Alta |
| RF04 | O sistema deve permitir que interessados em adotar enviem pedidos formais ao doador da planta[cite: 4]. | Adotantes | N04 | Alta |
| RF05 | O sistema deve permitir troca de mensagens entre doador e adotante para discussão dos detalhes da entrega[cite: 4]. | Todos os usuários | N05 | Alta |
| RF06 | O sistema deve permitir que usuários avaliem doadores e adotantes após a conclusão da adoção[cite: 4]. | Todos os usuários | - | Média |
| RF07 | O sistema deve permitir que usuários atualizem seus dados pessoais, preferências e foto de perfil[cite: 4]. | Todos os usuários | - | Média |

---

# ⭐ 9. Requisitos de Qualidade

Os requisitos de qualidade devem ser escritos de forma clara e, sempre que possível, **mensurável e verificável**.

## Requisitos de Qualidade do Projeto

| ID | Característica de Qualidade | Requisito | Como será verificado? |
|---|---|---|---|
| RQ01 | Segurança | O sistema deve controlar o acesso às funcionalidades conforme o perfil do usuário e proteger dados pessoais conforme LGPD. Senhas criptografadas[cite: 4]. | Testes de penetração, verificação de criptografia no banco e auditoria de acesso a dados. |
| RQ02 | Usabilidade | A interface deve apresentar informações claras, ser intuitiva e responsiva para dispositivos móveis[cite: 4]. Mensagens de erro claras[cite: 4]. | Testes de usabilidade com usuários e validação de responsividade em diferentes telas. |
| RQ03 | Desempenho | Buscas de plantas devem retornar resultados em até 2 segundos e carregamento de fotos em até 3 segundos[cite: 4]. | Testes de carga e monitoramento de tempo de resposta do servidor. |
| RQ04 | Disponibilidade | O sistema deve ter disponibilidade mínima de 99% do tempo, operando 24/7[cite: 4]. | Monitoramento contínuo de uptime do servidor. |
| RQ05 | Integridade | O sistema deve preservar a consistência, impedindo anúncio sem dados essenciais e exclusão de plantas com pedidos pendentes[cite: 4]. | Testes unitários e de integração validando as regras de banco de dados e backend. |
| RQ06 | Escalabilidade | O sistema deve suportar no mínimo 10.000 usuários simultâneos sem degradação de desempenho[cite: 4]. | Testes de stress simulando múltiplos acessos simultâneos. |

---

# 🚧 10. Restrições

Registre as limitações identificadas no projeto.

| ID | Restrição | Categoria | Justificativa/Fonte |
|---|---|---|---|
| RES01 | Adequação à LGPD | Legislação | Obrigatório para tratamento de dados pessoais no Brasil. |
| RES02 | Escopo exclusivamente gratuito | Negócio | A plataforma não suportará vendas ou transações financeiras, focando apenas em doação/adoção. |
| RES03 | Prazos acadêmicos | Prazo | O projeto deve ser concluído dentro do cronograma da disciplina de Engenharia de Software[cite: 2]. |

---

# 📜 11. Regras de Negócio

Registre as regras do domínio que precisam ser respeitadas pelo sistema.

| ID | Regra de Negócio | Fonte |
|---|---|---|
| RN01 | Usuários devem estar autenticados para acessar funções sensíveis, como enviar pedidos ou mensagens[cite: 4]. | RNF01 (Segurança)[cite: 4] |
| RN02 | Uma planta não pode ser excluída do sistema enquanto houver pedidos de adoção pendentes associados a ela[cite: 4]. | RNF05 (Integridade)[cite: 4] |
| RN03 | Apenas o usuário proprietário (doador) pode aceitar ou rejeitar um pedido de adoção para sua planta[cite: 4]. | RF04 (Pedidos)[cite: 4] |

---

# 🔗 12. Rastreabilidade Inicial

Relacione as necessidades identificadas aos requisitos correspondentes.

| Necessidade | Stakeholder | Requisito(s) relacionado(s) |
|---|---|---|
| N01 | Todos os usuários | RF01, RNF01 |
| N02 | Doador | RF02, RNF05 |
| N03 | Adotante | RF03, RNF03 |
| N04 | Adotante | RF04, RNF05 |
| N05 | Todos os usuários | RF05, RNF03 |
| N06 | Todos os usuários | RNF01 |

---

# 🏷️ 13. Priorização dos Requisitos — Técnica MoSCoW

## Matriz de Priorização

| ID | Requisito | MoSCoW | Justificativa |
|---|---|:---:|---|
| RF01 | Cadastrar usuário[cite: 4] | M | Sem cadastro, não há controle de usuários ou segurança. |
| RF02 | Anunciar planta[cite: 4] | M | Funcionalidade core do sistema (oferta). |
| RF03 | Buscar e filtrar[cite: 4] | M | Funcionalidade core do sistema (demanda). |
| RF04 | Enviar pedido[cite: 4] | M | Mecanismo principal de conexão entre as partes. |
| RF05 | Comunicação[cite: 4] | M | Essencial para viabilizar a entrega da planta. |
| RF06 | Avaliar e comentar[cite: 4] | C | Bom para gerar confiança, mas o sistema funciona sem isso na V1. |
| RF07 | Gerenciar perfil[cite: 4] | S | Importante para manter dados atualizados, mas pode ser feito em uma segunda iteração se necessário. |
| RQ01 | Segurança (RNF01)[cite: 4] | M | Proteção de dados é requisito legal (LGPD). |
| RQ02 | Usabilidade (RNF02)[cite: 4] | M | Garante que o público-alvo conseguirá usar a ferramenta. |
| RQ03 | Desempenho (RNF03)[cite: 4] | S | Tempos de resposta otimizados são importantes, mas uma leve lentidão na V1 não impede o uso. |
| RQ04 | Disponibilidade (RNF04)[cite: 4] | M | O sistema precisa estar no ar para cumprir seu papel. |
| RQ05 | Integridade (RNF05)[cite: 4] | M | Evita corrupção de dados e falhas nas transações de adoção. |
| RQ06 | Escalabilidade (RNF06)[cite: 4] | C | Otimização para grandes volumes pode ser implementada conforme o crescimento real. |

---

# 🚀 14. Requisitos da Primeira Versão

Após aplicar a técnica MoSCoW, selecionem os **5 requisitos considerados indispensáveis para a primeira versão**.

| Ordem | ID | Requisito | Por que deve estar na primeira versão? |
|:---:|---|---|---|
| 1 | RF01 | Cadastrar usuário[cite: 4] | Garante a base de usuários autenticados, essencial para rastreabilidade e segurança[cite: 4]. |
| 2 | RF02 | Anunciar planta para adoção[cite: 4] | É o que alimenta o sistema com o "produto" (plantas), sem isso não há o que adotar. |
| 3 | RF03 | Buscar e filtrar plantas[cite: 4] | Permite que os interessados encontrem as plantas anunciadas. |
| 4 | RF04 | Enviar pedido de adoção[cite: 4] | Formaliza o interesse e inicia o processo de adoção. |
| 5 | RF05 | Comunicação entre usuários[cite: 4] | Permite o alinhamento logístico (entrega/retirada) para concluir a adoção. |

---

# ⏭️ 15. Requisitos para Versões Futuras

Selecionem pelo menos três requisitos que poderão ser adiados.

| ID | Requisito | Motivo para adiar | Impacto |
|---|---|---|---|
| RF06 | Avaliar e comentar[cite: 4] | Requisito "Could Have". O fluxo principal de adoção funciona sem o sistema de reputação inicialmente. | Menor confiança inicial entre desconhecidos. |
| RQ06 | Escalabilidade (10.000 usuários)[cite: 4] | Requisito "Could Have". A base de usuários inicial será pequena, permitindo otimizar a infraestrutura depois. | Possível lentidão se houver um pico inesperado de acessos no lançamento. |
| RF07 | Gerenciar perfil completo[cite: 4] | Requisito "Should Have". O foco inicial deve ser no fluxo de adoção, a edição complexa de perfil pode aguardar. | Usuários não poderão alterar fotos ou preferências imediatamente. |

---

# 🔍 16. Revisão por Pares

**Grupo responsável pela revisão:** (A preencher pelos revisores)

| ID do Requisito | Problema Encontrado | Sugestão de Melhoria |
|---|---|---|
| | | |

---

# ✅ 17. Checklist de Qualidade dos Requisitos

- [X] Os requisitos estão completos?
- [X] Os requisitos estão corretos em relação às necessidades?
- [X] Cada requisito representa uma única capacidade ou característica?
- [X] Os requisitos são necessários?
- [X] Os requisitos são viáveis?
- [X] Todos possuem prioridade?
- [X] Termos ambíguos foram eliminados?
- [X] Os requisitos podem ser verificados ou testados?
- [X] A fonte ou stakeholder está identificado?
- [X] As necessidades estão relacionadas aos requisitos?
- [X] Os requisitos de qualidade são mensuráveis sempre que possível?
- [X] As prioridades MoSCoW possuem justificativa?

---

# 💭 18. Reflexão do Grupo

## 18.1 Qual requisito gerou mais discussão durante o levantamento? Por quê?

> A comunicação entre usuários (RF05)[cite: 4]. Discutimos se seria necessário um chat interno em tempo real ou apenas a disponibilização do contato (como WhatsApp) após o aceite do pedido, devido à complexidade de implementar um chat robusto.

---

## 18.2 Qual necessidade inicialmente parecia simples, mas gerou vários requisitos?

> O processo de adoção. Inicialmente parecia ser apenas um clique, mas desdobrou-se na necessidade de envio de pedido, aceite/recusa do doador, comunicação e regras de integridade (não excluir planta com pedido em andamento).

---

## 18.3 O grupo identificou algum requisito implícito durante a discussão?

> Sim, a necessidade de adequação à LGPD (RNF01) e a garantia de que as fotos inseridas fossem de tamanhos adequados para não prejudicar o desempenho (RNF03)[cite: 4].

---

## 18.4 Qual requisito foi mais difícil de priorizar utilizando MoSCoW? Por quê?

> A avaliação de usuários (RF06)[cite: 4]. É um recurso muito importante para gerar segurança na comunidade, mas tecnicamente não é essencial para o fluxo básico (Minimum Viable Product), acabando classificado como "Could Have".

---

## 18.5 Houve algum requisito inicialmente considerado Must que mudou de prioridade?

> Sim, a edição detalhada do perfil (RF07)[cite: 4]. Percebemos que na primeira versão o usuário só precisa criar a conta e usar o sistema. A edição de dados não é bloqueante para a adoção em si, passando para "Should Have".

---

# 📝 19. Conclusão

**Conclusão:**

> O projeto PlantTinder investigou a dificuldade de realizar a adoção responsável de plantas devido à falta de plataformas centralizadas. Identificamos que os principais stakeholders são os doadores e adotantes, cujas necessidades mais relevantes são um ambiente seguro para anunciar, buscar e gerenciar o processo de adoção. Os requisitos considerados essenciais (Must Have) focam exclusivamente na jornada principal: cadastro, anúncio, busca, pedido e comunicação. A técnica MoSCoW foi fundamental para evitar o excesso de escopo (scope creep), permitindo que o grupo separasse funcionalidades desejáveis (como sistema de avaliações e perfil complexo) das funcionalidades vitais para a primeira versão do sistema.

---

# 📚 Referência

REINEHR, Sheila. **Requisitos de Software**. Material de apoio utilizado na disciplina Engenharia de Requisitos.

---

**Disciplina:** Engenharia de Software[cite: 2]
**Projeto:** Levantamento e Priorização de Requisitos  
**Profª Kadidja Valéria**
