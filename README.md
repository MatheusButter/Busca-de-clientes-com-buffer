



Trabalho Prático 2 - Sistema de Gerenciamento de Cliente
Instituto Federal do Espírito Santo Campus Serra
 Bacharelado em Sistemas de Informação
 Técnicas de Programação Avançada
 Prof. Mateus Conrad B. da Costa

 Equipe: Irene Schmidt da Silva Alves
Irlane Schmidt da Silva Alves
Matheus Butter Dias





Descrição do Problema e Equipe
O trabalho consiste na implementação de um sistema para gerenciar o cadastro de clientes de uma empresa global, focando em grandes volumes de dados. As operações principais incluem listar clientes, pesquisar, inserir e remover registros.
Arquitetura da Aplicação com Diagrama de Classes
O sistema utiliza uma interface gráfica baseada em JFrames no estilo do Windows, com manipulação de dados utilizando algoritmos de ordenação externa. Abaixo está o diagrama de classes representando a arquitetura do sistema.

Descrição dos Principais Algoritmos Utilizados
O sistema implementa ordenação externa para lidar com grandes volumes de dados. Esse método divide os dados em blocos menores, ordenados separadamente e combinados posteriormente, otimizando o uso de memória.

A classe Cliente é um modelo de cliente com atributos como nome, sobrenome, endereço, telefone e pontuação de crédito (creditScore). Ela implementa a interface Serializable, permitindo que seus objetos sejam serializados. A classe possui métodos de acesso (getters) e de modificação (setters) para cada atributo, além de validação para o creditScore (deve estar entre 0 e 100). Existe também um método printCliente() que exibe as informações do cliente no console.

A classe GeradorDeArquivosDeClientes é responsável por gerar arquivos binários contendo registros de clientes fictícios, utilizando a biblioteca Faker para criar dados aleatórios. Ela possui métodos que facilitam a criação de arquivos com dados de clientes de forma simples e em grande quantidade.
A classe ArquivoCliente implementa a interface ArquivoSequencial e permite a manipulação de dados de clientes armazenados em arquivos binários, oferecendo métodos simples para abrir, fechar, ler e escrever registros de clientes.



A classe BufferDeClientes implementa a interface Buffer e tem a função de gerenciar um buffer para leitura e escrita de registros de clientes em um arquivo sequencial, otimizando o processo ao lidar com grandes volumes de dados. 

A classe ClienteGUI é uma implementação de uma interface gráfica para gerenciar clientes, ela permite carregar, adicionar, remover, ordenar e buscar clientes em uma tabela visual. Além disso, os clientes podem ser carregados de um arquivo binário, e a interface oferece uma série de funcionalidades para manipulação desses dados.


A classe ClienteGUI2 é uma aplicação gráfica,  que utiliza um BufferDeClientes para carregar registros de clientes de um arquivo de forma otimizada. Essa versão da interface foi projetada para exibir grandes volumes de dados de maneira eficiente,

Imagens das Telas
As imagens a seguir ilustram as principais operações do sistema, incluindo a interface gráfica para listagem, busca, inserção e remoção de clientes.

Figura 02: Representa a tela inicial sem carregar a base de clientes.

Figura 03: Representa a tela principal com a base de clientes carregada. 

Figura 04: Representa a tela de cadastro de um novo cliente. 

Figura 05: Representa a tela de busca de um cliente. 










 
Figura 6: Representa a tela  da ordenação alfabética





Figura 7: Representa a funcionalidade de remover cliente (Remoção dos clientes cujo o nome é Alex)

Figura 8: Representa a tela após a remoção dos clientes

Instruções Detalhadas de Execução
1. Certifique-se de ter o Java instalado.
 2. Clone o repositório do projeto.
 3. Compile o código-fonte utilizando o comando `javac`.
 4. Execute o programa com o comando `java`.
 5. Navegue pelas opções disponíveis na interface gráfica para listar, buscar, inserir ou remover clientes.
Link para o Código-Fonte
O código-fonte documentado e comentado pode ser acessado em: 
