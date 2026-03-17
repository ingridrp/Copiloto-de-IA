#  Modo-Study.md — DOM e Eventos no JavaScript

---

## Objetivo do Estudo

Entender como o JavaScript interage com o HTML usando o DOM e como responder a ações do usuário com eventos.

---

##  Conceito 1 — DOM (Document Object Model)

### Conceito

DOM é a representação do HTML como objetos manipuláveis pelo JavaScript.

---

### Intuição

Pense no HTML como uma árvore.

Cada elemento (div, botão, input) é um “nó” que o JavaScript pode acessar e modificar.

---

### Exemplo simples

```id="a1x9pz"
// seleciona um elemento pelo id
const titulo = document.querySelector("#titulo");

// muda o texto
titulo.textContent = "Novo título";
```

---

### O que está acontecendo

* `querySelector` busca o elemento no HTML
* `textContent` altera o conteúdo

---

### Armadilhas comuns

* Elemento não existe → retorna `null`
* Script executa antes do HTML carregar

---

### Quando usar

* Sempre que precisar ler ou alterar algo na tela

---

### Quando evitar

* Evite buscar o mesmo elemento várias vezes (guarde em variável)

---

##  Conceito 2 — Seletores

### Conceito

Formas de encontrar elementos no DOM.

---

### Intuição

É como usar um “endereço” para encontrar algo na página.

---

### Exemplo

```id="v2lm8n"
document.querySelector("#id")
document.querySelector(".classe")
document.querySelector("button")
```

---

### O que está acontecendo

* `#` → id
* `.` → classe
* nome → tag

---

### Armadilhas comuns

* Esquecer `#` ou `.`
* Selecionar algo que ainda não existe

---

### Quando usar

* Sempre antes de manipular elementos

---

##  Conceito 3 — Eventos

### Conceito

Eventos são ações do usuário (clique, digitação, etc.).

---

### Intuição

Você “escuta” o que o usuário faz e reage.

---

### Exemplo simples

```id="x8pt2c"
const botao = document.querySelector("#btn");

botao.addEventListener("click", function() {
  alert("Clicou!");
});
```

---

### O que está acontecendo

* `addEventListener` registra uma ação
* `"click"` é o evento
* função executa quando ocorre

---

### Armadilhas comuns

* Esquecer de selecionar o elemento antes
* Erro de digitação no nome do evento

---

### Quando usar

* Interações com usuário (botões, inputs, etc.)

---

### Quando evitar

* Evitar múltiplos eventos desnecessários no mesmo elemento

---

## Conceito 4 — Manipulação de elementos

### Conceito

Criar, adicionar e remover elementos do DOM.

---

### Intuição

Você está “montando” o HTML via JavaScript.

---

### Exemplo

```id="5qz9jw"
const lista = document.querySelector("#lista");

const item = document.createElement("li");
item.textContent = "Nova tarefa";

lista.appendChild(item);
```

---

### O que está acontecendo

* `createElement` cria elemento
* `appendChild` adiciona na tela

---

### Armadilhas comuns

* Esquecer de adicionar no DOM
* Criar elemento mas não usar

---

### Quando usar

* Listas dinâmicas (ex: To-Do, notas)

---

## Conceito 5 — classList

### Conceito

Manipular classes CSS via JavaScript.

---

### Intuição

Você liga/desliga estilos dinamicamente.

---

### Exemplo

```id="m4j2kp"
item.classList.add("ativo");
item.classList.remove("ativo");
item.classList.toggle("ativo");
```

---

### O que está acontecendo

* `add` adiciona classe
* `remove` remove
* `toggle` alterna

---

### Armadilhas comuns

* Nome da classe errado
* Esperar efeito sem CSS definido

---

### Quando usar

* Mostrar/ocultar elementos
* Marcar como concluído

---

## Conectando tudo (visão geral)

Fluxo típico:

1. Selecionar elemento
2. Escutar evento
3. Executar ação
4. Atualizar DOM

---

##  Problema clássico

Erro:

```
Cannot read properties of null
```

### Por quê?

Elemento não foi encontrado.

### Solução

* Verificar seletor
* Usar:

```id="u8n1lw"
document.addEventListener("DOMContentLoaded", function() {
  // seu código aqui
});
```

---

## Mini exercício mental

Imagine:

* um input
* um botão
* uma lista

Pergunta:

 O que acontece quando o botão é clicado?

Resposta esperada:

* pegar valor do input
* criar elemento
* adicionar na lista

---


