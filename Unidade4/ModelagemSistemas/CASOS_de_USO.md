# PlantTinder 🌱

## Diagrama de Caso de Uso

O PlantTinder possui funcionalidades voltadas ao cadastro de usuários, gerenciamento de plantas, solicitação de adoção e comunicação entre adotantes e doadores.

## Atores

- **Visitante:** usuário que acessa o sistema sem estar autenticado.
- **Adotante:** usuário interessado em buscar plantas e solicitar sua adoção.
- **Doador:** usuário responsável por cadastrar e gerenciar plantas disponíveis para adoção.

## Casos de Uso

| Código | Caso de uso | Descrição |
|---|---|---|
| UC01 | Criar Conta | Permite criar uma conta no sistema. |
| UC02 | Validar E-mail | Realiza a validação do e-mail do usuário. |
| UC03 | Fazer Login | Permite acessar o sistema por meio de uma conta. |
| UC04 | Cadastrar Planta | Permite cadastrar uma planta para adoção. |
| UC05 | Editar / Remover Planta | Permite editar ou remover uma planta cadastrada. |
| UC06 | Buscar / Visualizar Catálogo de Plantas | Permite buscar e visualizar as plantas disponíveis. |
| UC07 | Enviar Solicitação de Adoção | Permite enviar uma solicitação para adotar uma planta. |
| UC08 | Gerenciar Solicitações | Permite gerenciar as solicitações de adoção. |
| UC09 | Chat Direto | Permite a comunicação direta entre usuários. |
| UC10 | Avaliar Adotante / Doador | Permite avaliar o adotante ou o doador. |

## Relacionamentos

- **UC01 — Criar Conta** inclui **UC02 — Validar E-mail** (`<<include>>`).

## Regras de Acesso Representadas

- O doador pode cadastrar, editar e remover plantas.
- O catálogo de plantas pode ser consultado pelos usuários.
- O adotante pode enviar solicitações de adoção.
- O sistema contempla gerenciamento de solicitações, chat direto e avaliação entre adotantes e doadores.

---

**Projeto:** PlantTinder  
**Tipo de documentação:** Diagrama UML de Caso de Uso
