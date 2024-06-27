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
