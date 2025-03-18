# Chave-Estrangeira
Criação de chave estrangeira.

ALTER TABLE tb_pedidos
ADD CONSTRAINT fk_pedidos_clientes
FOREIGN KEY (cliente_id)
REFERENCES tb_clientes(cliente_id);

==============================================================================================================================================================
Incluir os inserts no Banco de Dados do MySQL:

INSERT INTO tb_clientes (cliente_nome, cliente_email, cliente_telefone) VALUES

('Ana Souza', 'ana@email.com', '11987654321'),

('João Silva', 'joao@email.com', '11976543210'),

('Carlos Mendes', 'carlos@email.com', '11965432109'),

('Mariana Lima', 'mariana@email.com', '11954321098'),

('Fernanda Costa', 'fernanda@email.com', '11943210987');


INSERT INTO tb_pedidos (cliente_id, pedido_data) VALUES

(1, '2024-03-01'),

(2, '2024-03-02'),

(3, '2024-03-03'),

(4, '2024-03-04'),

(2, '2024-03-05');


INSERT INTO tb_produtos (produto_nome, produto_preco) VALUES

('Notebook', 3500.00),

('Mouse', 120.00),

('Teclado', 200.00),

('Monitor', 900.00),

('Impressora', 700.00);


INSERT INTO tb_itens_pedido (pedido_id, produto_id, quantidade) VALUES

(1, 1, 1),

(1, 2, 2),

(2, 3, 1),

(3, 4, 1),

(4, 5, 1);

INSERT INTO tb_pagamentos (pedido_id, pagamento_valor, pagamento_data) VALUES

(1, 3740.00, '2024-03-02'),

(2, 200.00, '2024-03-03');
