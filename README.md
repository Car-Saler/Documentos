# Documentos
Documentação do projeto

## Objetivos do Projeto
Este projeto consiste no desenvolvimento de um sistema de gestão de estoque e vendas para uma revendedora de carros, que permita o gerenciamento eficiente de um estoque de veículos, desde o cadastro até a venda. Esse sistema oferece uma interface para cadastrar novos carros, listar estes veículos por diferentes filtros, como marca, ano, faixa de preço e quilometragem, registrar vendas. Além disso, ele também exibe informações financeiras, como o lucro obtido em determinada venda, cálculo da comissão do vendedor e um relatório detalhado do que foi obtido nas vendas. Com uma estrutura orientada a objetos em Java, o projeto visa a otimização dos processos internos, facilitando a tomada de decisões e aumentando a visibilidade sobre o desempenho das vendas e do estoque disponível.

## Definições, Acrônimos e Abreviações
•	Valor de Compra - Preço pelo qual o veículo foi adquirido pela revendedora

•	Valor de Venda - Preço pelo qual o carro é vendido ao cliente final, registrado na transação de venda.

•	Comissão do Vendedor - Percentual sobre o lucro da venda pago ao vendedor. O valor deve ser inserido a cada venda por se tratar de algo que pode variar conforme cada caso

•	Quilometragem - Total de quilômetros rodados pelo veículo, servindo para filtrar veículos mais usados de veículos mais novos ou veículos 0km.

## Requisitos e Histórias de Usuário

### Requisitos Funcionais

1.	Cadastro de Carros

O sistema deve permitir que o usuário cadastre novos carros no estoque, registrando informações como marca, modelo, ano, país de origem, cor, valor de compra e quilometragem.

2.	Consulta de Carros Disponíveis

O sistema deve possibilitar ao usuário listar todos os carros disponíveis para venda, ou filtrar veículos por atributos como marca, ano, faixa de preço ou quilometragem.

3.	Exclusão de Carros

O usuário deve poder excluir carros do estoque, desde que não tenham sido vendidos, assegurando o controle e a organização do inventário.

4.	Realização de Venda

O sistema deve permitir que o usuário registre a venda de um carro, com informações do valor de venda, comissão do vendedor, e o cálculo automático do lucro da transação.

5.	Exibição de Resultados Financeiros

O sistema deve gerar relatórios financeiros que mostrem o lucro total, a comissão total paga aos vendedores, e a média de lucro por carro vendido.


### Requisitos Não Funcionais

1.	Usabilidade

A interface do sistema deve ser intuitiva e de fácil navegação, permitindo que o usuário acesse as funcionalidades básicas (cadastro, consulta, exclusão e venda de carros) com eficiência.


2.	Desempenho

O sistema deve ser capaz de responder rapidamente às operações de consulta, venda e exibição de relatórios, independentemente do número de carros cadastrados.

## Diagramas UML

### Diagrama de Casos de Uso

#### ID    -    Caso de Uso    -    Descrição do Objetivo do Caso de Uso

UC1    -    Cadastrar Carro    -    Permite ao usuário cadastrar novos carros com detalhes como marca, modelo, e valor de compra.

UC2    -    Listar Carros    -    Permite ao usuário visualizar todos os carros disponíveis no estoque.

UC3    -    Filtrar Carros    -    Permite ao usuário filtrar carros por atributos como marca, ano, faixa de preço ou quilometragem.

UC4    -    Realizar Venda    -    Permite ao usuário registrar a venda de um carro, calculando lucro e comissão do vendedor.

UC5    -    Excluir Carro    -    Permite ao usuário excluir carros que ainda não foram vendidos.

UC6    -    Exibir Resultados    -    Financeiros	Exibe ao usuário relatórios com o lucro total, comissões e média de lucro por venda.

## Diagrama de Classes

Este diagrama de classes representa a estrutura do código, com as principais classes e associações.
•	Carro: Representa os veículos no estoque com atributos como marca, modelo, ano, paisOrigem, cor, valorCompra, e quilometragem.

•	Venda: Representa uma transação de venda, contendo referências ao Carro vendido, o valorVenda, a comissaoVendedor, e o nome do vendedor.

•	Revendedora: Classe Singleton que centraliza a operação da revendedora, incluindo listas de carrosDisponiveis e carrosVendidos, métodos para gerenciamento de estoque, vendas e exibição de relatórios.

## Estrutura das Classes e Relações:

•	Revendedora possui uma associação com Carro (1..) e Venda (1..), pois gerencia um estoque de carros e um histórico de vendas.

•	Venda possui uma associação com Carro (1..1), indicando que cada venda está associada a um único carro.
Essa estrutura organiza as operações e facilita a implementação dos casos de uso descritos.

## Tecnologias Utilizadas

•	Linguagem de Programação:

-	Java - O sistema de gerenciamento de estoque e vendas foi desenvolvido inteiramente em Java, aproveitando sua robustez para operações de back-end e sua orientação a objetos para organizar as classes e métodos.

•	Framework/Biblioteca:

-	JUnit - Utilizado para testes unitários das classes Revendedora, Carro, e Venda, garantindo que o sistema funcione corretamente e que os cálculos de lucro e comissão estejam precisos.

-	Java Collections Framework - Para manipulação de listas e estruturas de dados, como ArrayList, que armazenam os carros disponíveis e as vendas realizadas.

•	Outras Tecnologias:

-	Git - Utilizado para gerenciar o projeto.

-	IntelliJ IDEA - Um ambiente de desenvolvimento integrado, útil para facilitar o desenvolvimento e a depuração do código.

## Instruções de Instalação

https://github.com/Car-Saler/Estoque-de-Carros

