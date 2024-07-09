# HotelEmC
## Descrição do Código
Este projeto em C implementa um sistema de gerenciamento de hotel, permitindo o cadastro e a manipulação de dados de clientes, funcionários, quartos e estadias. As principais funcionalidades incluem:

###Cadastro de Clientes: Permite adicionar novos clientes, armazenando informações como nome, endereço e telefone. Os dados são salvos em um arquivo chamado clientes.txt.
###Cadastro de Funcionários: Permite adicionar novos funcionários, armazenando informações como nome, telefone, cargo e salário. Os dados são salvos em um arquivo chamado funcionarios.txt.
###Cadastro de Quartos: Permite adicionar novos quartos, armazenando informações como número, quantidade de hóspedes, valor da diária e status (ocupado ou desocupado). Os dados são salvos em um arquivo chamado quartos.txt.
###Cadastro de Estadias: Permite adicionar novas estadias, verificando a disponibilidade de quartos e calculando o valor total com base na quantidade de diárias. Os dados são salvos em um arquivo chamado estadias.txt.
###Finalização de Estadias: Permite finalizar uma estadia, atualizando o status do quarto para desocupado e calculando o valor total a ser pago pelo cliente.
###Pesquisa de Clientes: Permite pesquisar clientes pelo código ou nome, exibindo as informações encontradas.
###Pesquisa de Funcionários: Permite pesquisar funcionários pelo código ou nome, exibindo as informações encontradas.
###Mostrar Estadias de um Cliente: Exibe todas as estadias registradas para um determinado cliente.
Estruturas de Dados
###Cliente: Armazena código, nome, endereço e telefone.
###Funcionario: Armazena código, nome, telefone, cargo e salário.
###Estadia: Armazena código, código do cliente, número do quarto, data de entrada, data de saída, quantidade de diárias, valor total e status (ativa ou finalizada).
###Quarto: Armazena código, número do quarto, quantidade de hóspedes, valor da diária e status (ocupado ou desocupado).
Arquivos de Dados
Os dados são persistidos em arquivos de texto separados para clientes, funcionários, quartos e estadias:

clientes.txt
funcionarios.txt
quartos.txt
estadias.txt
##Funções Principais
####Salvar Dados: Funções para salvar dados de clientes, funcionários, quartos e estadias nos arquivos correspondentes.
###Carregar Dados: Funções para carregar dados de clientes, funcionários, quartos e estadias dos arquivos correspondentes.
###Cadastro: Funções para cadastrar novos clientes, funcionários, quartos e estadias.
###Pesquisa: Funções para pesquisar clientes e funcionários.
###Finalização de Estadia: Função para finalizar estadias e atualizar o status dos quartos.
##Menu Principal
O sistema apresenta um menu interativo para o usuário, permitindo acessar as principais funcionalidades através de opções numéricas:

Cadastrar cliente
Cadastrar funcionário
Cadastrar quarto
Cadastrar estadia
Finalizar estadia
Pesquisar cliente
Pesquisar funcionário
Mostrar estadias de um cliente
Sair
O código principal (main) carrega os dados dos arquivos, exibe o menu e processa as escolhas do usuário em um loop contínuo até que a opção de sair seja selecionada.
