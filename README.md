# Diagrama de Entidade-Relação Melhorado • e-Commerce

Criando um Diagrama EER de um sistema de e-commerce. Foi especificado as instâncias, priorizando as entidades principais e desenvolvendo os relaciomantos a partir disso.

## Desafio Modelagem de Dados • DIO

Refine o modelo apresentado acrescentando os seguintes pontos:

- Cliente PJ e PF – Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;
- Pagamento – Pode ter cadastrado mais de uma forma de pagamento;
- Entrega – Possui status e código de rastreio.

## Ferramenta

Foi utilizado o designer de diagramas do Workbench MySQL.

O MySQL Workbench é uma ferramenta gráfica versátil para arquitetos de banco de dados, desenvolvedores e administradores de banco de dados.

![worbench](https://github.com/devcaiada/ecommerce-db-EER/blob/main/assets/mysql_workbench.jpg?raw=true)

## Resultado final

Após a modelagem inicial com a instrutura, foram definidas três etapas para o desafio: inclusão de clientes PJ e PF, gerenciamento de pagamentos e controle de entregas. A seguir, apresento o resultado obtido:

1. **Clientes PJ e PF**:
   Na tabela de clientes, incluímos duas tabelas específicas para pessoa jurídica (PJ) e pessoa física (PF). Os dados relevantes, como CNPJ/CPF, razão social/nome e endereço, foram relacionados conforme necessário.
2. **Pagamentos**:
   Criamos uma tabela para registrar informações de pagamentos. Isso inclui detalhes como valor, data, método de pagamento e referência ao pedido associado. A relação entre pedidos e pagamentos foi estabelecida por meio de chaves estrangeiras.
3. **Entrega**:
   Para controlar as entregas, implementamos uma tabela que armazena dados como status do pedido, data de envio e código de rastreio. Novamente, vinculamos essas informações aos pedidos correspondentes.

![err](https://github.com/devcaiada/ecommerce-db-EER/blob/main/assets/ecommerce%20db.png?raw=true)

---
