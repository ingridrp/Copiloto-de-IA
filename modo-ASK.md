#  modo-ASK.md — Projeto To-Do List

##  Visão Geral

Projeto simples de lista de tarefas usando:

* HTML
* CSS
* JavaScript (Vanilla)

Executado diretamente no navegador (sem instalação).

---

##  Objetivo

Praticar:

* Manipulação de DOM
* Eventos
* Organização de código
* Contribuição em projetos Open Source

---

##Estrutura do Projeto

```
/projeto-todo
  index.html
  style.css
  script.js
  modo-ASK.md
```

---

## Funcionamento

### 1. Adicionar tarefa

Usuário digita no input e clica no botão.

Fluxo:

* Captura valor do input
* Cria elemento `<li>`
* Adiciona na lista

---

### 2. Remover tarefa

Cada item possui um botão de remover.

Fluxo:

* Evento de clique
* Remove o elemento do DOM

---

### 3. Marcar como concluída

Ao clicar na tarefa:

* Alterna classe CSS (`completed`)
* Aplica estilo visual

---

## Conceitos usados

### DOM

* `document.querySelector`
* `createElement`
* `appendChild`

### Eventos

* `click`
* `submit` (opcional)

### Classes CSS

* `classList.add`
* `classList.toggle`

---

## Possíveis problemas

### Erro: elemento null

Causa:

* seletor incorreto
* script carregando antes do HTML

Solução:

* usar `DOMContentLoaded`

---

### Input vazio

Causa:

* falta de validação

Solução:

* verificar `.value.trim()`

---

## Melhorias (Open Source)

Essas são sugestões ideais para contribuição:

###  Nível iniciante

* Validar input vazio
* Limpar campo após adicionar
* Melhorar CSS

---

###  Nível intermediário

* Salvar tarefas no `localStorage`
* Criar botão "limpar tudo"
* Contador de tarefas

---

###  Nível avançado (dentro da stack)

* Filtro:

  * todas
  * concluídas
  * pendentes
* Editar tarefa
* Drag and drop simples

---

##  Testes manuais

Checklist:

* [ ] Adicionar tarefa funciona
* [ ] Remover funciona
* [ ] Marcar como concluída funciona
* [ ] Não adiciona tarefa vazia

---

##  Boas práticas aplicadas

* Separação de arquivos
* Código simples e legível
* Uso básico de eventos
* Manipulação segura do DOM

---

##  Como contribuir

1. Faça um fork
2. Crie uma branch:

   ```
   git checkout -b minha-feature
   ```
3. Faça alterações
4. Commit:

   ```
   git commit -m "feat: nova funcionalidade"
   ```
5. Envie:

   ```
   git push origin minha-feature
   ```
6. Abra um Pull Request

---

##  Ideias de issues

Você pode criar issues como:

* "Adicionar persistência com localStorage"
* "Melhorar responsividade"
* "Corrigir bug ao remover tarefa"

---

