
---

# 📚 Referência

REINEHR, Sheila. **Engenharia de Requisitos**. Bookman, 2020.

---
---

# 📑 FICHAS DE ELICITAÇÃO DE REQUISITOS (UDF)

---

## 📄 Ficha REQ-001 — Cadastro de Usuários


### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de autenticação, perfil e gerenciamento de acesso. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Todos os Usuários (Doadores e Adotantes) |
| Relação com o projeto | Usuário final |
| Contato ou setor (se aplicável) | Comunidade doadores/adotantes de plantas |
| Técnica e data da elicitação | Entrevista / Questionário (24/09/2026) |
| Responsável pelo registro | Davi Gonçalves Castro |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-001 (RF01) |
| Necessidade relatada pelo stakeholder | "Preciso me cadastrar na plataforma para poder doar ou adotar plantas de forma segura." |
| Descrição consolidada | O sistema deve permitir que novos usuários se cadastrem na plataforma fornecendo dados pessoais (nome, e-mail, senha, localização) e preferências de cultivo. |
| Justificativa ou benefício esperado | Garantir a identificação, rastreabilidade e segurança dos usuários na comunidade. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende de validação das diretrizes da LGPD (RNF01). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para acessar funções sensíveis. | RNF01 (Segurança) |
| RN-002 | O e-mail cadastrado deve ser único na plataforma. | Equipe de Desenvolvimento |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** Sem cadastro e autenticação, o sistema não possui controle de acesso nem segurança para os dados pessoais.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado que o usuário preencheu todos os campos obrigatórios válidos, quando clicar em "Cadastrar", então o sistema cria a conta e redireciona para a tela inicial. | Teste de cadastro com dados válidos e checagem no banco de dados. |
| CA-02 | Dado que o e-mail informado já está cadastrado, quando o usuário tentar finalizar o cadastro, então o sistema exibe mensagem de erro e impede o cadastro duplicado. | Teste unitário de e-mail duplicado. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Senhas devem ser armazenadas com criptografia (hash seguro). |
| Links relacionados | [GitHub - MF-DAVI](https://github.com/MF-DAVI) |

---

## 📄 Ficha REQ-002 — Anúncio de Plantas para Adoção


### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de gestão de anúncios de doação. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Doadores de Plantas (ST01) |
| Relação com o projeto | Usuário final (Doador) |
| Contato ou setor (se aplicável) | Doadores |
| Técnica e data da elicitação | Oficina / Entrevista (24/09/2026) |
| Responsável pelo registro | João Pedro Alves De Sousa |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-002 (RF02) |
| Necessidade relatada pelo stakeholder | "Quero cadastrar as plantas que tenho para doar com foto e detalhes dos cuidados que ela precisa." |
| Descrição consolidada | O sistema deve permitir que doadores cadastrem anúncios de plantas informando espécie, fotos, tamanho, cuidados específicos e localização de retirada. |
| Justificativa ou benefício esperado | Ofertar espécies na plataforma e esclarecer o nível de cuidado exigido antes do processo de adoção. |
| Tipo | Funcional |
| Dependências ou dúvidas | Requer estar autenticado (REQ-001). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Apenas usuários autenticados podem criar anúncios. | RNF01 |
| RN-003 | Uma planta cadastrada não pode ter campos obrigatórios (espécie, fotos e localização) em branco. | RNF05 (Integridade) |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** É a funcionalidade core da oferta. Sem plantas anunciadas, o sistema não possui catálogo para adoção.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um usuário autenticado com dados da planta preenchidos, quando submeter o anúncio, então o sistema publica a planta no catálogo. | Teste funcional de criação de postagem. |
| CA-02 | Dado um formulário de anúncio sem fotos anexadas, quando o doador tentar salvar, então o sistema bloqueia e exige pelo menos uma imagem. | Validação no frontend e backend. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Fotos devem passar por compressão para não degradar o tempo de carregamento (RNF03). |
| Links relacionados | [GitHub - jpedro-swe](https://github.com/jpedro-swe) |

---

## 📄 Ficha REQ-003 — Busca e Filtro de Plantas


### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de pesquisa, navegação e catálogo de anúncios. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Adotantes de Plantas (ST02) |
| Relação com o projeto | Usuário final (Adotante) |
| Contato ou setor (se aplicável) | Adotantes de plantas |
| Técnica e data da elicitação | Questionário / Análise de usabilidade (24/09/2026) |
| Responsável pelo registro | Hélter Brandão De Oliveira |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-003 (RF03) |
| Necessidade relatada pelo stakeholder | "Quero procurar plantas disponíveis perto da minha casa e filtrar por tamanho ou facilidade de cuidar." |
| Descrição consolidada | O sistema deve permitir que usuários busquem e filtrem plantas por espécie, porte/tamanho, localização e requisitos de cuidados. |
| Justificativa ou benefício esperado | Permitir que adotantes encontrem plantas adequadas à sua região e ao seu espaço disponível. |
| Tipo | Funcional |
| Dependências ou dúvidas | Pode requerer suporte à integração com API de geolocalização. |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-004 | Anúncios desativados ou com adoção concluída não devem aparecer nos resultados de busca pública. | Regra do Domínio |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** É a funcionalidade core da demanda. Permite o encontro entre o adotante e a planta desejada.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um filtro selecionado (ex: "Porte Pequeno"), quando o adotante pesquisar, então o sistema exibe apenas plantas correspondentes a esse critério. | Teste de integração de filtros no catálogo. |
| CA-02 | Dado um parâmetro de busca sem resultados, quando pesquisado, então o sistema exibe mensagem de "Nenhuma planta encontrada". | Verificação da interface e tratamento de lista vazia. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | O tempo de resposta da busca deve cumprir o limite estipulado em RNF03 (até 2s). |
| Links relacionados | [GitHub - brandao395](https://github.com/brandao395) |

---

## 📄 Ficha REQ-004 — Solicitação de Adoção


### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de gerenciamento do processo de adoção. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Adotantes e Doadores (ST01 e ST02) |
| Relação com o projeto | Usuários finais |
| Contato ou setor (se aplicável) | Comunidade doadores/adotantes |
| Técnica e data da elicitação | Oficina de Requisitos (24/09/2026) |
| Responsável pelo registro | Jorge Luis Soares do Santos |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-004 (RF04) |
| Necessidade relatada pelo stakeholder | "Quero mandar uma solicitação formal demonstrando interesse em adotar a planta para que o doador analise." |
| Descrição consolidada | O sistema deve permitir que um adotante autenticado envie um pedido de adoção para o doador de uma planta e que este doador aceite ou recuse a solicitação. |
| Justificativa ou benefício esperado | Formalizar e organizar o interesse, evitando interações desordenadas sobre o mesmo anúncio. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende de REQ-001 (autenticação) e REQ-002 (existência da planta). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para solicitar adoção. | RNF01 |
| RN-005 | Apenas o doador proprietário da planta pode aceitar ou rejeitar a solicitação. | RN03 / RNF05 |
| RN-006 | Uma planta com pedido de adoção pendente não pode ser removida do sistema. | RN02 / RNF05 |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** É a ação transacional do sistema (o "match") que formaliza o início do processo de transferência da planta.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um adotante interessado, quando ele clica em "Solicitar Adoção", então o sistema registra o pedido e notifica o doador. | Teste de fluxo transacional e notificação. |
| CA-02 | Dado um pedido em aberto, quando o doador clica em "Aceitar", então a solicitação muda de status para "Aprovada" e libera o canal de comunicação. | Teste de transição de status no pedido. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Múltiplos pedidos podem ser recebidos pelo doador antes do aceite. |
| Links relacionados | [GitHub - 7deo](https://github.com/7deo) |

---

## 📄 Ficha REQ-005 — Troca de Mensagens (Comunicação)


### 1. Identificação do projeto
| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de mensagens e logística de entrega. |

### 2. Stakeholder e fonte
| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Todos os Usuários (Doadores e Adotantes) |
| Relação com o projeto | Usuários finais |
| Contato ou setor (se aplicável) | Comunidade doadores/adotantes |
| Técnica e data da elicitação | Entrevista / Análise documental (24/09/2026) |
| Responsável pelo registro | Davi Gonçalves Castro |

### 3. Requisito elicitado
| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-005 (RF05) |
| Necessidade relatada pelo stakeholder | "Preciso conversar com a pessoa para combinar o dia, horário e local onde vou retirar ou entregar a planta." |
| Descrição consolidada | O sistema deve disponibilizar um canal interno de troca de mensagens entre o doador e o adotante após a solicitação de adoção. |
| Justificativa ou benefício esperado | Viabilizar o alinhamento logístico entre as partes garantindo privacidade de dados pessoais no contato inicial. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende da aceitação ou envio da solicitação (REQ-004). |

### 4. Regras de negócio
| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para enviar mensagens. | RNF01 |
| RN-007 | O chat só pode ser iniciado entre doador e adotante atrelados a um pedido de adoção ativo. | Regra do Domínio |

### 5. Prioridade
**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  
**Justificativa da prioridade:** Sem comunicação, as partes não conseguem combinar a logística de retirada/entrega física da planta.

### 6. Critérios de aceitação
| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um pedido de adoção ativo, quando um dos usuários digita e envia uma mensagem, então ela deve ser entregue no painel do destinatário. | Teste de envio e recebimento de mensagens. |
| CA-02 | Dado um usuário não envolvido na adoção, quando tentar acessar a conversa alheia, então o acesso é negado. | Teste de permissão e segurança. |

### 7. Validação e rastreabilidade
| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24/09/2026 |
| Observações e decisões | Na Versão 1 (MVP) será um chat básico assíncrono. |
| Links relacionados | [GitHub - MF-DAVI](https://github.com/MF-DAVI) |
