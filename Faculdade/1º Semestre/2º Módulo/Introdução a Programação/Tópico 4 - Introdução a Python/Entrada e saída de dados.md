#Python #Programação #IntroduçãoAProgramação 

- Python é uma linguagem interpretada, o interpretador executa um comando por vez para funcionar o código
- Podemos executar o código pela linha de comando
- Para criar comentários basta usarmos o caractere '#' ou com três aspas duplas antes e depois dos comentários, isso irá criar um bloco de comentário
- O Python usa a identação para estruturar o código
```python
for x in array:
	if x < pivot:
		less.append(x)
	else:
		greater.append(x)
```
- Podemos exibir os resultados com o comando <span style="color:#8ef3f5">print</span>()
	- Podemos dar saída nesses dados diretamente de uma variável, do próprio comando, ou de um módulo (como são chamados os programas em Python)
- Podemos também usar placeholders para mostrar dados através da interpolação de strings
```python
dia = 20
mes = dezembro

print('Hoje é dia %d de %s' %(dia,mes))
# Nesse caso estaremos usando um placeholder para que caso seja necessário mudar o dia ou o mês alteremos somente a variável e não a string em si


```
- Podemos também usar outros modos de formatação de strings
```python
nome = Daniel
idade = 24

# Usando f-strings para formatar
print(f"Olá, me chamo {nome} e tenho {idade} anos")

# Podemos usar o metodo .format()

print("Olá, me chamo {0} e tenho {1} anos".format(nome,idade))
# Podemos usar o valor do índice ou os nomes das variáveis
print("Olá, me chamo {nome} e tenho {idade} anos".format(nome,idade))
```
- Usamos o comando <span style="color:#d97f36">INPUT</span> para entrada de dados do usuário
```python
input("Digite seu nome por favor")

# Podemos salvar os dados em uma variável

nome = input("Digite seu nome por favor")

# A partir disso podemos usar a variável para oque quisermos

print(nome)

print("Meu nome é %s" % nome)
print(f'Meu nome é {nome}')
print('Meu nome é {nome}'.format(nome))
```
- Fazemos atribuição de valores usando o sinal de igualde '='
	- É possível atribuir várias variáveis de uma vez
```python

a = 1
a,b = 3*a, a
print(a,b)
a,b = b,a
print(a,b)
```

- O Python possui tipagem dinâmica, ou seja, os tipos são definidos dependendo da entrada de dados em uma variável
	- Existem algumas formas de <span style="color:#d97f36">TIPAGEM</span> 
		- <span style="color:#d97f36">TIPAGEM FORTE</span>: É necessário declarar explicitamente o tipo da variável que estamos alocando
		- <span style="color:#d97f36">TIPAGEM FRACA</span>: Não é necessário explicitar o tipo de dado
		- <span style="color:#d97f36">TIPAGEM DINÂMICA</span>: Além de não ser necessário explicitar o tipo de dado, é possível modificar o tipo quando quisermos
- O Python possui suas limitações com a tipagem, não podemos por exemplo, somar uma <span style="color:#d97f36">string</span> com um <span style="color:#d97f36">int</span>.
- Todos os dados que são coletados utilizando o comando INPUT são <span style="color:#d97f36">strings</span>, será necessário converter para outro TIPO caso seja necessário
```python
idade_cachorro = int(input('idade do cachorro'))
idade_humano = idade_cachorro*7
print(idade_humano)
```
- Usamos a palavra reservada <span style="color:#8ef3f5">def</span> para criar uma função


***Link de referência extra***: https://realpython.com/python-f-strings/#interpolating-and-formatting-strings-before-python-36