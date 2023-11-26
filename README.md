# Sistema-de-Gerenciamento-de-Pedidos

# Sistema de Gerenciamento de Clientes e Pedidos

Este conjunto de scripts SQL e stored procedures constitui um sistema simples para gerenciar clientes, pedidos e suas inter-relações em um ambiente de banco de dados relacional.

## Estrutura do Banco de Dados

O banco de dados contém duas tabelas principais:

### Tabela `Clientes`

Armazena informações sobre os clientes.
- `ID_Cliente`: Identificador único do cliente.
- `Nome`: Nome do cliente.
- `Endereco`: Endereço do cliente.
- `Email`: Endereço de e-mail do cliente.
- `Telefone`: Número de telefone do cliente.

### Tabela `Pedidos`

Registra informações sobre os pedidos feitos pelos clientes.
- `ID_Pedido`: Identificador único do pedido.
- `ID_Cliente`: Chave estrangeira referenciando a tabela `Clientes`.
- `Data_Pedido`: Data em que o pedido foi feito.
- `Status_Pedido`: Status atual do pedido.
- `Total`: Valor total do pedido.

## Inserção de Dados de Exemplo

Foram inseridos dados de exemplo nas tabelas `Clientes` e `Pedidos` para demonstrar o funcionamento do sistema.

## Stored Procedures

### Procedure `Inserir_Pedidos`

Permite a inserção de novos pedidos no banco de dados.
- Parâmetros: `p_ID_Cliente` (ID do cliente), `p_Data_Pedido` (Data do pedido), `p_Status_Pedido` (Status do pedido), `p_Total` (Valor total do pedido).

## Trigger

### Trigger `Calcular_Total_Pedidos`

Após a inserção de um novo pedido, atualiza o valor total dos pedidos associados ao cliente na tabela `Clientes`.

## View

### View `Pedidos_Clientes`

Uma view foi criada para mostrar informações sobre pedidos e seus clientes associados.

## Consulta JOIN

Uma consulta JOIN foi realizada para mostrar os clientes que fizeram pedidos no mês atual.

---

Este sistema é um exemplo básico de um sistema de gerenciamento de clientes e pedidos. Pode ser expandido e aprimorado conforme necessário para atender a requisitos específicos do usuário.

![image](https://github.com/SamuelJorgetto/Sistema-de-Gerenciamento-de-Pedidos/assets/144075081/70aababf-feb2-4253-b5dc-0e98c3fd7222)
![image](https://github.com/SamuelJorgetto/Sistema-de-Gerenciamento-de-Pedidos/assets/144075081/25348efd-41cf-4d64-94e2-d36076578807)

