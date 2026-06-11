# BUG_PAYMENT_01 - Finalização sem pagamento

## Severidade

Alta

## Prioridade

Alta

## Descrição

O sistema permite finalizar uma compra sem o preenchimento dos dados de pagamento.

## Passos para Reproduzir

1. Adicionar um produto ao carrinho.
2. Acessar o checkout.
3. Não preencher os dados de pagamento.
4. Confirmar a compra.

## Resultado Esperado

O sistema deve impedir a finalização da compra e exibir uma mensagem de erro.

## Resultado Atual

A compra é finalizada com sucesso mesmo sem pagamento.

## Impacto

Falha crítica que compromete a segurança e a integridade do processo de compra.
