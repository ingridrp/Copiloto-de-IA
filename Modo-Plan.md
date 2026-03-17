# Modo-Plan.md — Projeto Notes App

---

## Objetivo

Criar uma aplicação simples de **gerenciamento de notas** no navegador, com persistência usando `localStorage`.

---

##  Contexto e Assunções

### Assunções

* O projeto será executado abrindo `index.html`
* JavaScript estará em `script.js`
* CSS separado em `style.css`
* Interface simples (lista de notas)

### Limitações

* Sem Node.js
* Sem banco de dados
* Sem frameworks
* Apenas navegador

### Pontos em aberto

* Edição será feita via `prompt` (assumido por ser mais simples)

---

##  Escopo

### Inclui

* Criar nota
* Editar nota
* Excluir nota
* Listar notas
* Persistir dados com `localStorage`

### Não inclui

* Login
* Backend
* Upload de arquivos
* Editor avançado

---

##  Estratégia

* Usar array em memória para armazenar notas
* Sincronizar com `localStorage`
* Re-renderizar lista completa a cada alteração
* Usar eventos de clique para ações
* Estrutura simples para facilitar entendimento

---

##  Estrutura do Projeto

```
/projeto-notas
  index.html
  style.css
  script.js
  Modo-Plan.md
```

---

##  Modelo de Dados

```
Nota = {
  id: number,
  texto: string
}
```

---

##  Funções principais (planejamento)

```
carregarNotas()
salvarNotas()
adicionarNota(texto)
editarNota(id, novoTexto)
removerNota(id)
renderizarNotas()
```

---

##  Plano passo a passo

### 1. HTML

* Criar:

  * textarea (entrada de texto)
  * botão "Adicionar"
  * container de notas

---

### 2. CSS

* Layout em coluna
* Estilizar notas como “cards”
* Botões visíveis (editar/excluir)

---

### 3. JavaScript — Base

* Criar array de notas
* Implementar carregar/salvar no `localStorage`

---

### 4. Adicionar nota

* Capturar texto
* Validar (não vazio)
* Criar objeto nota
* Salvar e renderizar

---

### 5. Renderização

* Limpar container
* Criar elementos HTML para cada nota
* Adicionar botões (editar/excluir)

---

### 6. Remover nota

* Identificar pelo `id`
* Remover do array
* Atualizar armazenamento
* Re-renderizar

---

### 7. Editar nota

* Usar `prompt`
* Atualizar texto
* Salvar e re-renderizar

---

### 8. Persistência

* Usar:

  * `JSON.stringify`
  * `JSON.parse`

---

## Testes e validação

### Testes principais

* [ ] Adicionar nota
* [ ] Editar nota
* [ ] Remover nota
* [ ] Recarregar página mantém dados

### Casos extremos

* [ ] Texto vazio
* [ ] Texto muito longo
* [ ] Muitas notas (20+)

### Como validar

* Abrir `index.html`
* Interagir com a interface
* Verificar `localStorage` no DevTools

---

##  Riscos e mitigação

### DOM não encontrado

* Usar `DOMContentLoaded`

### Entrada inválida

* Validar com `.trim()`

### Erro no localStorage

* Sempre usar JSON corretamente

### IDs duplicados

* Usar `Date.now()`

---

## Melhorias futuras

* Contador de notas
* Botão "limpar tudo"
* Filtro (todas / editadas)
* UI mais moderna
* Responsividade

---

