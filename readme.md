

  <img src="https://via.placeholder.com/1200x300.png?text=Shopee+Cart+Simulator" alt="Banner Shopee Cart Simulator" />
</p>

<h1 align="center">🛒 Shopee Cart Simulator</h1>

<p align="center">
  🚀 Projeto Backend com Node.js | JavaScript | Clean Code
</p>

<p align="center">
  <img src="https://img.shields.io/badge/status-em%20desenvolvimento-blue" />
  <img src="https://img.shields.io/badge/focus-backend-important" />
  <img src="https://img.shields.io/badge/javascript-ESModules-yellow" />
  <img src="https://img.shields.io/badge/node.js-runtime-green" />
  <img src="https://img.shields.io/badge/portfolio-project-purple" />
  <img src="https://img.shields.io/badge/open%20to-work-success" />
</p>

---

## 🎥 Demonstração

<p align="center">
  <img src="https://via.placeholder.com/800x400.gif?text=Demo+do+Projeto" alt="Demo do projeto" />
</p>


## 📌 Sobre o Projeto

Este projeto é uma **simulação de carrinho de compras**, inspirado em plataformas reais de e-commerce.

Ele foi desenvolvido com foco em:

- 📦 Regras de negócio reais  
- 🧱 Arquitetura modular  
- 🧼 Clean Code  
- ⚙️ Preparação para backend real (API + banco)  

---

## 🧠 Conceitos Aplicados

### 🧩 Arquitetura Modular
```js
import * as cartService from "./services/cart.js";
import createItem from "./services/item.js";
````
### ⚙️ Async/Await

Uso de funções assíncronas simulando cenários reais de backend:

```js
const item = await createItem("produto", 10.99, 2);
````
🧮 Programação Funcional (reduce)

Cálculo do total utilizando abordagem funcional:
```js
const total = cart.reduce((sum, item) => sum + item.subtotal(), 0);
````

🔍 Manipulação de Arrays

Principais métodos utilizados:

push() → adicionar itens

findIndex() → localizar itens

splice() → remover itens

forEach() → percorrer lista

🏗️ Factory Pattern (Encapsulamento)

Criação de itens com comportamento próprio:
```js
function createItem(name, price, quantity) {
  return {
    name,
    price,
    quantity,
    subtotal: () => price * quantity,
  };
}
````
🛠️ Funcionalidades

✔️ Adicionar item ao carrinho
✔️ Remover uma unidade do item
✔️ Deletar item completamente
✔️ Listar itens do carrinho
✔️ Calcular total automaticamente

📊 Regras de Negócio

Quantidade > 1 → decrementa

Quantidade = 1 → remove item

Total calculado dinamicamente
```js
📂 Estrutura do Projeto
📦 shopee-cart-simulator
 ┣ 📂 services
 ┃ ┣ 📄 cart.js
 ┃ ┗ 📄 item.js
 ┣ 📄 index.js
 ┣ 📄 package.json
````
▶️ Como Executar
```js
# Clonar o repositório
git clone https://github.com/EduardoDev98/Cart-Shopee

# Acessar a pasta
cd shopee-cart-simulator

# Executar o projeto
node index.js
````
💡 Exemplo de Saída
```js
Welcome to your Shopee Cart!

Shopee cart list:
1. hotwheels ferrari - R$ 20.99 | 50x | Subtotal = 1049.5
2. hotwheels lamborghini - R$ 39.99 | 3x | Subtotal = 119.97

Shopee Cart TOTAL IS:
🎁Total: 1169.47
````
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
💻 Desenvolvedor Full Stack 

⭐ Considerações Finais

Este projeto demonstra na prática fundamentos essenciais de engenharia de software, com foco em organização, escalabilidade e boas práticas.
