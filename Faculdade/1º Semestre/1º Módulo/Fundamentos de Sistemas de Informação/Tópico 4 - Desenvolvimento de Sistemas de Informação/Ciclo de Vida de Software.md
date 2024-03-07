---
tags:
  - software
  - SI
  - sistemasDeInformação
  - Engenharia
  - Desenvolvimento
---
# O ciclo
---

Chamamos de ciclo de vida de software as fases que ele irá passar desde a sua concepção até a sua extinção. Ao se desenvolver um software, ele irá passar por um ciclo, organizado em etapas as quais estarão organizadas de alguma forma.

![](./img/Pasted%20image%2020240305140939.png)


1. O levantamento das necessidades que identifica as necessidades de informações da organização.
2. A análise de alternativas consiste na identificação e avaliação de sistemas alternativos
3. Projeto trata da construção das especificações detalhadas para o projeto, elas incluem o projeto de interfaces, banco de dados, caraterísticas físicas do sistema, hardware do processamento, o cabeamento e o dispositivo de rede.
4. Desenvolvimento, que inclui o desenvolvimento ou aquisição do software, a provável aquisição do hardware e o teste do novo sistema.
5. Implementação, que ocorro após o sistema ter passado satisfatoriamente por testes de aceitação. O sistema é transferido do ambiente de desenvolvimento para o de produção, caso o sistema antigo ainda exista, ele deve migrar para o novo
6. Manutenção se refere a todas as atividades relacionadas a um sistema depois que ele é implementado

Uma variação dos passos apresentados anteriormente:

- **Comunicação:** a intenção é compreender os objetivos das partes interessadas (gestores, usuário comuns, etc.) para com o projeto e fazer o levantamento das necessidades que ajudarão a definir as funções e características do software;
- **Planejamento:** a atividade de planejamento cria um “mapa” que ajuda a guiar a equipe na sua jornada. O mapa — denominado plano de projeto de software — define o trabalho de engenharia de software, descrevendo as tarefas técnicas a serem conduzidas, os riscos prováveis, os recursos que serão necessários, os produtos resultantes a serem produzidos e um cronograma de trabalho;
- **Modelagem**: cria-se um “esboço” da coisa, de modo que se possa ter uma ideia do todo — qual será o seu aspecto em termos de arquitetura, como as partes constituintes se encaixarão e várias outras características;
- **Construção**: esta atividade combina geração de código (manual ou automatizada) e testes necessários para revelar erros na codificação;
- **Emprego**: o software (como uma entidade completa ou como um incremento parcialmente efetivado) é entregue ao cliente, que avalia o produto entregue e fornece feedback, baseado na avaliação.

Outro conceito muito importante aplicado ao desenvolvimento de software são as [[Linguagens de Programação|linguagens de programação]].

## Alguns outros modelos de desenvolvimento

É muito importante escolher de forma correta um modelo de desenvolvimento que vá se adequar aos recursos e demanda que temos.

Se te temos algo mais simples, estático e com poucos recursos, como por exemplo, algo para um pequeno comércio, podemos utilizar um modelo mais linear. Onde o produto final só será entregue ao término de todas as atividades. [Temos o Modelo Cascata](https://pt.wikipedia.org/wiki/Modelo_em_cascata) como famoso exemplo.

![](./img/Pasted%20image%2020240305143829.png)

Há algumas iterações (refluxos) devido a uma maior possibilidade, em algum momento, dos requisitos de negócio mudarem ou, mesmo ainda, não se encontrarem em um ponto ideal de entendimento. À medida que vão sendo identificados, podem evoluir e, junto com eles, a complexidade do produto final, que será entregue também ao final do desenvolvimento.

![](./img/Pasted%20image%2020240305144046.png)

Temos ainda o fluxo evolutivo, que permite entregarmos parcialmente o produto ao fim do primeiro fluxo.

![](./img/Pasted%20image%2020240305144226.png)

Essa abordagem é interessante pois permite que os usuários convivam com uma solução parcial para que possam validar seus requisitos e entenderem melhor seus objetos e alinhamento com o ambiente de negócios.

Abordagens famosas que usam esse fluxo:
- [SCRUM](https://usemobile.com.br/metodologia-scrum-desenvolvimento/)
- [TDD](https://dev.to/womakerscode/o-que-e-tdd-4b5f#:~:text=TDD%20significa%20Desenvolvimento%20Orientado%20por,do%20XP%20(Extreme%20Programming).)

