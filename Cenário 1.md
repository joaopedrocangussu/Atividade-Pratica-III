# Atividade-Pratica-III


 CENÁRIO 01 – ESTACIONAMENTO

 1. Entidades (Classes)

Classes principais:

* Veiculo (abstrata)
* Carro
* Moto
* Caminhao
* Ticket
* Estacionamento
* Pagamento

Classes de pagamento:

* PagamentoDinheiro
* PagamentoCartao

 2. Métodos

Veiculo

* calcularValor(int horas)

 Carro

* calcularValor()

 Moto

* calcularValor()

 Caminhao

* calcularValor()

 Ticket

* registrarEntrada()
* registrarSaida()
* calcularTempo()

 Estacionamento

* gerarTicket()
* encerrarTicket()

 Pagamento

* realizarPagamento(valor)

 3. Interfaces

Interface IPagamento

Responsável por definir o comportamento dos meios de pagamento.

Método:

* realizarPagamento(double valor)

Implementações:

* PagamentoDinheiro
* PagamentoCartao

 Interface ICobranca (Opcional)

Método:

* calcularValor(int horas)

3 4. Relacionamentos

* Veiculo é superclasse de Carro, Moto e Caminhao.
* Ticket possui um Veiculo.
* Estacionamento gerencia vários Tickets.
* Pagamento possui especializações Cartão e Dinheiro.

 5. Tratamento de Exceções

Possíveis exceções:

* Ticket inexistente.
* Saída sem ticket.
* Tempo inválido.
* Falha no pagamento.

Exemplo:

* TicketNaoEncontradoException
* PagamentoNaoRealizadoException
