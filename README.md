# Desafio DIO: Construindo um Sistema para um Estacionamento com C#

Este repositório contém a solução do desafio proposto no bootcamp **Randstad - Backend com .NET** da [DIO](https://www.dio.me/), onde foi solicitado o desenvolvimento de um sistema para gerenciar um estacionamento utilizando a linguagem **C#**.

## Descrição do Desafio

O desafio consistiu em construir uma aplicação que simula o gerenciamento de um estacionamento, permitindo as seguintes operações:

- **Cadastrar um veículo**: O usuário informa a placa de um veículo, que é armazenada em uma lista de veículos estacionados.
- **Remover um veículo**: O usuário informa a placa do veículo e a quantidade de horas que ele ficou estacionado. O sistema calcula o valor total a ser cobrado com base em um preço inicial e um preço por hora de permanência. Em seguida, o veículo é removido da lista.
- **Listar veículos estacionados**: Exibe todos os veículos que estão atualmente no estacionamento.

## Funcionalidades Implementadas

**Classe Estacionamento**:
   - A classe `Estacionamento` contém as seguintes variáveis:
     - `precoInicial` (decimal): o valor inicial cobrado pelo estacionamento.
     - `precoPorHora` (decimal): o valor cobrado por hora de permanência.
     - `veiculos` (List<string>): uma lista que armazena as placas dos veículos atualmente estacionados.
   
   - **Métodos**:
     - `AdicionarVeiculo()`: Pede ao usuário a placa do veículo e adiciona essa placa à lista de veículos estacionados.
     - `RemoverVeiculo()`: Solicita a placa e a quantidade de horas que o veículo permaneceu no estacionamento. Caso o veículo esteja na lista, calcula o valor total e o remove da lista.
     - `ListarVeiculos()`: Exibe a lista de veículos estacionados no momento. Caso não haja nenhum veículo, informa que o estacionamento está vazio.

 **Menu Interativo**:
   - A aplicação é executada em um loop que apresenta um menu com as seguintes opções:
     1. Cadastrar veículo
     2. Remover veículo
     3. Listar veículos
     4. Encerrar

   O usuário pode interagir com o sistema através dessas opções, permitindo o cadastro, remoção e listagem dos veículos.


