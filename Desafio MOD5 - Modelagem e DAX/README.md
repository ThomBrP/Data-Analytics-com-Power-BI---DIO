
# Desafio Módulo 3 DIO - Processando e Transformando Dados com Power BI 

Esse é o entregável do módulo 5 do curso de Data Analytics com Power BI via DIO, sob o tema "Modelando dados com Power BI".

Este readme tem o objetivo de esclarecer os passos dados em relação ao projeto, além de esclarecer dificuldades e pontuar considerações sobre o projeto.





## Desenvolvimento

Foram utilizados alguns passos para a entrega do projeto. Todos os passos foram anotados em um arquivo .txt e organizados no presente readme

Para início:
 - Foi realizado o download da sample financials do Power BI e conectado com uma cópia do projeto "financials sample" entregue anteriormente.
 - Foram seguidos os passos conforme o vídeo de apoio do curso

### Continuação

- Foram realizadas várias mesclas, levando em consideração as colunas relacionadas na tabela f_vendas com as dimensões. Com a finalidade de criar as colunas ID e diminuir o número de colunas na f_vendas. (Foram realizados testes para que tais mesclas fossem feitas utilizando DAX, mas a mescla do Power Query pareceu mais simples e intuitiva)
- Foi criado uma tabela data, contendo todas as datas presentes no relatório, excluídos os valores duplicados.
- Na tabela data, foram inclusos via DAX as colunas `Ano, Mês, Dia, Tri`
- Foram realizadas as conexões no editor das tabelas do Power BI
- Foi alterado nos visuais o link para os atributos da tabela origem para as novas tabelas criadas.
- Foi excluído a tabela original do modelo.


O modelo do Schema está presente no arquivo `.pbix` e em formato `.png` no entregável do projeto.




## Autor

- Thom BrP
[Github](https://github.com/ThomBrP) | 
[LinkedIn](https://www.linkedin.com/in/thomasbrp/)

