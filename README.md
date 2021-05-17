
<div align="center">
  <img src="https://user-images.githubusercontent.com/61476935/118506970-2bf28b80-b704-11eb-9ff5-2310b0a6b35f.png">
</div>

<br>

<img src="https://img.shields.io/static/v1?label=SQL&message=Language&color=orange&style=for-the-badge&logo=SQL"/>


O SQL, ou Structured Query Language, é uma linguagem de consulta e estruturação declarativa padrão para banco de dados relacionais.
Tendo sido desenvolvida pela IBM nos anos 70, a linguagem SQL é utilizada de maneira relativamente parecida entre os principais bancos
de dados relacionais do mercado: Oracle, MySQL, MariaDB, PostgreSQL, Microsoft SQL Server, entre muitos outros.


<h2>Bancos de Dados Relacionais</h2>


Um banco de dados relacional separa as de informações em classes. Essas classes são formadas a partir de semelhanças entre atributos, ou  seja: mesma tipo, modelo, cargo, etx. A função é agrupar informações do mesmo tipo. Essas classes formam tabelas, que possuem campos(colunas): Representa os atributos dos dados; registros(linhas): Dados de uma entidade única. A relação entre tais tabelas se torna uma informação relevante dentro do banco de dados.


<h2> Funções do SQL </h2>


Um exemplo prático das funcionalidades de uma linguagem de query aplicada a um banco de dados relacional e a administração de dados empresariais. Empresas de diversas proporções utilizam de informação para gerir seus processos, seja uma sturtup ou uma multinacional,
o registro e consulta de infiormações é imprescindível. Os bancos de dados suprem tal necessidade de forma eficiente há banse tempo.
Para ilustrar o uso dessa tecnologia imagine o seguinte processo de administração de dados:

Imagine que uma série de informações sobre novos funcionários seram registradas no banco de dados de uma empresa contrarante. Essas 
infromações consistem em: um identificador individual, o salário e o seto que cada um deles integra. Além disso, a empresa possui vários
setores distintos, cada qual com sua lista de funcionários:


<h3> Setores </h3>


|        NumSetor         |             NomeDepart             |  |        NumSetor         |             NomeDepart             |  
| ----------------------- | ---------------------------------- |  | ----------------------- | ---------------------------------- |  
|           01	          |          Recursos Humanos	       |  |           01	        |          Recursos Humanos	         | 
|           02	          |        Limpeza e Manutenção        |  |           02	        |        Limpeza e Manutenção        | 
|           03	          |      Tecnologia da informação      |  |           03	        |      Tecnologia da informação      | 


<h3> Empregados do Departamento de TI </h3>


|         NumEmp          |      Salário      |      Setor     |
| ----------------------- | ----------------- | -------------- |
|          016            |    R$ 2,520,60    |       03       |  
|          034            |    R$ 3000,00     |       03       |
|          057            |    R$ 4,500,10    |       03       |


A relação entre essas tabelas fica clara graças ao compartilhamento de dados semelhantes. Estes dados representam a relação que as duas tabelas têm, sendo chamado de chave estrangeira. O número que determina o setor de Tecnologia da Informação (03) mostra que ele é mais um de uma lista de setores. Ou seja, caso eu seja necessário  
saber o salário de um determinado funcionário do setor d 03, primeiramente, deve-se acessar a lista de setores da empresa, acessar o setor 03, e em seguida identificar
o empregado através do identificador, nesse caso o número do empregado. Quando surge a necessidade de manipular algum dado de alguma tabela, feze-se uso de uma linguagem de manipulação de bancos de dados relacionais, uma delas é a SQL.

Com isso, pode-se definir algumas das funcionalidades do SQl:

<ul>
  <li>Permitir acesso a dados em um SGBDR, ou Sistema Gerenciador de Banco de Dados Relacionais;</li>
  <li>Permitir manipular e definir dados em um banco de dados;</li>
  <li>Pode ser utilizado em várias outras linguagens por meio de bibliotecas e módulos SQL;</li>
  <li>Permitir criar e deletar: dados, tabelas e os próprios bancos de dados;</li>
  <li>
      Permitir a criação de Stored Procedures, que são técnicas avançadas de controle de dados e envio de resultados por meio da criação de estruturas de repetição, sendo possível criar parâmetros para tais estruturas;
  </li>
  <li>Permitir também o controle de acesso às tabelas e funções de um banco de dados.</li>
</ul>


<h2> SQL Server Management Studio </h2>


O SQL Server Management Studio é um SGBDR, ou Sistema Gerenciador de Bancos de Dados Relacionais, que consiste em uma ferramenta de criação, desenvolvimento e manipulação de bancos de dados. Desenvolvida e mantida pela Microsoft, é usado para configurar, gerenciar e administrar todos os componentes do Microsoft SQL Server,
sendo um dos ambientes que suportão e compilam comandos SQl.

Documentação e Processo de Instalação da versão 2021: https://docs.microsoft.com/pt-br/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15


<h2> Comandos SQL </h2>

