# Chave-Estrangeira
Criação de chave estrangeira.

ALTER TABLE tb_pedidos
ADD CONSTRAINT fk_pedidos_clientes
FOREIGN KEY (cliente_id)
REFERENCES tb_clientes(cliente_id);
