#Atividade Banco de Dados
```sql
CREATE TABLE Funcionarios (
    ID INT PRIMARY KEY,
    Nome VARCHAR(100),
    Sobrenome VARCHAR(100),
    Salario DECIMAL(10, 2)
);
```
```sql
ALTER TABLE Funcionarios
ADD DataNascimento DATE;
```
```sql
CREATE TABLE Departamentos (
    ID INT PRIMARY KEY,
    Nome VARCHAR(100)
);
```
```sql
ALTER TABLE Funcionarios
ADD IDDepartamento INT;
```
```sql
CREATE TABLE Projetos (
    ID INT PRIMARY KEY,
    NomeProjeto VARCHAR(100)
);
```
```sql
CREATE TABLE Alocacoes (
    ID INT PRIMARY KEY,
    IDFuncionario INT,
    IDProjeto INT
);
```
```sql
ALTER TABLE Funcionarios
RENAME COLUMN Sobrenome TO Apelido;
```
```sql
CREATE TABLE Clientes (
    ID INT PRIMARY KEY,
    NomeCliente VARCHAR(100)
);
```
```sql
ALTER TABLE Projetos
ADD IDCliente INT;
```
```sql
CREATE TABLE Enderecos (
    ID INT PRIMARY KEY,
    Rua VARCHAR(200),
    Cidade VARCHAR(100),
    CEP VARCHAR(10)
);
```
```sql
ALTER TABLE Funcionarios
ADD IDEndereco INT;
```
```sql
ALTER TABLE Clientes
RENAME COLUMN NomeCliente TO NomeEmpresa;
```
```sql
CREATE TABLE Pedidos (
    ID INT PRIMARY KEY,
    DataPedido DATE
);
```
```sql
ALTER TABLE Pedidos
ADD IDCliente INT;
```
```sql
CREATE TABLE ItensPedido (
    ID INT PRIMARY KEY,
    IDPedido INT,
    IDProduto INT
);
```
```sql
CREATE TABLE Produtos (
    ID INT PRIMARY KEY,
    NomeProduto VARCHAR(100),
    QuantidadeProduto INT,
    ValorProduto DECIMAL(10, 2)
);
```
```sql
ALTER TABLE Produtos
RENAME COLUMN NomeProduto TO DescricaoProduto;
```
```sql
CREATE TABLE Estoques (
    ID INT PRIMARY KEY,
    Quantidade INT
);
```
```sql
ALTER TABLE Estoques
ADD IDProduto INT;
```
```sql
CREATE TABLE Vendas (
    ID INT PRIMARY KEY,
    DataVenda DATE
);
```
```sql
ALTER TABLE Vendas
ADD IDCliente INT;
```
