
<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/118687223-274cd680-b7db-11eb-9ced-de5605e25940.png">
</div>

<br>

<img src="https://img.shields.io/static/v1?label=SQL&message=Language&color=orange&style=for-the-badge&logo=SQL"/>


O SQL, ou Structured Query Language, é uma linguagem de consulta e estruturação declarativa padrão para banco de dados relacionais.
Tendo sido desenvolvida pela IBM nos anos 70, a linguagem SQL é utilizada de maneira relativamente parecida entre os principais bancos
de dados relacionais do mercado: Oracle, MySQL, MariaDB, PostgreSQL, Microsoft SQL Server, entre muitos outros.


<h2>Bancos de Dados Relacionais</h2>


Um banco de dados relacional separa as informações em classes. Essas classes são formadas a partir de semelhanças entre atributos, ou  seja: mesma tipo, modelo, cargo, etc. A função é agrupar informações do mesmo tipo. Essas classes formam tabelas, que possuem campos(colunas): Representa os atributos dos dados; registros(linhas): Dados de uma entidade única. A relação entre tais tabelas se torna uma informação relevante dentro do banco de dados.


<h2> Funções do SQL </h2>


Um exemplo prático das funcionalidades de uma linguagem de query aplicada a um banco de dados relacional é a administração de dados empresariais. Empresas de diversas proporções utilizam de informação para gerir seus processos, seja uma sturtup ou uma multinacional, o registro e consulta de infiormações é imprescindível. Os bancos de dados suprem tal necessidade de forma eficiente há banstante tempo.

Com isso, pode-se definir algumas das funcionalidades do SQl:


  - Permitir acesso a dados em um SGBDR, ou Sistema Gerenciador de Banco de Dados Relacionais;
  - Permitir manipular e definir dados em um banco de dados;
  - Pode ser utilizado em várias outras linguagens por meio de bibliotecas e módulos SQL;
  - Permitir criar e deletar: dados, tabelas e os próprios bancos de dados;
  - Permitir a criação de Stored Procedures, que são técnicas avançadas de controle de dados e envio de resultados por meio da criação de estruturas de repetição,
    sendo possível criar parâmetros para tais estruturas;
  - Permitir também o controle de acesso às tabelas e funções de um banco de dados.

<br>

<div align="center">
  <h1> Elementos de Banco de Dados </h1>
</div>

<br>

<h2> Tabelas </h2>


Estruturas destinadas ao armazenamento de dados, compostas de um número limitado de colunas (Campos) e um número ilimitado de linhas (Registros ou Tuplas).


<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/118540858-69b4db80-b727-11eb-9387-6b587a579455.png">
</div>


<h2> Chaves </h2>


Campos, ou conjunto de campos, têm o objetivo de identificar unicamente um registro e ou estabelecer relações entre registros.


<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/118540943-8224f600-b727-11eb-9250-eca534b61f19.png">
</div>


<h2> Chaves Candidatas ou Alternativas </h2>


Campos, ou conjunto de campos, que podem identificar unicamente um registro.


<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/118541020-9a951080-b727-11eb-9396-ee5489fac8bd.png">
</div>


<h2> Chaves Primárias( PRIMARY KEY )</h2>


Chaves candidatas escolhidas como identificadoras de registros em suas tabelas.


<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/118541101-b6001b80-b727-11eb-83ae-6a44202875ad.png">
</div>


- Identifica de forma única cada registro em uma tabela de banco de dados;
- Chaves primárias devem conter valores únicos;
- Uma coluna de chave primária não pode conter valores Null; 
- Cada tabela deve conter apenas uma chave primária, mas uma chave primária pode ser uma chave estrangeira em outra tabela.



<h2> Chaves Estrangeiras( FOREIGN KEY ) </h2>


Campo, ou conjunto de campos, de uma tabela que se liga a chave primaria de uma tabela relacionada.


<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/118550749-70495000-b733-11eb-82e5-8acd98ac0f47.png">
</div>


- Uma Foreign Key sinaliza um relacionamento entre tabelas;
- A Foreign Key é a chave primária de uma tabela dentro da tabela com a qual ela se relaciona.
- Uma Foreign Key pode ser definida como Null; 


<h1> Tipos de Dados </h1>


Por se tratar de uma linguagem voltada exclusivamente para o tratamento e controle de informações em bancos de dados, é notável a diversidade de tipos de dados com que o SQL trabalha. Informações contidas nos bancos podem variar e possuir inúmeros caracteres. Um CPF por exemplo possui 11 dígitos, um nome pode possuir uma quantidade muito maior de caracteres, já o gênero do usuário pode ser representado por uma única letra. Números, sejam decimais ou inteiros; valores, datas, letras, nomes, gêneros, id, endereço, formação, instituição de ensino e mesmo a cor de um veículo podem ser dados presentes em algum banco de dados. A manipulação destas informações ocorre de formas diferentes de acordo com o tipo de dado em questão. Logo, é importante entender quais são os tipos de dados e como podem ser manipulados, usando os tipos de comandos anteriormente vistos.


