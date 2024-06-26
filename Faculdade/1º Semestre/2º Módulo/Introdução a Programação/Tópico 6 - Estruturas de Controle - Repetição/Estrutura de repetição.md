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
- Podemos acessar os dados através do índice, e com isso criarmos iterações a partir do fatiamento dos índices.
- Podemos usar o <span style="color:#f04ff3">CONTINUE</span> nos nossos loops, basicamente oque ele faz é sempre que a condicional aonde ele está colocado for verdadeira, o loop será reiniciado.
```python
lista = [0,1,2,3,4,5,6,7,8,9,10]

for i in lista:
	if i == 4:
		continue
	print('Item: ', i)
```
- O output que teremos será todos os itens da lista menos o 4 já que quando o condicional <span style="color:#f04ff3">IF</span> foi verdadeiro, o computador voltou para o inicio do loop, ignorando o comando <span style="color:#c5de0d">print</span> logo abaixo.
```python
cesta = ["maçã", "laranja", "pêra", "maçã", "laranja", "maçã", "uva", "mamão", "pêra"]
frutas_nao_gosto = []
frutas_gosto = ["maçã", "laranja"]

for fruta in cesta:
	if any([fruta in frutas_gosto, fruta in frutas_nao_gosto]):
		continue
	frutas_nao_gosto.append(fruta)
print(frutas_nao_gosto)
```
- Aqui checar se a fruta está em alguma cesta, caso ela esteja, o loop será resetado e passará para a próxima fruta (índice).
	- [Leitura extra para a função ANY()](https://www.programiz.com/python-programming/methods/built-in/any)

## Range
---

- Usamos a função range para construir uma lista de iteração
- Pode ser usada para construir a lista de iteração para o <span style="color:#f04ff3">FOR</span> para definirmos como o nosso loop será iterado
```python
sum, inicio, fim, lista = 0,1,5,[]

for x in range(inicio,fim):
	lista.append(x)
	sum += x
print(lista)
print(sum)
```
- A nossa iteração vai ATÉ o número q selecionamos, o seu final é EXCLUSIVO, ou seja, ele não inclui o valor definido como o fim.

## While
---

- Podemos criar um loop com VÁRIAS instruções usando o <span style="color:#f04ff3">WHILE</span> onde será realizado um teste a cada iteração

```python
contador = 0
fim = 10

while(contador < fim):
	contador += 1
	print(contador)
```

- Temos que tomar cuidado para não criarmos loops infinitos com o <span style="color:#f04ff3">WHILE</span> 
- Assim como no <span style="color:#f04ff3">FOR</span>, nós podemos usar o <span style="color:#f04ff3">BREAK</span> e o <span style="color:#f04ff3">CONTINUE</span> 
	- Assim como estrutura <span style="color:#f04ff3">IF</span> e <span style="color:#f04ff3">ELSE</span> 