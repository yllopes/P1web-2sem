# Sistema de Gerenciamento de Produtos

## Descrição
Este projeto é um sistema de gerenciamento de produtos que permite cadastrar, atualizar, listar e excluir produtos. Além disso, todas as operações são registradas em uma tabela de logs para rastreamento e auditoria.

## Funcionalidades
- **Gerenciamento de Produtos**
  - Cadastrar novos produtos.
  - Atualizar informações de produtos existentes.
  - Listar todos os produtos ou um produto específico.
  - Excluir produtos do sistema.

- **Registro de Logs**
  - Todas as operações CRUD são registradas com informações detalhadas, como tipo de operação, data e hora, e ID do produto afetado.

## Tecnologias Utilizadas
- **Banco de Dados**: SQLite
- **Framework**: [Nome do Framework utilizado, se aplicável]
- **Documentação da API**: Postman

## Endpoints

### Produtos
- **GET /produtos**
  - Retorna todos os produtos.
  
- **GET /produtos/{id}**
  - Retorna o produto com o ID especificado.
  
- **POST /produtos**
  - Cria um novo produto (com validação de campos).
  
- **PUT /produtos/{id}**
  - Atualiza os dados de um produto existente (com validação de campos).
  
- **DELETE /produtos/{id}**
  - Exclui o produto com o ID especificado.

#### Validações de Produtos
- O nome do produto deve ter no mínimo 3 caracteres.
- O preço deve ser um valor positivo.
- O estoque deve ser um número inteiro maior ou igual a zero.

### Logs
- **GET /logs**
  - Retorna todos os logs das operações realizadas nos produtos.

## Documentação da API
A documentação detalhada da API está disponível no Postman e inclui:
- Descrição dos endpoints.
- Parâmetros de entrada.
- Exemplos de requisições e respostas.
- Códigos de status esperados (200, 400, 404, 500).

## Testes
Todos os endpoints foram testados utilizando o Postman, e as capturas de tela dos testes estão incluídas no documento de entrega.

## Relatório Técnico
Um relatório final foi elaborado, abordando:
- O desenvolvimento da aplicação.
- Implementação dos logs.
- Funcionamento das validações de campos.
- Dificuldades encontradas e soluções adotadas.

## Conclusão
O Sistema de Gerenciamento de Produtos é uma aplicação robusta e eficaz, que garante a integridade dos dados por meio de validações e registros de log, proporcionando uma gestão eficiente dos produtos.
