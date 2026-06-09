CENÁRIO 05 – E-COMMERCE

 1. Entidades (Classes)

 Principais

* Cliente
* Produto
* Carrinho
* Pedido
* ItemPedido
* Pagamento
* Entrega

 Formas de Pagamento

* PagamentoCartao
* PagamentoPix
* PagamentoBoleto

 Tipos de Entrega

* EntregaNormal
* EntregaExpressa

 2. Métodos

 Carrinho

* adicionarProduto()
* removerProduto()
* calcularTotal()
* converterPedido()

 Pedido

* gerarPedido()
* calcularValorFinal()

 ItemPedido

* calcularSubtotal()

 Pagamento

* realizarPagamento()

 Entrega

* calcularFrete()
* calcularPrazo()

 3. Interfaces

 Interface IPagamento

Método:

* realizarPagamento()

Implementações:

* Cartão
* Pix
* Boleto

 Interface ITipoEntrega

Métodos:

* calcularFrete()
* calcularPrazo()

Implementações:

* EntregaNormal
* EntregaExpressa

 4. Relacionamentos

* Cliente possui um Carrinho.
* Carrinho possui vários Produtos.
* Carrinho gera um Pedido.
* Pedido possui vários Itens.
* Cada Item referencia um Produto.
* Pedido possui um Pagamento.
* Pedido possui uma Entrega.

 5. Tratamento de Exceções

Possíveis exceções:

* Produto sem estoque.
* Carrinho vazio.
* Pagamento recusado.
* Endereço inválido.

Exemplo:

* EstoqueInsuficienteException
* CarrinhoVazioException
* PagamentoNaoAprovadoException


 CONCLUSÃO

Os cinco cenários utilizam conceitos fundamentais da Orientação a Objetos:

* Herança
* Polimorfismo
* Interfaces
* Associação
* Composição
* Encapsulamento
* Tratamento de Exceções
