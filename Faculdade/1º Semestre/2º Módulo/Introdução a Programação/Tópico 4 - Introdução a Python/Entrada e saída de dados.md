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

print('Hoje é dia %d de %s'%(dia,mes))
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