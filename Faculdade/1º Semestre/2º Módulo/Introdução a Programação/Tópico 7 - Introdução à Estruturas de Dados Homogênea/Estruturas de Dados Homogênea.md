
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
