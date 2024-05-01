
#Python #Programação #Dados #IntroduçãoAProgramação 


- Estruturas homogêneas são aquelas em que todos os dados são do mesmo tipo
- Uma lista pode conter dados de tipos diferente ao mesmo tempo
- Podemos criar ARRAYS homogêneos com a biblioteca NUMPY
```python
import numpy as np

dado1 = [1,2,3,4,5]
array1 = np.array(dado1)
print(array1)

#OUTPUT
# [1 2 3 4 5]
```

```python
import numpy as np

dado2 = [[1,2,3],[4,5,6]]
array2 = np.array(dado2)
print(array2)

#OUTPUT
#[[1 2 3]
#  [4 5 6]]	
```

- <span style="color:#0ac2bf">DADO2</span> é uma lista de listas, o NDARRAY criado é um array multidimensional, no caso, um array bidimensional de 2 por 3, duas linhas e três colunas.
- Ao importar uma biblioteca, nós geralmente damos um codinome para que fique mais fácil a escrita do código
- Os arrays nos dão uma flexibilidade muito grande e nos permitem criar código sem depender de loops o tempo todo
- Podemos usar o DTYPE para estipular com que tipo de dados estamos trabalhando, para que, se necessário, possamos fazer a conversão.
```python
import numpy as np

arr1 = np.array([1,2,3,4,5])
print(arr1.dtype)
print(arr1)

#[OUT]
#int64
#[1 2 3 4 5]

arr2 = arr1.astype(np.float64)
print(arr2.dtype)
print(arr2)

#[OUT]
#float64
#[1. 2. 3. 4. 5.]
```

- Os arrays são importantes porque permitem que você expresse operações em sequência nos dados sem utilizar nenm loop FOR ou WHILE. Os usuários de NumPy chamam isso de vetorização
- Qualquer operação entre arrays de mesmo tamanho é aplicada de elemento em elemento
- Operações aritméticas com escalares são propagadas para cada elemento da matriz

```python

import numpy as np

arr = np.array([1,2,3],[4,5,6])
print(arr+1)
#[OUT]
#[[2 3 4]
#[ 5 6 7 ]]
```

- É possível também fazer comparações com arrays de mesmas dimensões, que resultará em um array de mesmo tamanho com expressões booleanas de true e false.

```python
import numpy as np
arr1 = np.array([[1, 2, 3], [4, 5, 6]])
arr2 = np.array([[6, 5, 4], [3, 2, 1]])
print(arr1 > arr2)

# [OUT]:
# [[False False False]
# [True True True]]
```

- Podemos usar o também o fatiamento e os índices nas nossas arrays
- No caso de arrays de duas dimensões, os elementos de um índice passam a representar a linha da matriz
- 