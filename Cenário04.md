 CENÁRIO 04 – PLATAFORMA DE STREAMING

 1. Entidades (Classes)

* Usuario
* Plano (abstrata)
* Conteudo
* Assinatura
* Pagamento

Especializações de Plano:

* PlanoBasico
* PlanoPremium

Especializações de Conteúdo:

* Filme
* Serie

Formas de pagamento:

* PagamentoCartao
* PagamentoPix

 2. Métodos

 Usuario

* assinarPlano()
* assistirConteudo()

 Plano

* verificarAcesso()

 Assinatura

* renovar()
* cancelar()

 Conteudo

* reproduzir()

 3. Interfaces

 Interface IPagamento

Método:

* processarPagamento()

 Interface IAcesso

Método:

* verificarAcesso()

 4. Relacionamentos

* Usuário possui uma Assinatura.
* Assinatura está vinculada a um Plano.
* Plano pode ser Básico ou Premium.
* Conteúdo pode ser Filme ou Série.
* Pagamento pode ocorrer por Cartão ou Pix.

 5. Tratamento de Exceções

Possíveis exceções:

* Assinatura vencida.
* Pagamento recusado.
* Conteúdo indisponível para o plano.

Exemplo:

* AssinaturaExpiradaException
* AcessoNegadoException
