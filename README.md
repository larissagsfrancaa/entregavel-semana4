# Entregável de Desenvolvimento Web – Arrays, DOM e Eventos – Semana 04

## 💻 Sobre o Projeto
Este projeto consiste na resolução dos desafios práticos propostos na aula de Manipulação de Arrays, DOM e Eventos (U4). O objetivo principal é dominar métodos modernos de iteração de arrays, manipulação dinâmica de elementos HTML e otimização de eventos na página.

O projeto é composto por um arquivo estrutural `index.html` e um script de comportamento `app.js` rodando em conjunto no navegador.

---

## 🧠 Conceitos e Métodos de Array Aplicados

No **Bloco 1**, foram aplicados os principais métodos do ES6 para gerenciamento de dados:
* **`forEach`:** Utilizado para percorrer coleções e executar ações (como impressões no console), sem gerar um novo array.
* **`map`:** Aplicado para transformar dados. Ele percorre o array original e retorna um **novo array** de mesmo tamanho com os elementos modificados (ex: nomes em caixa alta).
* **`filter`:** Utilizado para filtragem condicional. Retorna um **novo array** contendo apenas os elementos que atendem a um critério lógico (ex: preços maiores que 20 ou menores que 50).
* **`reduce`:** Método de acumulação. Ele reduz todos os valores de um array a um **único valor final** (ex: a soma total de todos os preços da lista).

---

## 🏗️ Manipulação do DOM e Lógica do Projeto

### Bloco 2 – Manipulação do DOM (`querySelector`, `createElement`, `classList`)
* Seleção dinâmica e alteração de textos de elementos usando `querySelector` e `querySelectorAll`.
* Inserção de itens em listas (`#lista`) utilizando tanto `innerHTML` quanto a criação segura de nós com `document.createElement()` combinado com `.append()`.
* Manipulação de estilos por meio do objeto `classList`, injetando e verificando a presença de classes CSS (`.add` e `.contains`).

### Bloco 3 – Eventos e Event Delegation
* **Captura de Eventos Comuns:** Manipulação de cliques (`click`), passagem de mouse (`mouseover`) e digitação em tempo real (`keyup`).
* **Formulário Resiliente:** Monitoramento do evento `submit` com o uso obrigatório de `e.preventDefault()` para bloquear o recarregamento automático da página, tratando strings com `.trim()` para rejeitar entradas vazias ou com espaços em branco.
* **Otimização com Event Delegation:** 
  * **O que é:** Em vez de adicionar um escutador (*listener*) para cada item `<li>` individualmente (o que sobrecarregaria a memória), foi adicionado **um único listener no elemento pai** (`#lista`).
  * **Importância:** Essa técnica melhora drasticamente a performance da aplicação e garante que **novos elementos criados dinamicamente** (como as tarefas adicionadas via formulário) herdem automaticamente o comportamento de clique sem a necessidade de registrar novos escutadores no código.

---

## 🚀 Como Executar o Projeto

1. Baixe os arquivos `index.html` e `app.js` na mesma pasta do seu computador.
2. Abra o arquivo `index.html` em qualquer navegador web (Google Chrome, Edge, Firefox, etc.).
3. Pressione a tecla **F12** (ou clique com o botão direito e vá em *Inspecionar*) e mude para a aba **Console** para acompanhar todas as saídas e logs gerados pelos scripts.

---

## ✍️ Autoria
Atividade acadêmica desenvolvida para a disciplina de **Desenvolvimento Web** (Semana 04).  
**Universidade CEUMA.**
