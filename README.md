# Solução de E-Commerce
Modelo de Entidade Relacionamento para uma Solução de E-Commerce
## Escopo do Modelo de ER para uma Solução de E-Commerce
### Requisitos – Produto
- Os produtos são vendidos por uma única plataforma online, mas podem ter vendedores distintos (maketplace);
- Cada produto possui um único fornecedor
- Um pedido pode ter mais de 1 unidade do mesmo produto e mais de um tipo de produto.
### Requisitos – Cliente:
- O cliente pode ser pessoa física ou pessoa jurídica, com CPF ou CNPJ respectivamente, como os atributos são diferentes teremos uma entidade para cada tipo de pessoa;
- O Endereço do cliente está vinculado ao valor do frete do pedido;
- Um cliente pode ter vários pedidos com vários produtos em cada um. Vinculado a cada pedido temos um período para devolução dos produtos;
- O cliente pode ter uma ou mais formas de pagamentos;
- O cliente pode ter um ou mais endereços para entrega. No caso de cliente pessoa jurídica normalmente o único endereço de entrega válido é o vinculado ao registrado no CNPJ da mesma.
### Requisitos – Pedido:
- O pedido é criado pelo cliente e possui informações de compra, endereço de entrega, status da entrega, forma de pagamento, data de entrega, código de rastreamento, data limite de devolução;
- Um pedido pode ter mais de 1 tipo de produto e mais de 1 item de cada produto;
- O pedido pode ser cancelado dependendo do status do pedido no momento.
### Requisitos – Fornecedor:
- Um produto pode ser disponibilizado por vários fornecedores para venda própria, mas a quantidade em estoque é agrupada independentemente do fornecedor e o valor de venda é o mesmo;
- Um produto também pode ser vendido via marketplace, nesse caso cada vendedor parceiro tem uma quantidade de produtos em estoque e um respectivo preço de venda para cada produto.
