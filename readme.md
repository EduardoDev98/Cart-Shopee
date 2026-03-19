

🛒 Shopee Cart Simulator
🚀 Projeto Backend com Node.js | JavaScript | Clean Code








📌 Sobre o Projeto

Este projeto é uma simulação de carrinho de compras, inspirado em plataformas reais de e-commerce como a Shopee.

O principal objetivo foi demonstrar, na prática, conceitos fundamentais de backend, com foco em:

Implementação de regras de negócio

Organização e escalabilidade de código

Escrita de código limpo e manutenível

🧠 Conceitos Aplicados
🧩 Arquitetura Modular (ES Modules)

Separação clara de responsabilidades utilizando módulos nativos do JavaScript:

cartService.js → regras de negócio do carrinho

item.js → criação e estrutura dos itens

import * as cartService from "./services/cart.js";
import createItem from "./services/item.js";
⚙️ Uso de Async/Await

Mesmo sem integração externa, o uso de funções assíncronas simula cenários reais de backend (APIs, banco de dados).

const item = await createItem("produto", 10.99, 2);
🧮 Programação Funcional (reduce)

Cálculo do total do carrinho utilizando abordagem funcional:

const total = cart.reduce((sum, item) => sum + item.subtotal(), 0);
🔍 Manipulação de Arrays

Aplicação de métodos essenciais do JavaScript:

push() → adicionar itens

findIndex() → localizar itens

splice() → remover itens

forEach() → percorrer lista

🏗️ Factory Pattern (Encapsulamento)

Criação de itens com comportamento próprio:

function createItem(name, price, quantity) {
  return {
    name,
    price,
    quantity,
    subtotal: () => price * quantity,
  };
}
🛠️ Funcionalidades

✔ Adicionar item ao carrinho
✔ Remover uma unidade do item
✔ Deletar item completamente
✔ Listar itens do carrinho
✔ Calcular total automaticamente

📊 Regras de Negócio

Se a quantidade do item for maior que 1, apenas decrementa

Se a quantidade for igual a 1, o item é removido

O total é calculado dinamicamente com base no subtotal

📂 Estrutura do Projeto
📦 shopee-cart-simulator
 ┣ 📂 services
 ┃ ┣ 📄 cart.js
 ┃ ┗ 📄 item.js
 ┣ 📄 index.js
 ┣ 📄 package.json
▶️ Como Executar
# Clonar o repositório
git clone https://github.com/seu-usuario/seu-repo.git

# Acessar a pasta
cd shopee-cart-simulator

# Executar o projeto
node index.js
💡 Exemplo de Saída
Welcome to your Shopee Cart!

Shopee cart list:
1. hotwheels ferrari - R$ 20.99 | 50x | Subtotal = 1049.5
2. hotwheels lamborghini - R$ 39.99 | 3x | Subtotal = 119.97

Shopee Cart TOTAL IS:
🎁Total: 1169.47
🎯 Objetivo

Este projeto foi desenvolvido com foco em:

Evoluir habilidades em backend

Praticar boas práticas de código

Simular regras reais de sistemas de e-commerce

Servir como base para aplicações escaláveis

🚀 Próximos Passos

 Criar API REST com Node.js

 Integração com banco de dados (PostgreSQL / MongoDB)

 Implementar autenticação de usuário

 Criar frontend com React

 Persistência de carrinho

👨‍💻 Autor

Eduardo Garcia Ribeiro
💻 Desenvolvedor 

⭐ Considerações Finais

Apesar de ser um projeto simples, ele demonstra na prática fundamentos essenciais de engenharia de software, utilizados em aplicações reais.