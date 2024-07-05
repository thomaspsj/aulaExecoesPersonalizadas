# Solução do problema

 ## First commit: 
 Solução 1 (muito ruim): lógica de validação no programa principal
- Lógica de validação não delegada à reserva
 
## Second commit: 
Solução 2 (ruim): método retornando string
- A semântica da operação é prejudicada
- Retornar string não tem nada a ver com atualização de reserva
- E se a operação tivesse que retornar um string?
- Ainda não é possível tratar exceções em construtores
- A lógica fica estruturada em condicionais aninhadas

 ## Third commit:
- Cláusula throw: lança a exceção / "corta" o método
- O modelo de tratamento de exceções permite que erros sejam tratados de forma consistente e flexível, usando boas práticas
- Vantagens:
- Lógica delegada
- Construtores podem ter exceções
- Código mais simples. Não há aninhamento de condicionais: a qualquer momento que uma exceção for disparada, a execução é interrompida e cai no bloco catch correspondente.
- É possível capturar inclusive outras exceções de sistema
