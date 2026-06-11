# Casos de Teste

## TC_LOGIN_01 – Login com credenciais válidas

**Pré-condição:** Usuário previamente cadastrado.

**Passos:**

1. Acessar página de login.
2. Inserir e-mail válido.
3. Inserir senha válida.
4. Clicar em "Entrar".

**Resultado Esperado:** Usuário autenticado e redirecionado para a página inicial.

**Resultado Obtido:** Login realizado com sucesso.

**Status:** ✅ Aprovado

---

## TC_CART_01 – Adicionar produto ao carrinho

**Pré-condição:** Usuário na listagem de produtos.

**Passos:**

1. Selecionar produto.
2. Clicar em "Adicionar ao carrinho".

**Resultado Esperado:** Produto exibido no carrinho.

**Resultado Obtido:** Funcionamento correto.

**Status:** ✅ Aprovado

---

## TC_CHECKOUT_01 – Preenchimento de dados no checkout

**Pré-condição:** Usuário logado com produto no carrinho.

**Passos:**

1. Acessar carrinho.
2. Clicar em "Checkout".
3. Preencher First Name.
4. Preencher Last Name.
5. Preencher Postal Code.
6. Clicar em "Continue".

**Resultado Esperado:** Sistema deve avançar para a próxima etapa.

**Resultado Obtido:** Tela branca ao preencher o campo Last Name.

**Status:** ❌ Reprovado

**Severidade:** Alta

**Prioridade:** Alta

**Bug Relacionado:** BUG_CHECKOUT_01

---

## TC_LOGIN_02 – Login com e-mail vazio

**Pré-condição:** Tela de login aberta.

**Passos:**

1. Deixar campo e-mail vazio.
2. Inserir senha válida.
3. Clicar em "Entrar".

**Resultado Esperado:** Exibir mensagem de campo obrigatório.

**Resultado Obtido:** Mensagem exibida corretamente.

**Status:** ✅ Aprovado

---

## TC_LOGIN_03 – Login com senha vazia

**Passos:**

1. Inserir e-mail válido.
2. Deixar senha vazia.
3. Clicar em "Entrar".

**Resultado Esperado:** Exibir mensagem de campo obrigatório.

**Resultado Obtido:** Mensagem exibida corretamente.

**Status:** ✅ Aprovado

---

## TC_REGISTER_01 – Cadastro com e-mail inválido

**Pré-condição:** Acesso à tela de cadastro.

**Passos:**

1. Inserir nome válido.
2. Inserir e-mail inválido.
3. Inserir senha válida.
4. Confirmar senha.
5. Clicar em "Cadastrar".

**Resultado Esperado:** Sistema deve impedir o cadastro.

**Resultado Obtido:** Cadastro realizado com sucesso.

**Status:** ❌ Reprovado

**Severidade:** Média

**Prioridade:** Alta

**Bug Relacionado:** BUG_REGISTER_01

---

## TC_CART_02 – Remover produto do carrinho

**Pré-condição:** Produto no carrinho.

**Passos:**

1. Acessar carrinho.
2. Clicar em remover.

**Resultado Esperado:** Produto removido.

**Resultado Obtido:** Funcionamento correto.

**Status:** ✅ Aprovado

---

## TC_CART_03 – Adicionar múltiplos produtos

**Pré-condição:** Usuário logado.

**Passos:**

1. Adicionar produto A.
2. Adicionar produto B.

**Resultado Esperado:** Ambos os produtos devem ser exibidos no carrinho.

**Resultado Obtido:** Funcionamento correto.

**Status:** ✅ Aprovado

---

## TC_CHECKOUT_02 – Finalizar compra sem pagamento

**Pré-condição:** Produto no carrinho.

**Passos:**

1. Acessar carrinho.
2. Clicar em finalizar compra.
3. Não preencher os dados de pagamento.
4. Confirmar a compra.

**Resultado Esperado:** Sistema deve bloquear a ação.

**Resultado Obtido:** Compra finalizada com sucesso.

**Status:** ❌ Reprovado

**Severidade:** Alta

**Prioridade:** Alta

**Bug Relacionado:** BUG_PAYMENT_01
