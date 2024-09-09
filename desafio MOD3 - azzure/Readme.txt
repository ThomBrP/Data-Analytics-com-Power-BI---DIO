
# Desafio Módulo 3 DIO - Processando e Transformando Dados com Power BI 

Esse é o entregável do módulo 3 do curso de Data Analytics com Power BI via DIO, sob o tema "Processando e Transformando Dados com Power BI".

Este readme tem o objetivo de esclarecer os passos dados em relação ao projeto, além de esclarecer dificuldades e pontuar considerações sobre o projeto.





## Desenvolvimento

Foram utilizados alguns passos para a entrega do projeto. Todos os passos foram anotados em um arquivo .txt e organizados no presente readme

Para início:


- Realização de testes de servidor na Azure;
- Conexão do servidor azure com mysql workbench com sucesso
- Inserção do script "script_bd_company.sql" no workbench, com 1 erro: `Error Code: 1091. Can't DROP 'departament_ibfk_1'; check that column/key exists`
- Comentei a linha em questão e testei novamente, dessa vez com sucesso.
- Realização de testes linha a linha, com a exibição de alguns erros (em especial com os drops), os quais foram corrigidos
- Organização do script SQL utilizando Inteligência Artificial, remodelei o banco de dados e a alimentação do mesmo. O script estará em anexo ao entregável, em outro arquivo.
- Ao tentar realizar a conexão do Power BI com o banco de dados MySQL, eu obtive a mensagem de instalação do conector /NET (o que já havia feito previamente). Eu removi a instalação, reiniciei o Power BI, reinstalei o conector, reiniciei o computador, mas tudo sem sucesso.
- Para contornar o problema, entrei na fonte de dados do ODBC do meu computador e adicionei a conexão com o servidor azure, o que deu um retorno positivo.
- Realizei a conexão do servidor ODBC com Power BI, o que também obtive um retorno positivo. O que possibilitou a realização das transformações de dados.

### No Power Query

Com a conexão ODBC funcionando, o servidor ativo e o banco de dados alimentado, pude finalmente iniciar as transformações de dados utilizando Power Query:

- Alterar alguns nomes de colunas para melhor observação
- Dividir "Adress" da tabela Employee em Número, nome da rua e UF (o que posteriormente concatenei nome da rua e UF para utilizar em um mapa)
- Criar uma nova tabela "employee" e utilizar a mescla com departament para buscar os nomes dos departamentos
- Criar as relações de Emp-Dep, Employee e Departament
- Remoção das colunas desnecessárias na nova tabela
- Mesclagem na tabela Employee para resgatar o nome do supervisor
- Mesclar as colunas relacionadas ao nome para que haja apenas 1 coluna com o nome do colaborador (nome completo)
- Mesclar as colunas relacionadas ao nome do supervisor para que haja apenas 1 coluna com o nome do supervisor
- Mesclagem do nome do departamento com sua localização na tabela dept_locations
- Classificar os colaboradores, a fim de verificar a quantidade de colaborador por gerente.


### Finalização
A partir dessas manipulações, pude fazer um relatório simples para amostragem dos dados.



## Autor

- Thom BrP
[Github](https://github.com/ThomBrP) | 
[LinkedIn](https://www.linkedin.com/in/thomasbrp/)

