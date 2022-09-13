# My Finance Web
MyFinance - Projeto do Curso de Pós Graduação em Engenharia de Software da PUC-MG

# Arquitetura

Para desenvolvimento desta aplicação dividimos em três camadas são elas: Acesso aos dados, Engenharia de negócio e camada da Aplicação que seria a parte do MVC.
A Camada Business: Possui a lógica de serviço, as models, views e controlles.

<img src="docs\projetmyfinance.png" alt="estrutura">

# Banco de dados

Para o banco de dados neste projeto foi utilizado o Entity Framework versão 6, não usamos o C# puro e utilizamos métodos assíncronos.
o Entity Framework é uma estrutura ORM de código aberto para aplicativos .NET com suporte da Microsoft. Ele permite que os desenvolvedores trabalhem com dados usando objetos de classes específicas de domínio sem se concentrar nas tabelas e colunas subjacentes do banco de dados onde esses dados são armazenados. Com o Entity Framework, os desenvolvedores podem trabalhar em um nível mais alto de abstração quando lidam com dados e podem criar e manter aplicativos orientados a dados com menos código em comparação com aplicativos tradicionais.

A figura abaixo apresenta onde o Entity Framework se encaixa em uma aplicação:

<img src="docs\Entiity.png" alt="banco">
 
O entity se encaixa entre as entidades de negócios e o banco de dados. Ele salva dados armazenados nas propriedades de entidades de negócios e também recupera dados do banco e os converte em objetos de entidades de negócios automaticamente.

# Chat.Js

Neste projeto, utilizamos o Chart. JS é uma biblioteca em JavaScript que auxilia na criação de gráficos utilizando apenas HTML, CSS e JS para renderizar os gráficos na tela do usuário, utilizamos para criação do projeto o gráfico de pizza referente as transações, ou seja, tudo que foi gasto de credito e debito por período onde é possível que o usuário visualize o total de sua receita e despesas por um período desejado.

 <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.9.1/chart.js"></script>
 
<div> <script>
var chart = null;
    function loadDraft(d, c) {
        if (chart != null) {
            chart.destroy();
        }
        const data = {
            labels: [
                'Débito',
                'Credito'
            ],
            datasets: [{
                label: 'My First Dataset',
                data: [d, c],
                backgroundColor: [
                    'rgb(255, 99, 132)',
                    'rgb(54, 162, 235)'
                ],
                hoverOffset: 4
            }]
        };
        const config = {
            type: 'pie',
            data: data,
        };
       const ctx = document.getElementById('myChart').getContext('2d');
        const myChart = new Chart(ctx, config);
        chart = myChart;
    }
</script> </div>
