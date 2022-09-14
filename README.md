# My Finance Web
MyFinance - Projeto do Curso de Pós Graduação em Engenharia de Software da PUC-MG

# 💻 Arquitetura

Para desenvolvimento desta aplicação dividimos em três camadas são elas: Acesso aos dados, Engenharia de negócio e camada da Aplicação que seria a parte do MVC.
A Camada Business: Possui a lógica de serviço, Model, View e Controller.

<img src="docs\projetmyfinance.png" alt="estrutura">

# 💻 Banco de dados

Para o banco de dados neste projeto foi utilizado o Entity Framework versão 6, não usamos o C# puro e utilizamos métodos assíncronos.
o Entity Framework é uma estrutura ORM de código aberto para aplicativos .NET com suporte da Microsoft. Ele permite que os desenvolvedores trabalhem com dados usando objetos de classes específicas de domínio sem se concentrar nas tabelas e colunas subjacentes do banco de dados onde esses dados são armazenados. Com o Entity Framework, os desenvolvedores podem trabalhar em um nível mais alto de abstração quando lidam com dados e podem criar e manter aplicativos orientados a dados com menos código em comparação com aplicativos tradicionais.

A figura abaixo apresenta o processo do Entity Framework no qual se encaixa em uma aplicação:

<img src="docs\Entiity.png" alt="banco">
 
O entity se encaixa entre as entidades de negócios e o banco de dados. Ele salva dados armazenados nas propriedades de entidades de negócios e também recupera dados do banco e os converte em objetos de entidades de negócios 
automaticamente.


# Chat.Js

Neste projeto, utilizamos o Chart. JS é uma biblioteca em JavaScript que auxilia na criação de gráficos utilizando apenas HTML, CSS e JS para renderizar os gráficos na tela do usuário, utilizamos para criação do projeto o gráfico de pizza referente as transações, ou seja, tudo que foi gasto de crédito e débito por período, sendo possível que o usuário visualize o total de suas receitas e despesas por um período desejado.

https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.9.1/chart.js

<img src="docs\Codchartjs.PNG" alt="cod">


## ☕ Contribuintes do Projeto<br>

<img src="https://avatars.githubusercontent.com/u/48659873?v=4" width=70> <br> <sub> Luiz David: </sub> https://github.com/LuizDavidOlv|

<img src="https://avatars.githubusercontent.com/u/43283168?v=4" width=70> <br> <sub> Rodrigo Moreira: </sub>https://github.com/Rdsm02|


<img src="https://avatars.githubusercontent.com/u/100494953?v=4" width=70> <br> <sub> Débora Moura: </sub>https://github.com/debora-moura|







