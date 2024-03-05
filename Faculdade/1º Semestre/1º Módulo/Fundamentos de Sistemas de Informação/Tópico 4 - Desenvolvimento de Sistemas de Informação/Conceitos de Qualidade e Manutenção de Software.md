---
tags:
  - software
  - sistemasDeInformação
  - SI
  - Programação
  - Engenharia
---
# Avaliando um Software
---

Um software pode ser descrito como bom quando ele é adequado para sua finalidade, a qualidade de um projeto engloba o grau de atendimento às funções e características especificadas no modelo de requisitos.

A qualidade subjetiva de um sistema de software baseia-se em grande parte em suas características não funcionais (tempo de processamento, segurança, facilidade de uso etc.) Isso reflete a experiência prática do usuário.

> Se produzimos um sistema de software de péssima qualidade, perdemos porque ninguém irá querer comprá-lo. Se, por outro lado, gastamos um tempo infinito, um esforço extremamente grande e grandes somas de dinheiro para construir um software absolutamente perfeito, então, isso levará muito tempo para ser completado, e o custo de produção será tão alto que iremos à falência. Ou perdemos a oportunidade de mercado ou então simplesmente esgotamos todos os nossos recursos. Dessa maneira, os profissionais desta área tentam encontrar aquele meio-termo mágico onde o produto é suficientemente bom para não ser rejeitado logo de cara, como, por exemplo, durante uma avaliação, mas também não é o objeto de tamanho perfeccionismo e trabalho que levaria muito tempo ou que custaria demasiadamente para ser finalizado.
> \- Pressman, 2011

O processo de desenvolvimento usado tem uma influência significativa sobre a qualidade de software e bons processos são mais suscetíveis de conduzir o software de boa qualidade

## Modelos de qualidade

Os modelos de qualidade objetivam avaliar o produto de software, segundo diferentes aspectos baseados na visão do usuário.

Para padronizar internacionalmente as características de implementação do software, foram criadas algumas normas, como a [**ISO 9126**](https://medium.com/@nicolasnmg/iso-9126-o-que-%C3%A9-e-por-que-%C3%A9-importante-para-a-qualidade-de-software-33faa81d2cf9), que possui um **conjunto de atributos** que têm impacto na capacidade do software de manter o seu nível de desempenho dentro de condições estabelecidas por um dado período de tempo, como Funcionalidade, Confiabilidade e Usabilidade, e a [**ISO 12119**](https://pt.linkedin.com/pulse/iso-12119-avalia%C3%A7%C3%A3o-de-pacotes-software-dani-cavalcanti) (norma foi publicada em 1994) que trata da **avaliação de pacotes de software**, também conhecidos como “software de prateleira”. Ambas as normas focam na qualidade do produto de software.

## Testes

Outro item importante na busca pela qualidade de software é a realização de testes.

Teste é um conjunto de atividades que podem ser planejadas com antecedência e executadas sistematicamente.

De forma mais objetiva, pensemos nos Testes contendo duas atividades macro, chamadas de **verificação** e **validação (V&V).** Verificação refere-se ao conjunto de tarefas que garantem que o software implementa corretamente uma função específica. Validação refere-se a um conjunto de tarefas que asseguram que o software foi criado e pode ser rastreado segundo os requisitos do cliente.

O teste proporciona o último elemento a partir do qual a qualidade pode ser estimada e, mais pragmaticamente, os erros podem ser descobertos.

## Manutenção

Após as devidas ações voltadas para a qualidade do software, ele passará a operar no ambiente real da empresa. Dizemos que o software estará em **Manutenção**.


>“Poucos sistemas de software são completamente novos, e faz muito mais sentido ver o desenvolvimento e a manutenção como processos contínuos. Em vez de dois processos separados, é mais realista pensar na engenharia de software como um processo evolutivo, no qual o software é constantemente alterado durante seu período de vida em resposta as mudanças de requisitos e as necessidades do cliente. A mudança aumenta os custos de desenvolvimento de software, porque, geralmente, significa que o trabalho deve ser refeito. Isso é chamado retrabalho”.
>\- Summerville, 2011

Duas abordagens que podem ser adotadas para a redução de custos de retrabalho:

1. **Prevenção de mudanças**: O processo de software inclui atividades capazes de antecipar as mudanças possíveis antes que seja necessário qualquer trabalho.
2. **Tolerância a mudanças**: O processo foi projetado para que as mudanças possam ser acomodadas a um custo relativamente baixo, isso normalmente envolve alguma forma de desenvolvimento incremental.