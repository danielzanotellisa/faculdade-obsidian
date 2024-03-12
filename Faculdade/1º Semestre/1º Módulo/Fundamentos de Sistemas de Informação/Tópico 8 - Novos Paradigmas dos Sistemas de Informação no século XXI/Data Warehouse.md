#BI #SI #sistemasDeInformação 


# Oque é
---

Uma data warehouse é um repositório central de informações que podem ser analisadas para tomar decisões mais adequadas. Os dados fluem de sistemas transacionais, bancos de dados relacionais e de outras fontes para o datawarehouse, normalmente com uma cadência regular.

Analistas de negócios, engenheiros de dados, cientistas de dados e tomadores de decisões acessam os dados por meio de ferramentas de BI, clientes SQL e outras aplicações de análise.

Os dados e análises se tornaram indispensáveis no meio corporativo, os usuários contam com relatórios, painéis e análises para extrair valor dos dados, monitorar a performance do negócio e apoiar a tomada de decisões. Os DW são responsáveis por alimentar esses relatórios, análises e ferramentas.

## Características de um DW

1. <span style="color:#d97f36">Orientado a Assunto</span>: um DW está sempre orientado ao redor do principal assunto da organização sobre o qual se deseja realizar análises.
2. <span style="color:#d97f36">Integrado</span>: nesses ambientes, há a coleta de dados em diversas fontes, desde aqueles estruturados até aqueles que não são estruturados. Uma vez coletados, todos esses dados devem ser disponibilizados juntos, em uma única base de dados, de forma integrada.
3. <span style="color:#d97f36">Não volátil</span>: uma vez ocorrido o fato de interesse naquele assunto específico, ele faz parte do histórico, pois reflete uma realidade num dado momento, que não muda mais.
4. <span style="color:#d97f36">Variante no tempo</span>: os fatos associados a determinado assunto ocorrem durante um determinado período.

Um projeto de construção de um DW envolve a seleção de várias tecnologias. Uma arquitetura DW contém alguns elementos importantes que são as **fontes de dados**(Ambiente transacional), a **_Staging Area,_** representando uma “área de transferência” temporária de dados coletados e que, para fins de isolamento de alterações (e mudança em seu entendimento), ficam disponíveis na forma original (arquivos) ou manipulados para que possam ser melhor integrados a uma base integrada, **um banco de dados integrado (_Data Warehouse_)**, que irá armazenar os dados de interesse no assunto (Data Mart) a ser analisado em um formato dimensional (visões de negócio), além de campos quantificadores a respeito de alguma métrica de negócio e, finalmente, um **Ambiente (camada) de apresentação,** correspondendo às ferramentas que irão disponibilizar, de forma dinâmica e interativa, as informações de interesse dos usuários finais, que podem ser na forma de relatórios ad hoc (não padronizados) ou através de dashboards (painéis gráficos) contendo indicadores do negócio.