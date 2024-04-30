#Python #Programação #IntroduçãoAProgramação 


- Loops são estruturas de repetição criadas para processar coleções de dados em um mesmo bloco de código.
- Computadores são ótimos em repetir as coisas 

## FOR
---

- Usado geralmente com listas ou tuplas ou um iterador.

```python

sequência = [1,2,3,4,5]
total = 0

for valor in sequencia:
	total += valor
print(total)
```

- Iteração na computação é só uma maneira bonita de dizer que algo vai ser repetido, quando dizemos que algo faz um incremento em cada iteração, quer dizer que algo vai ser acrescentado a cada repetição. Toda repetição da execução de um bloco de comandos que ocorre infinitamente ou com o encerramento em determinado momento atendendo alguma condição é uma iteração.
- No exemplo acima, a variável <span style="color:#8ef3f5">valor</span> muda a cada iteração(repetição)
	- Ela começa valendo 1, depois 2 e assim por diante até chegar no fim da lista.
```python 
sequência = [1, -7, 1+1J, 2, None, 3, 3.3, 4, 5] 
total = 0 
for valor in sequência: 
	if isinstance(valor,int) and valor >= 0: 
		total += valor 
print(total)
```
- Na estrutura acima adicionamos um condicional que só realizará a soma caso a variável <span style="color:#8ef3f5">valor</span> seja um tipo <span style="color:#8ef3f5">int</span> e maior que 0
	- A cada iteração ela assume o próximo valor, porém, só executa a soma caso seja um <span style="color:#8ef3f5">int</span> maior que 0
- O laço de repetição <span style="color:#f04ff3">FOR</span> possui uma estrutura <span style="color:#f04ff3">ELSE</span> 
```python
seq1 = [1,4,7,None,5+5j,5,12,9]
seq2 = []
total = 0
for var in seq1:
	if isinstance(var,int):
		seq2 = seq2 + [var]
	else:
		total = sum(seq2)
print('Sequência: ',seq2)
print('Total: 'total)
```
- Tudo oque esta dentro do <span style="color:#f04ff3">ELSE</span> só é executado no fim do bloco de código do <span style="color:#f04ff3">FOR</span> 
	- Quando usamos o comando <span style="color:#f04ff3">BREAK</span> para terminar a iteração antes do bloco de código do <span style="color:#f04ff3">ELSE</span>, o computador ignora todo aquele código.
- 