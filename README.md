# 🏨 Sistema de Gerenciamento de Hotel

Este projeto é um sistema de gerenciamento de hotel escrito em C. Ele permite o cadastro e gerenciamento de clientes, funcionários, quartos e estadias, incluindo a finalização de estadias e pesquisas por clientes e funcionários.

## 🚀 Funcionalidades

- **Cadastrar Cliente**: Registra novos clientes no sistema.
- **Cadastrar Funcionário**: Adiciona novos funcionários ao hotel.
- **Cadastrar Quarto**: Insere novos quartos disponíveis para reserva.
- **Cadastrar Estadia**: Cria novas estadias associadas a clientes e quartos específicos.
- **Finalizar Estadia**: Marca estadias como finalizadas e libera os quartos ocupados.
- **Pesquisar Cliente**: Busca clientes pelo código ou nome.
- **Pesquisar Funcionário**: Pesquisa funcionários pelo código ou nome.
- **Mostrar Estadias de um Cliente**: Exibe todas as estadias de um cliente específico.

## 📂 Estruturas de Dados

O sistema utiliza quatro estruturas principais:

1. **Cliente**: Armazena informações sobre os clientes, incluindo código, nome, endereço e telefone.
2. **Funcionário**: Guarda dados sobre os funcionários, como código, nome, telefone, cargo e salário.
3. **Estadia**: Mantém detalhes das estadias, incluindo código do cliente, número do quarto, datas de entrada e saída, quantidade de diárias, valor total e status da estadia.
4. **Quarto**: Registra informações dos quartos, como número, quantidade de hóspedes, valor da diária e status (ocupado ou desocupado).

## 💾 Persistência de Dados

Os dados são salvos em arquivos de texto para garantir a persistência das informações:

- **clientes.txt**: Armazena dados dos clientes.
- **funcionarios.txt**: Contém informações dos funcionários.
- **estadias.txt**: Guarda detalhes das estadias.
- **quartos.txt**: Registra dados dos quartos.

## 🛠️ Funções Principais

### Funções de Cadastro

- `cadastrarCliente()`: Cadastra um novo cliente.
- `cadastrarFuncionario()`: Adiciona um novo funcionário.
- `cadastrarQuarto()`: Insere um novo quarto.
- `cadastrarEstadia()`: Cria uma nova estadia, verificando disponibilidade e sobreposição de datas.

### Funções de Salvamento

- `salvarClientes()`: Salva os dados dos clientes no arquivo.
- `salvarFuncionarios()`: Guarda os dados dos funcionários no arquivo.
- `salvarEstadias()`: Armazena as informações das estadias no arquivo.
- `salvarQuartos()`: Registra os dados dos quartos no arquivo.

### Funções de Carregamento

- `carregarClientes()`: Carrega os dados dos clientes a partir do arquivo.
- `carregarFuncionarios()`: Lê as informações dos funcionários do arquivo.
- `carregarEstadias()`: Carrega os dados das estadias do arquivo.
- `carregarQuartos()`: Lê os dados dos quartos a partir do arquivo.

### Outras Funções

- `finalizarEstadia()`: Finaliza uma estadia ativa e atualiza o status do quarto.
- `pesquisarCliente()`: Pesquisa um cliente pelo código ou nome.
- `pesquisarFuncionario()`: Busca um funcionário pelo código ou nome.
- `mostrarEstadiasCliente()`: Exibe todas as estadias de um cliente específico.

## 🚀 Execução

Para compilar e executar o sistema, utilize os comandos abaixo:

```sh
gcc -o hotel hotel.c
./hotel
