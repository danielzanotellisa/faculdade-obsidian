#Lógica #Programação #IntroduçãoAProgramação 

- Indicamos uma implicação lógica com a notação => 
- Quando temos duas proposições compostas P e Q, diz-se que ocorre uma implicação lógica sempre que Q for verdadeiro quando P for verdadeiro também 

| p   | q   | p ^ q |
| --- | --- | ----- |
| V   | V   | V     |
| V   | F   | F     |
| F   | V   | F     |
| F   | V   | F     |

- p ^ q implica p (p ^ q => p) porque todas as vezes em que a proposição composta p ^ q é verdadeira, p também é verdadeiro
- Ocorre uma implicação lógica entre duas proposições compostas quando o a proposição condicional (P -> Q) é uma tautologia.

| p   | q   | r   | p -> q | q -> r | (p->q) ^ (q->r) | p -> r | (p -> q) ^ (q -> r) -> (p -> r) |
| --- | --- | --- | ------ | ------ | --------------- | ------ | ------------------------------- |
| V   | V   | V   | V      | V      | V               | V      | V                               |
| V   | V   | F   | V      | F      | F               | F      | V                               |
| V   | F   | V   | F      | V      | F               | V      | V                               |
| V   | F   | F   | F      | V      | F               | F      | V                               |
| F   | V   | V   | V      | V      | V               | V      | V                               |
| F   | V   | F   | V      | F      | F               | V      | V                               |
| F   | F   | V   | V      | V      | V               | V      | V                               |
| F   | F   | F   | V      | V      | V               | V      | V                               |



