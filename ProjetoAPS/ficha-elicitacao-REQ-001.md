# Ficha de Elicitação de Requisitos — REQ-001

**Curso:** Engenharia de Software  
**Disciplina:** Análise e Projeto de Sistemas  
**Instituição:** UDF Centro Universitário  
**Grupo/integrantes:** João Pedro Alves De Sousa, Hélter Brandão De Oliveira, Davi Gonçalves Castro, Jorge Luis Soares do Santos  
**Turma:** D2 | **Data:** 10/09/2026 | **Versão:** 1.0  

---

## 1. Identificação do projeto

| Campo | Preenchimento |
|---|---|
| Nome do projeto | Rede de Apoio para Adoção de Plantas (PlantTinder) |
| Objetivo do projeto | Facilitar a doação e adoção responsável de plantas por meio do matching de perfis e comunicação direta entre usuários. |
| Contexto e escopo | Módulo de autenticação, perfil e gerenciamento de acesso. |

---

## 2. Stakeholder e fonte

| Campo | Preenchimento |
|---|---|
| Stakeholder (nome ou papel) | Todos os Usuários (Doadores e Adotantes) |
| Relação com o projeto | Usuário final |
| Contato ou setor (se aplicável) | Comunidade doadores/adotantes de plantas |
| Técnica e data da elicitação | Entrevista / Questionário (10/09/2026) |
| Responsável pelo registro | Davi Gonçalves Castro |

---

## 3. Requisito elicitado

| Campo | Preenchimento |
|---|---|
| ID do requisito | REQ-001 (RF01) |
| Necessidade relatada pelo stakeholder | "Preciso me cadastrar na plataforma para poder doar ou adotar plantas de forma segura." |
| Descrição consolidada | O sistema deve permitir que novos usuários se cadastrem na plataforma fornecendo dados pessoais (nome, e-mail, senha, localização) e preferências de cultivo. |
| Justificativa ou benefício esperado | Garantir a identificação, rastreabilidade e segurança dos usuários na comunidade. |
| Tipo | Funcional |
| Dependências ou dúvidas | Depende de validação das diretrizes da LGPD (RNF01). |

---

## 4. Regras de negócio

| ID | Regra de negócio relacionada | Fonte ou responsável pela validação |
|---|---|---|
| RN-001 | Usuários devem estar autenticados para acessar funções sensíveis. | RNF01 (Segurança) |
| RN-002 | O e-mail cadastrado deve ser único na plataforma. | Equipe de Desenvolvimento |

---

## 5. Prioridade

**Classificação MoSCoW:** [X] Must have (essencial)  [ ] Should have  [ ] Could have  [ ] Won't have nesta versão  

**Justificativa da prioridade:** Sem cadastro e autenticação, o sistema não possui controle de acesso nem segurança para os dados pessoais.

---

## 6. Critérios de aceitação

| ID | Dado/Quando | Então (resultado esperado) | Evidência ou forma de verificação |
|---|---|---|---|
| CA-01 | Dado que o usuário preencheu todos os campos obrigatórios válidos, quando clicar em "Cadastrar", então o sistema cria a conta e redireciona para a tela inicial. | Teste de cadastro com dados válidos e checagem no banco de dados. |
| CA-02 | Dado que o e-mail informado já está cadastrado, quando o usuário tentar finalizar o cadastro, então o sistema exibe mensagem de erro e impede o cadastro duplicado. | Teste unitário de e-mail duplicado. |

---

## 7. Validação e rastreabilidade

| Campo | Preenchimento |
|---|---|
| Situação | [ ] Pendente de validação  [X] Validado  [ ] Necessita revisão |
| Validado por / data | Profª Kadidja Valéria / 10/09/2026 |
| Observações e decisões | Senhas devem ser armazenadas com criptografia (hash seguro). |
| Links relacionados | [RF01 no Documento Principal](https://github.com/MF-DAVI) |
