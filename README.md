# cp-.NET

📊 Modelo Entidade-Relacionamento (MER)

Este repositório contém o Modelo Entidade-Relacionamento (MER) de um sistema simples de gestão de pedidos.

O diagrama abaixo representa a estrutura conceitual das entidades, atributos e relacionamentos do sistema:

📌 Descrição do Modelo
🧑 Cliente

id_cliente (PK)

Nome_cliente

Email

Um cliente pode realizar um ou vários pedidos.

📦 Pedido

id_pedido (PK)

nome_pedido

id_cliente (FK)

id_funcionario (FK)

Cada pedido é feito por um único cliente, mas pode ser preparado por um ou mais funcionários.

👨‍💼 Funcionário

id_funcionario (PK)

cargo

nome_funcionario

Um funcionário pode preparar vários pedidos.

🔗 Relacionamentos

Cliente — Faz — Pedido

Um cliente pode fazer vários pedidos (1,N).

Cada pedido pertence a um único cliente (N,1).

Funcionário — Prepara — Pedido

Um funcionário pode preparar vários pedidos (1,N).

Cada pedido pode ser preparado por um ou mais funcionários (N,1).

🚀 Objetivo

Este modelo pode ser utilizado como base para implementação em um banco de dados relacional para sistemas de:

Restaurantes

Lanchonetes

Deliverys

Ou qualquer aplicação que envolva clientes, pedidos e funcionários.
