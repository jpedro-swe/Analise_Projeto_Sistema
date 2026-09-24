# Ficha de Elicitação de Requisitos

**Curso:** Engenharia de Software  
**Disciplina:** Análise e Projeto de Sistemas  
**Instituição:** UDF Centro Universitário  
**Grupo/integrantes:** [João Pedro Alves De Sousa](https://github.com/jpedro-swe) | [Hélter Brandão De Oliveira](https://github.com/brandao395) | [Davi Gonçalves Castro](https://github.com/MF-DAVI) | [Jorge Luis Soares do Santos](https://github.com/7deo)  
**Turma:** D2 - Engenharia de Software  **Data:** 24/09/2026  **Versão:** 1.0  

---

## 1. Identificação do projeto

| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | O projeto consiste no desenvolvimento de uma plataforma digital focada em conectar pessoas interessadas em adotar plantas com doadores. O objetivo principal é facilitar a adoção responsável por meio do matching de perfis, gerenciamento de anúncios e comunicação direta entre os usuários, reduzindo o descarte inadequado e a falta de informação sobre o manejo de espécies. |
| Contexto e escopo | Sistema web que permite a doadores e adotantes o cadastro de perfis, gerenciamento de anúncios de plantas, busca avançada por critérios (porte, espécie, localização), envio de solicitações de adoção e chat de comunicação. Nesta etapa, o trabalho se concentra na análise e levantamento de requisitos e elicitação por fichas padronizadas, sem envolver o desenvolvimento da infraestrutura completa. |

## 2. Stakeholder e fonte

| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | ST01 e ST02 — Doadores e Adotantes de Plantas (Stakeholders principais). |
| Relação com o projeto | Usuários principais: são diretamente afetados pela dificuldade de encontrar lares adequados para suas plantas ou de encontrar espécies para adoção de forma confiável e centralizada. Influência: alta. |
| Contato ou setor (se aplicável) | Comunidade de entusiastas de plantas, jardineiros amadores e pessoas interessadas em doação responsável. |
| Técnica e data da elicitação | Entrevista e questionário com usuários potenciais; 24 de setembro de 2026. |
| Responsável pelo registro | Davi Gonçalves Castro |

## 3. Requisito elicitado

| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-001 (corresponde ao RF01 do levantamento do grupo). |
| Necessidade relatada pelo stakeholder | N01 — “Criar conta para acessar a plataforma”: o usuário necessita de um ambiente seguro e identificado para poder realizar doações ou solicitações de adoção de forma rastreável. |
| Descrição consolidada | O sistema deve permitir que novos usuários se cadastrem na plataforma informando seus dados pessoais (nome, e-mail, senha, localização) e preferências de plantas. |
| Justificativa ou benefício esperado | É a função de entrada do sistema. Garante a autenticação, controle de acesso e rastreabilidade da comunidade de doadores e adotantes, assegurando o cumprimento de normas de segurança. |
| Tipo | Funcional. |
| Dependências ou dúvidas | 1) O sistema deve estar em conformidade estrita com as diretrizes da LGPD (RNF01 / RES01).<br>2) As senhas cadastradas exigem salvamento com criptografia (hash seguro).<br>3) O e-mail deve ser validado para evitar contas duplicadas ou fakes.<br>4) Requisitos de qualidade relacionados: RNF01 (segurança), RNF02 (usabilidade) e RNF04 (disponibilidade). |

## 4. Regras de negócio

| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para acessar funções sensíveis, como publicar anúncios, enviar solicitações de adoção ou trocar mensagens. | RNF01 (Segurança / LGPD) |
| RN-002 | O endereço de e-mail fornecido no cadastro deve ser único no sistema. | Regra do Domínio / Equipe de Desenvolvimento |

## 5. Prioridade

**Classificação MoSCoW (marque uma):** [x] Must have (essencial)  [ ] Should have (importante)  [ ] Could have (desejável)  [ ] Won't have nesta versão (fora do escopo atual)

**Justificativa da prioridade:** Sem a criação de contas e autenticação de usuários, não é possível ter rastreabilidade, segurança nos contatos nem controle sobre quem está doando ou adotando as plantas.

## 6. Critérios de aceitação

Escreva condições verificáveis que permitam decidir se o requisito foi atendido.

| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado um visitante não cadastrado, quando ele preencher o formulário com dados válidos e clicar em "Cadastrar" | Então o sistema registra a nova conta, efetua a criptografia da senha e redireciona o usuário para o painel principal. | Teste funcional de formulário e consulta direta ao banco de dados para checagem do hash da senha. |
| CA-02 | Dado um usuário tentando se cadastrar, quando ele fornecer um e-mail que já existe no sistema | Então o sistema exibe uma mensagem clara de erro e impede a criação da conta duplicada (RN02). | Teste unitário e de interface com e-mail preexistente. |
| CA-03 | Dado um usuário preenchendo o cadastro, quando ele omitir algum campo obrigatório (como nome ou senha) | Então o sistema sinaliza os campos pendentes e bloqueia o envio até o preenchimento correto (RNF02). | Teste de validação de campos no frontend e backend. |
| CA-04 | Dado o envio de dados do cadastro, quando a requisição for processada | Então a resposta do servidor ocorre em até 2 segundos sob condições normais de uso (RNF03). | Teste de desempenho e tempo de resposta de API. |

## 7. Validação e rastreabilidade

| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [x] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 24 de setembro de 2026. |
| Observações e decisões | Requisito classificado como Must have e incluído na primeira versão (MVP, ordem 1). Senhas obrigatoriamente salvas com hash seguro e dados pessoais protegidos sob os princípios da LGPD. |
| Links relacionados | Rastreabilidade: N01 → ST01 / ST02 → REQ-001 (RF01), relacionado a RF02, RF04, RNF01 e RNF02.<br>[Board do projeto no Miro](https://miro.com/app/board/uXjVHo3jFqo=/)<br>[Repositório GitHub — PlantTinder](https://github.com/jpedro-swe/Analise_Projeto_Sistema) |