<h2> String </h2>


Char - Cadeia de caracteres de valor fixo.

VarChar - Cadeia de caracteres de valor variável. 

Text - Número variável de caracteres de Texto.

nChar - Cadeia de caracteres de valor fixo com espaço em branco.

nVarChar - Cadeia de caracteres de valor variável com espaço em branco.

Image - Tamanho variável.


<h2>Numéricos</h2>


Bit - Número inteiro, podendo ser 0, 1 ou NULL.

Tinyint - Número inteiros de 0 a 255.

Decimal - Cadeia de valores decimais.

Integer - Números inteiros exatos.

Money - Cadeia de valores monetários. 


<h2>Data</h2>


DateTime - De 1 de Janeiro de 1753 a 31 de Dezembro de 9999.

DateTime2 - De 1 de Janeiro de 0001 a 31 de Dezembro de 9999.

Time - Armazena tempo.


<h1> Comandos SQL </h1>


Por possuir funções que abrangem um grande número de possibilidades, os comandos em SQL também possuem especificações quanto ao tipo de dado manipulado e as ações que serão realizadas. Eles são:


<h2> DDL - Data Definition Language </h2>


Possui a função de criar e estruturar os dados e objetos dentro de uma tabela, podendo incluir, alterar e excluir objetos:

<strong>CREATE</strong> - Cria novos objetos e tabelas dentro do banco de dados e define novas entidades;

<strong>DROP</strong> - Exclui entidades e tabelas inteiras de um banco de dados;

<strong>ALTER</strong>  - Modifica objetos e tabelas existentes, podendo inserir ou excluir colunas, linhas e novos dados nas mesmas.


<h2> DML - Data Manipulation Language  </h2>


Por definição, manipula os dados presentes dentro das tabelas e do banco de dados em si, podendo incluir, alterar e mesmo excluir:

<strong>SELECT</strong> - Permite selecionar e recuperar linhas e colunas das tabelas e do banco de dados respectivamente;

<strong>INSERT</strong> - Insere dados em uma ou mais tabelas;

<strong>UPDATE</strong> - Atualiza dados e funções nas tabelas do banco de dados;

<strong>DELETE</strong> - Utilizado para excluir dados de uma ou mais tabelas.


<h2> DCL - Data Control Language  </h2>


Tem a função de controlar o acesso e gerenciar permissões em um banco de dados. Podendo exercer a função de limitador de ações realizadas pelo usuário dentro do banco de dados:

<strong>GRANT</strong>  - Dá ao usuário o privilégios de acesso a informações e objetos contidos no banco de dados;

<strong>REMOKE</strong>  - Anula as funções e privilégios de informações dados ao usuário pela função Grant; 

<strong>DENY</strong>  - Restringe o acesso a determinada informação ou objeto impedindo que o usuário tenha uma permissão ou privilégio específicos. 


<h2> DQL - Data Query Language  </h2>


Permite a realização de consultas ao banco de dados, permitindo acesso a informações específicas presentes nas tabelas:

<strong>SELECT</strong> - Permite a obtenção de registros específicos em diferente tabelas. 


<h2> DTL - Data Transition Language  </h2>


Se refere aos comandos de gerenciamento de transações em bancos de dados, podendo iniciar, confirmar ou desfazer uma transação:


<strong>BEGIN TRAN(ou TRANSITION)</strong> - É o marcador do início de uma transação no banco, e a mesma pode ou não ser finalizada;

<strong>COMMIT</strong> - Responsável por enviar todos os dados contidos na transação, permanentemente, para o banco de dados;

<strong>ROLLBACK</strong> - Tem a função de desfazer as alterações decorrentes da transação.



<div align="center">
  <h1> Estudando Comandos </h1>
</div>


<h2> Comandos DDL </h2>

    --Cria banco de dados 

    CREATE DATABASE  meu_banco 

<br>

    --Acessa banco de dados     
    
    USE  meu_banco  

<br>

    --Altera nome do banco dedados 

    ALTER DATABASE  meu_banco  MODIFY NAME  =  meu_novo_banco  

