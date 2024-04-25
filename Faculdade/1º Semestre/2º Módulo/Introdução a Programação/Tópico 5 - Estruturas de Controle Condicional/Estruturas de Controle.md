#Python #IntroduçãoAProgramação #Programação 

- IF, ELSE e ELIF são estruturas que variam muito pouco de linguagem para linguagem
- Sempre prestar muita atenção da sintaxe, qualquer erro quebra o código
- A estrutura do IF em python fica assim
```Python
if condição:
	bloco de código

# Prestar atenção na indentação, o bloco de código pertencente ao IF
# deve estar alinhado à direita para que funciona corretamente.
```
- Caso a condição seja verdadeira, o bloco de código será executado
```python
# Definimos uma variável e atribuimos um valor
idade = 18
# Aqui usamos um operador de comparação como nossa condição
if idade < 25:
	print("Jovem")
# O print só será executado caso o valor da variável idade seja menor que 25
```
- Preste <span style="color:#ee2020">MUITA</span> <span style="color:#ee2020">ATENÇÃO</span> na indentação e no uso dos pontos 
- Em python, os dois pontos denotam o início de um bloco de código indentado
- Caso falte indentação, ocorrerá um erro
	- ![](img/Pasted%20image%2020240425134755.png)
- Podemos usar os operadores lógicos nos IF para criar condições mais específicas
```python
idade = 29

if idade <= 12:
	print('Criança')
if idade > 12 and <= 25:
	print ('Jovem')
if idade > 25 and <= 60:
	print('Adulto')
if idade >=60:
	print('Idoso')
```
- O python executa o código linha a linha, mesmo encontrando a resposta no terceiro IF, ele continuará executando a última linha, tomando mais processamento e levando mais tempo na execução do nosso programa.
```python
if idade <= 12:
	print('Criança')
else:
	if idade > 12 and <= 25:
		print ('Jovem')
	else:
		if idade > 25 and < 60:
			print('Adulto')
		else: 
			print('Idoso')
```
- Adicionando o ELSE nós podemos PARAR o código assim que a condição de algum IF for atingida
- 