# Esteira de Precificação de transporte turistico

O objetivo deste projeto foi otimizar o processo de precificação de viagens turisticas de uma empresa de transporte e turismo e centralizar todas as cotações dos diversos canais de atendimento em um unico local.


| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | **Esteira de vendas**
| :label: Tecnologias | Google Sheets, java script, html, Power bi
| :rocket: URL         | 
| :fire: Desafio     |

<!-- Inserir imagem com a #vitrinedev ao final do link -->
![image](https://neilpatel.com/wp-content/uploads/2019/12/o-que-e-precificacao.jpeg)
#vitrinedev

## Objetivo do projeto

O intuito do desenvolvimento desta planilha foi Agilizar o processo de cotação, dispensando a utilização do Google Maps para buscar a quilometragem do frete e Centralizar as as solicitações de orçamento em apenas 1 local de forma padronizada com intuito de gerar indicadores e analises que possam contribuir com aumento das vendas.

## Porque o Google Sheets?

Além de ser uma ferramenta do dia dia é de fácil utilização, baixo custo e ideal como para soluções personalizadas, tendo uma grande gama de integrações e automatizações com CRM de vendas e entre outros.

## Detalhes do projeto

**Como é feita a precificação?**

A precificação de um serviço de fretamento é com base no Tipo de veiculo (onibus,micro ou van) + Quilometragem rodada


**Como era o processo?**

O cliente entrava em contato solicitando o serviço de transporte, o atendete coletava informações essenciais para a precificação da viagem, como:

 ***Data e horario de Embarque e Desembarque***  *(Com essas informações o atendente ja verificava o tempo duração do serviço, dia da semana)*

***Ponto de Origem e Destino*** *(Com essas informações o atendete entrava no google maps para levantar a Quilometragem)*

***Tipo de veiculo*** *(onibus,micro ou van)*

Coma as informações de Origem e Destino o atendente acessava o Google Maps coletava a quilometragem e com base no tipo de veiculo o atendente calculava o preço do serviço com auxilo de em uma tabela impressa, inseria as informações em um documento pré formatado, gerava um PDF para enviar ao cliente via Email ou Whatsapp, o mesmo PDF era salvo em um pasta local para questoões de consulta.


**Quais os desafios?**

Custo limitado, Automatizar o processo de levantamento da quilometragem, gerar proposta em PDF de semi automatica.


**Quais as Melhorias o projeto Trouxe?**

Busca automatica da quilometragem entre 3 pontos garagem, origem e destino, Exibição das caracteristicas da viagem (dia da semana, duraçao, quantidade de diarias), precificação automatica da viagem com base no tipo de veiculo, inserçao de campos de valores promocionais ou personalizados, campo com numero de reserva que integra com sistema ERP da empresa, proposta comercial em PDF semi automatica podendo ser enviada da planilha com apenas 1 click, centralização dos dados.

Visando analisar e demonstrar os dados da esteira foram conectados a um Bi, onde se monitora quantidade de cotaões realizadas e fechadas, preço medio da quilometragem vendida, e comparativo Realizado x Orçado.





**Preenchimento automatico da quilometragem**

![km automatico](https://user-images.githubusercontent.com/44843566/197912177-c1baceba-3dfb-4d3a-bffb-75d587640ef0.gif)



**Precificação do Frete**

A precificação do frete leva em consideração a Quilometragem, tipo de veiculo, quantidade de dias alocados, porem o levantamento da quilometragem era o item na qual demandava maior tempo, pois era necessario verificar via Google Maps, os demais itens eram tabelados e agregados ao valor. Por serem valores tabelados onde todos as variações disponiveis estavam previamente precificadas bastando apenas agregar ao valor por quilometro rodado, foi relativamente simples por ser compativel com o Sheets.


**Valores Promocionais**

Valores promocionais tambem foram previamente tabelados e tambem podem ser aplicados durante o processo de precificação na coluna (Cupom Promocional), cabe ao analista durante o processo de precificação avaliar se os criterios de aplicação do cupom se aplicam a viagem. Os valores Personalizados são aplicados caso aja uma negociação fora desse escopo tabelado e os valores da viagem devem ser digitados no campo Valor personalizado.


