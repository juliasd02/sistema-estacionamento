# DIO - Trilha .NET - Fundamentos: Sistema de Estacionamento

Projeto desenvolvido como parte do desafio de código do módulo de Fundamentos da trilha .NET da [DIO (Digital Innovation One)](https://www.dio.me/).

---

## 📌 Contexto e Proposta

O desafio consiste na construção de um sistema de console para gerenciar um estacionamento de veículos, com as seguintes operações:
1. **Cadastrar veículo**: Adicionar a placa do veículo na lista de estacionados.
2. **Remover veículo**: Verificar se o veículo existe, solicitar a quantidade de horas que permaneceu estacionado, calcular o valor cobrado (`precoInicial + precoPorHora * horas`) e remover a placa da lista.
3. **Listar veículos**: Exibir todos os veículos atualmente estacionados ou informar caso não haja nenhum.
4. **Encerrar**: Finalizar a aplicação.

---

## 📐 Diagrama de Classes

![Diagrama de classe estacionamento](diagrama_classe_estacionamento.png)

A classe principal `Estacionamento` possui os seguintes atributos e métodos:
- **`precoInicial`**: Preço fixo cobrado ao estacionar.
- **`precoPorHora`**: Valor cobrado por cada hora de permanência.
- **`veiculos`**: Coleção (`List<string>`) com as placas dos veículos estacionados.
- **`AdicionarVeiculo()`**: Lê a placa do console e adiciona à lista.
- **`RemoverVeiculo()`**: Calcula a estadia, exibe o total e remove o veículo.
- **`ListarVeiculos()`**: Itera sobre a lista exibindo cada veículo cadastrado.

---

## 🛠️ Tecnologias Utilizadas

- **C# / .NET** (Console Application)
- **Git & GitHub** (Controle de versão)

---

## 📂 Estrutura do Projeto

```
trilha-net-fundamentos-desafio/
├── DesafioFundamentos/
│   ├── Models/
│   │   └── Estacionamento.cs       # Lógica do estacionamento (adicionar, remover, listar)
│   ├── DesafioFundamentos.csproj   # Configuração do projeto .NET
│   └── Program.cs                  # Ponto de entrada e menu interativo
├── diagrama_classe_estacionamento.png
└── README.md
```

---

## 🚀 Como Executar

### Pré-requisitos
- [.NET SDK](https://dotnet.microsoft.com/download) instalado (versão 6.0 ou superior).

### Passo a passo

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/juliasd02/trilha-net-fundamentos-desafio.git
   cd trilha-net-fundamentos-desafio/DesafioFundamentos
   ```

2. **Execute o projeto:**
   ```bash
   dotnet run
   ```

3. **Siga as instruções exibidas no console:**
   - Informe o preço inicial e o preço por hora.
   - Utilize o menu numérico para cadastrar, remover e listar veículos.
