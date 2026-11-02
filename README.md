# DIO - Trilha .NET: Fundamentos | Sistema de Estacionamento

Este projeto foi desenvolvido durante a trilha .NET da [DIO (Digital Innovation One)](https://www.dio.me/), como parte de um desafio para praticar os conceitos básicos da linguagem C#.

---

## Sobre o projeto

A ideia do desafio foi criar um sistema de estacionamento executado pelo console, permitindo cadastrar veículos, consultar os que estão estacionados e calcular o valor a ser pago na saída.

O sistema possui as seguintes funcionalidades:

1. **Cadastrar veículo:** permite informar a placa de um veículo e adicioná-lo à lista de estacionados.
2. **Remover veículo:** verifica se a placa está cadastrada, solicita o tempo de permanência e calcula o valor a ser pago.
3. **Listar veículos:** mostra todos os veículos que estão no estacionamento no momento.
4. **Encerrar:** finaliza a execução do programa.

O valor cobrado é calculado considerando uma taxa inicial mais o valor por hora de permanência.

---

## Diagrama de Classes

![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

### Classe Estacionamento

A classe `Estacionamento` concentra as principais funcionalidades do sistema.

Ela possui os seguintes atributos e métodos:

- `precoInicial`: valor fixo cobrado pelo estacionamento.
- `precoPorHora`: valor adicional cobrado por hora.
- `veiculos`: lista que armazena as placas dos veículos cadastrados.
- `AdicionarVeiculo()`: recebe a placa informada e adiciona o veículo à lista.
- `RemoverVeiculo()`: calcula o valor da permanência e remove o veículo da lista.
- `ListarVeiculos()`: exibe os veículos que ainda estão estacionados.

---

## Tecnologias utilizadas

- C#
- .NET (Console Application)
- Git e GitHub

---

## Estrutura do projeto

```text
trilha-net-fundamentos-desafio/
├── DesafioFundamentos/
│   ├── Models/
│   │   └── Estacionamento.cs
│   ├── DesafioFundamentos.csproj
│   └── Program.cs
├── diagrama_classe_estacionamento.png
└── README.md
```

---

## Como executar

Para executar o projeto, é necessário ter o [.NET SDK](https://dotnet.microsoft.com/download) instalado (versão 6.0 ou superior).

**1. Clone o repositório:**

```bash
git clone https://github.com/juliasd02/trilha-net-fundamentos-desafio.git
```

**2. Acesse a pasta do projeto:**

```bash
cd trilha-net-fundamentos-desafio/DesafioFundamentos
```

**3. Execute o projeto:**

```bash
dotnet run
```

Após iniciar, basta seguir as instruções exibidas no console, informar os valores do estacionamento e utilizar o menu para cadastrar, remover ou consultar os veículos.
