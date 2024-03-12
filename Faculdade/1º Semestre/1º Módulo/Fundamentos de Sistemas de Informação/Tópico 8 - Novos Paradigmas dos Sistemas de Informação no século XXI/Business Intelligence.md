#SI #sistemasDeInformação #BI 



# Oque é
---

Business Intelligence ou BI é um conjunto de estratégias e técnicas empregadas pelas empresas com o propósito de analisar dados e melhorar a tomada de decisão baseada em informações concretas. É um termo abrangente que inclui os aplicativos, a infraestrutura, ferramentas e as melhores práticas que permitem o acesso e a análise de informações para melhorar e otimizar decisões e desempenho.


## Para oque serve

O objetivo principal é empoderar e agilizar a tomada de decisão, favorecendo a obtenção de melhores resultados.

Ferramentas de BI absorvem toda a complexidade da coleta e transformação de dados em informação, possibilitando que relatórios e análises preditivas sejam gerados com maior rapidez e profundidade.

## Principais Objetivos

- Permitir o acesso interativo dos dados
- Proporcionar a manipulação desses dados e fornecer aos gestores e analistas de negócio a capacidade de realizar a análise adequada
- Ao analisar os dados, situações e desempenhos históricos e atuais, os tomadores de decisão conseguem valiosos insights que podem servir como base para decisões melhores e mais informadas

## Arquitetura de uma solução de BI

![](img/Pasted%20image%2020240312145557.png)

Temos a origem dos dados a esquerda provenientes de outros sistemas da empresa. Ao lado, temos um repositório de dados muito grande, chamado de Data Warehouse. Em geral, é um banco de dados único, onde os dados ficam amarzenados conforme um modelo que permita análises em diferentes dimensões de negócio, por isso dizemos que os dados em um DW estão num formato "dimensional".

Entre a origem dos dados e o DW temos o processo de coleta, transformação e carregamento dos dados para dentro do DW, esse processo chamado de ETL(Extraction, Transformation and Load) é realizado por ferramentas de software e hardware. Pode ser manual ou automatizado.

![](img/Pasted%20image%2020240312145943.png)

### Outros componentes de uma solução BI

- [[Data Warehouse]]: responsável por armazenar todos os dados após o processo de ETL
- Análise de Negócios: uma coleção de ferramentas para manipular e analisar os dados no data warehouse, incluindo o data mining.
- Business Perfomance Management: utilizado na monitoria e análise do desempenho
- Interface de Usuário: como o dashboard

## Processo de implementação de uma solução de BI

1. <span style="color:#d97f36">Identificar as necessidades</span> a serem endereçadas na solução de BI. Elas devem ser relevantes para objetivos e estratégias do negócio.
2. <span style="color:#d97f36">Identificar as fontes de dados</span> já existentes na organização.
3. <span style="color:#d97f36">Extrair, transformar e carregar os dados</span> para criar uma base multidimensional orientada por assunto.
4. Ajudar a organização a <span style="color:#d97f36">escolher a ferramenta de apresentação</span> para visualizar e analisar as informações resultantes da etapa anterior.
5. <span style="color:#d97f36">Criar relatórios padrões</span>, permitir análises sob demanda e mineração de dados (Data Mining) visando obtenção de insights sobre os indicadores chave de desempenho.
6. <span style="color:#d97f36">Planejar uma implantação de forma abrangente</span> para toda a corporação, de forma a garantir que os tomadores de decisão tenham a informação adequada quando e onde eles precisarem.