<br>

    --Cria tabela e define seus campos

    CREATE TABLE  tabela1  ( <campo1> <tipo> [NOT NULL] ,
                             <campo2> <tipo> [NOT NULL] ,
                             [PRIMARY KEY (campo1,campo2,...),
                             [FOREIGN KEY (campo) REFERENCES tabela2 );

<br>

    --Adiciona um novo campo a tabela  

    ALTER TABLE  tabela1  ADD  <campo1>  <tipo>  [NOT NULL] 

<br>

    --Redefine tipo da coluna

    ALTER TABLE  tabela1  ALTER COLUMN  <campo1>  <tipo>

<br>
    
    --Apaga coluna especificada  
      	  
    ALTER TABLE  tabela1  DROP COLUMN  <nome>

<br>
    
    --Apaga tabela especificada    
    		           
    DROP TABLE  tabela1                                                      


<h2> Comandos DML </h2>


    --Insere dados na tablea  

    INSERT INTO  <Tabela>
  
            (Campo_A1, Campo_A2, Campo_An)
            (Campo_B1, Campo_B2, Campo_Bn)

    VALUES  (Valor_1, Valor_2, Valor_n)

<br>

    --Atualiza tabela de acordo com o parâmetro especificado 

    UPDATE  <tabela>
    SET  <campo>  =  <expressão>
    WHERE  <condição>

<br>

    --Deleta elemento de acordo com o parâmetro especificado 

    DELETE FROM  <tabela>
    WHERE  <condição>


<h2> Comandos DQL </h2>

    --Define método de consulta às tabelas criadas

    SELECT <[tipo] [campos]> FROM <tabela/view> [<condição/ordem>];

- [tipo] - parâmetro opcional que determina o tipo de registro (DISTINCT ou *)
- [campos] - colunas da consulta
- tabela - Nome das tabela a ser consultada
- condição - Permite o estabelecimento dos critérios a seguir:
- WHERE - Permite criar condições para filtrar dados utilizando operadores dos tipos:

- Relacionais - (<, <=, >, >=. =, <>);
- Lógicos - ([NOT] IN, [NOT] BETWEEN, [NOT] LIKE <%dado%>):

- GROUP BY - Agrupa dados em uma consulta.
- HAVING - Limita o resultado de uma consulta agrupada com GROUP BY.
- ORDER BY - Especifica a coluna ou as colunas que serão ordenadas na consulta e a forma de ordenação(ascendente <ASC> ou descendente <DESC>).


<h2> Consultando Dados </h2>

    --Seleciona todas as colunas * de uma tabela

    SELECT  *  FROM  <Tabela>;
    
    --Seleciona os dados da coluna1 de uma tabela, sem repetição

    SELECT  DISTINCT  Coluna1
    FROM  <Tabela>;
    
    --Selecionando os dados da colunas específicas de uma tabela

    SELECT  <Coluna1, Coluna2>
    FROM  <Tabela>;
    
    --Selecionando e nomeando colunas de uma tabela

    SELECT  <Coluna1 AS Nome1, Coluna2 AS Nome2>
    FROM  <Tabela>;


<h2> Comandos DQL - Álgebra Relacional </h2>


A álgebra relacional é uma forma de cálculo sobre conjuntos ou relações. Proposta por E.F Codd como uma base para linguagens de consulta em banco de dados no anos 70.   


<h2> Seleção (σ)</h2>

   <div align="center">
     <img src="https://user-images.githubusercontent.com/61476935/118683819-0fc01e80-b7d8-11eb-8261-78944004a579.png">
   </div>

Indicada pela letra grega sigma (σ) a operação visa a obtenção de dados que satisfaçam determinada condição ou predicado. Sendo predicado a condição que será aplicada a seleção, e sendo a relação a relação ou tabela de onde serão obtidos os dados. Exemplo:


    SELECT * FROM Agenda WHERE Sexo = 'F';


<h2> Projeção (π)</h2>


   <div align="center">
     <img src="https://user-images.githubusercontent.com/61476935/118683920-28303900-b7d8-11eb-9863-f45a3f27b240.png">
   </div>

É uma operação indicada pela letra grega pi (π) que visa a obtenção de dados referentes a mais de uma colunas de uma relação. Sendo coluna1, coluna2 as colunas a serem mostradas, e relação a relação ou tabela de onde serão obtidos os dados. Exemplo:


    SELECT Matricula, Nome FROM Agenda;


<h2> Seleção (σ) e Projeção (π) </h2>


   <div align="center">
     <img src="https://user-images.githubusercontent.com/61476935/118684011-3aaa7280-b7d8-11eb-8b51-b699785b4118.png">
   </div>

Selecione todos os dados das colunas Matricula e Nome na tabela Agenda, apenas dos empregados que possuem sexo = 'F':

    SELECT Matricula, Nome FROM Agenda WHERE sexo = 'F';


<h2> Ordenação (τ) </h2>


   <div align="center">
     <img src="https://user-images.githubusercontent.com/61476935/118684095-501f9c80-b7d8-11eb-9ad1-cba6d8c26ba2.png">
   </div>

É uma operação indicada pela letra grega tau (τ) que visa a ordenação dos dados consultados em uma relação. Sendo coluna – coluna a ser classificada, ord a ordem de classificação -> asc (Ascendente), desc (Descendente) e relação a relação ou tabela de onde serão obtidos os dados. Exemplo:

   <div align="center">
     <img src="https://user-images.githubusercontent.com/61476935/118684267-73e2e280-b7d8-11eb-8f47-f475f234227b.png">
   </div>

Selecione todos os dados referentes as colunas Matricula e Nome, da tabela Agenda, ordenando a coluna nome na ascendente.

    SELECT Matricula, Nome FROM Agenda ORDER BY Nome ASC;


<h2> Comandos DQL - Cláusula WHERE </h2>


Tem a função de estabelecer um predicado, condição para filtrar dados através da utilização de operadores lógicos, em uma consulta SQL.

    SELECT * FROM Tabela WHERE condição;


<h2> Comandos DQL - Cláusula WHERE ( Operadores Relacionais ) </h2>


|      O.R.     |     CONSULTA EM ÁLGEBRA RELACIONAL    |                   CONSULTA SQL                 |
| ------------- | ------------------------------------- | ---------------------------------------------- |
| <             |  σsalario < 2000 ( Agenda )           |   SELECT * FROM Agenda WHERE salario < 2000;   |
| <=            |  σsalario <= 2000 ( Agenda )          |   SELECT * FROM Agenda WHERE salario <= 2000;  |
| >             |  σsalario > 2000 ( Agenda )           |   SELECT * FROM Agenda WHERE salario > 2000;   |
| >=            |  σsalario >= 2000 ( Agenda )          |   SELECT * FROM Agenda WHERE salario >= 2000;  |
| =             |  σsalario = 2000 ( Agenda )           |   SELECT * FROM Agenda WHERE salario = 2000;   |
| <>            |  σsalario <> 2000 ( Agenda )          |   SELECT * FROM Agenda WHERE salario <> 2000;  |


<h2> Comandos DQL - Cláusula WHERE ( Operadores Lógicos ) </h2>


|      O.R.     |        CONSULTA EM ÁLGEBRA RELACIONAL       |                       CONSULTA SQL
| ------------- | ------------------------------------------- | ---------------------------------------------------------- |
| IN            |  σ matricula IN (1,3,5,7) ( Agenda )        |  SELECT * FROM Agenda WHERE matricula IN (1,3,5,7);        |
| BETWEEN       |  σsalario BETWEEN 1500 AND 2000 ( Agenda )  |  SELECT * FROM Agenda WHERE salario BETWEEN 1500 AND 2000; | 
| LIKE ( %, _ ) |  σ nome LIKE '%silva%' ( Agenda )           |  SELECT * FROM Agenda WHERE nome LIKE ‘%silva%';           |
| IS NULL       |  σsalario IS NULL ( Agenda )                |  SELECT * FROM Agenda WHERE salario IS NULL;               |
| NOT or I=     |                                 Nega o predicado nas consultas.                                          |



<h2> Comandos DQL - Cláusula WHERE </h2>


Tem a função de agrupar dados semelhantes em uma consulta SQL

    SELECT * FROM Tabela GROUP BY coluna

    Conte a quantidade de pessoas cadastradas, por sexo, na tabela Agenda:
    
    SELECT Sexo, Count(*) AS 'Qtd.'
    FROM Agenda
    GROUP BY Sexo;

<h2> Comandos DQL - Cláusula GROUP BY </h2>


<h2> Comandos DQL - Cláusula HAVING </h2>


<h2> Comandos DQL - Cláusula ORDER BY </h2>


<h2> Comandos DQL - Cláusula TOP </h2>


<h2> Restrição de Domínio </h2>


<h2> SQL Server Management Studio </h2>


O SQL Server Management Studio é um SGBDR, ou Sistema Gerenciador de Bancos de Dados Relacionais, que consiste em uma ferramenta de criação, desenvolvimento e manipulação de bancos de dados. Desenvolvida e mantida pela Microsoft, é usada para configurar, gerenciar e administrar todos os componentes do Microsoft SQL Server,
sendo um dos ambientes que suportão e compilam comandos SQl.

Documentação e processo de instalação da versão 2021: [https://docs.microsoft.com](https://docs.microsoft.com/pt-br/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15)