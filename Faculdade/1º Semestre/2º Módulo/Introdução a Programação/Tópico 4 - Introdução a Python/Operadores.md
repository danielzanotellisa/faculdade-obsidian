#Python #Programação #IntroduçãoAProgramação 

- Os operadores em python funcionam como nos da matemática convencional
```python
# Adição

1 + 1

# Subtração

1 - 1

# Multiplicação 

1 * 1

# Divisão

1 / 1

# Divisão exata 

1 // 1

# Resto inteiro da divisão entre dois números

1 % 1

# Potência

1 ** 1
```

- Podemos escrever constantes com a mesma notação usada na linguagem C
- Utilizamos o sufixo j para representar a parte imaginária de um número complexo

### Strings
---

- Existem caracteres não imprimíveis (consultar documentação) que alteram o comportamento das nossas strings na função print

```python
'ab\rd'

print('ab\rd')

print('ab\td')

print('abc\nd')
```

- Podemos desabilitar a função da barra invertida quando colocamos um r minúsculo na frente da string
```python
print(r'abc\d')
```

- É possível escrever as strings com TRÊS aspas duplas para não termos que escrever a quebra de linha ou uma barra invertida ao fim de cada linha
```python
print("""uma maçã
duas maçãs""")
```

- Os caracteres nas strings possuem índices, que começam em 0 (para o primeiro) e vão até o tamanho da string. Acessamos ele por meio dos colchetes '[]'
	- O índice -1 é o último caractere 
```python
a = 'teste de índice'
print(a[0])
print(a[-1])
```

- Para fazer o fatiamento das strings vamos usar os colchetes
```python
# Dentro dos colchetes passaremos 3 parâmetros separados por :
# [onde começa:onde termina:valor de iteração]
a = 'teste de índice'
print(a[0:2]) # Pegando todos os caracteres do índice 0 até o 2 

# Se o primeiro argumento é omitido, é assumido como 0
# Se o segundo argumento é omitido, é assumido o fim da STRING

print(a[::-1]) # Faz com que a string seja impressa ao contrário
```

### Expressões booleanas
---

- Usaremos os operadores relacionais e os booleanos E, OU, NÃO para criar nossa lógica
	- Operadores relacionais: > (maior), < (menor), == (igualdade), != (diferente), >= (maior igual), <= (menor igual)
- As avaliações são feitas da esquerda pra direita
	- Para imediatamente assim que o resultado é avaliado, ignorando o resto do código
- Qualquer valor não nulo é visto como VERDADEIRO
- O operador OR (ou) retorna o primeiro operando caso ele seja verdadeiro
- O operador AND (e) retorna o primeiro operando, se for visto como falso, caso contrário, retorna o segundo
- Os operadores relacionais são avaliados antes de NOT, que é avaliado antes de AND, que é avaliado antes de OR

### Módulos
---

- Além dos operadores podemos usar as funções para fazer determinadas operações
- O python possuem algumas funções embutidas como abs(), chr() e ord()