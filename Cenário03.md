CENÁRIO 03 – EMPRESA DE SERVIÇOS TÉCNICOS

 1. Entidades (Classes)

* Cliente
* Tecnico
* OrdemServico
* Servico (abstrata)

Especializações:

* Manutencao
* Instalacao
* Suporte

 2. Métodos

 OrdemServico

* abrir()
* atribuirTecnico()
* finalizar()
* calcularValor()

 Servico

* executar()
* calcularPreco()

 Manutencao

* executar()

### Instalacao

* executar()

 Suporte

* executar()

 3. Interfaces

 Interface IExecutavel

Método:

* executar()

Implementações:

* Manutencao
* Instalacao
* Suporte

 4. Relacionamentos

* Cliente abre Ordem de Serviço.
* Técnico executa Ordem de Serviço.
* Ordem de Serviço possui um Serviço.
* Serviço pode ser Manutenção, Instalação ou Suporte.

 5. Tratamento de Exceções

Possíveis exceções:

* Técnico indisponível.
* Ordem já finalizada.
* Serviço inexistente.
* Valor inválido.

Exemplo:

* TecnicoIndisponivelException
* OrdemJaFinalizadaException
