
#Python #Programação #IntroduçãoAProgramação 



- Podemos verificar as chaves e os valores dos nossos dicionários usando, respectivamente, os métodos .keys() e .values()
- Podemos combinar 2 dicionários usando o método .update(dicionário a ser combinado)
	- Caso houverem chaves repetidas, o valor da chave será substituído pelo valor do dicionário que foi adicionado por último.
	- Podemos também utilizar o .items para receber tanto as chaves quanto os valores
- Com os métodos .get() e .pop(), nós podemos definir uma mensagem de erro para caso a chave que estamos consultando não exista.
- Podemos usar o método setdefault(chave, []).append(valor) para quando queremos separar elementos de uma lista de acordo com determinado critério.
	- Podemos usar também o defaultdict, importado do collections.
- Embora os valores de um DICT possam ser qualquer objeto Python, as chaves devem ser objetos imutáveis
- 