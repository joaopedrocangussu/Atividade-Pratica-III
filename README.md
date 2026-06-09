CENÁRIO 02 – PLATAFORMA DE CURSOS

 1. Entidades (Classes)

* Aluno
* Curso
* Aula
* Matricula
* Progresso
* Pagamento

Especializações:

* CursoGratuito
* CursoPago

Formas de pagamento:

* PagamentoCartao
* PagamentoPix

 2. Métodos

 Aluno

* matricular()
* consultarProgresso()

 Curso

* adicionarAula()
* listarAulas()

 Matricula

* registrarMatricula()

 Progresso

* registrarConclusaoAula()
* calcularPercentual()

 CursoPago

* processarPagamento()

 3. Interfaces

 Interface IPagamento

Método:

* realizarPagamento()

Implementações:

* PagamentoCartao
* PagamentoPix

 Interface IConsumivel

Método:

* assistirAula()

 4. Relacionamentos

* Aluno realiza Matrícula.
* Matrícula relaciona Aluno e Curso.
* Curso possui várias Aulas.
* Aluno possui um Progresso para cada Curso.
* Curso pode ser Gratuito ou Pago.
* Curso Pago utiliza Pagamento.

 5. Tratamento de Exceções

Possíveis exceções:

* Curso não encontrado.
* Matrícula duplicada.
* Pagamento recusado.
* Acesso a curso pago sem pagamento.

Exemplo:

* MatriculaDuplicadaException
* PagamentoNaoAprovadoException
