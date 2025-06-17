# 📘 Capítulo 5 – CSS Grid

> Este capítulo apresenta o **CSS Grid Layout**, um sistema bidimensional que permite criar layouts complexos e responsivos com controle total sobre colunas e linhas. Ideal para estruturar áreas principais de páginas web com precisão.

---

## 📗 Aula 5.1 – Introdução ao Grid Layout

### 🎯 Objetivo da Aula

Compreender o conceito de grid no CSS, ativar seu comportamento e criar a estrutura inicial de linhas e colunas.

### 🧠 O que é CSS Grid?

> **CSS Grid** é um sistema de layout bidimensional que permite posicionar elementos em linhas e colunas, facilitando a criação de estruturas responsivas e consistentes.

### 🧩 Ativando o Grid

```css
.container {
  display: grid;
}
```

### 📐 Exemplo básico com colunas

```css
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}
```

> 🧠 Cria três colunas com largura igual (frações do espaço disponível)

### 📏 Principais Unidades

- `fr`: fração do espaço disponível
- `px`, `%`, `auto`: tamanhos fixos ou relativos

---

## 📗 Aula 5.2 – Definindo Linhas, Colunas e Gaps

### 🎯 Objetivo da Aula

Criar grades controlando o número de linhas, colunas, espaçamento e repetição de padrões.

### 📐 Exemplo com linhas e espaçamento

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 100px auto;
  gap: 1rem;
}
```

### 🔁 Uso de `repeat()`

```css
grid-template-columns: repeat(4, 1fr);
```

> 💡 Repete 4 colunas com largura igual

### 🔄 `auto-fit` vs `auto-fill`

```css
.container {
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}
```

- `auto-fit`: remove espaços vazios
- `auto-fill`: mantém o espaço reservado, mesmo vazio

### 🧪 Atividade Proposta

Crie uma galeria com 6 imagens dispostas em 3 colunas e 2 linhas, com espaçamento entre os itens. Use `repeat()` e `gap`.

---

## 📗 Aula 5.3 – Áreas Nomeadas e Responsividade

### 🎯 Objetivo da Aula

Utilizar áreas nomeadas no grid para estruturar o layout e adaptá-lo com media queries.

### 📦 Definindo Áreas

```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar content"
    "footer footer";
  grid-template-columns: 1fr 3fr;
  grid-template-rows: auto 1fr auto;
}

.header  { grid-area: header; }
.sidebar { grid-area: sidebar; }
.content { grid-area: content; }
.footer  { grid-area: footer; }
```

### 🔀 Tornando o layout responsivo

```css
@media (max-width: 768px) {
  .container {
    grid-template-areas:
      "header"
      "content"
      "sidebar"
      "footer";
    grid-template-columns: 1fr;
  }
}
```

### 🧪 Atividade Proposta

Monte um layout completo com header, sidebar, conteúdo e footer usando áreas nomeadas. Adapte o layout com uma media query para telas pequenas.

---

## 📌 Conclusão do Capítulo 5

- **CSS Grid** é ideal para layouts estruturais e áreas fixas
- Permite controle total sobre linhas, colunas e espaçamento
- Se complementa muito bem com Flexbox (para conteúdo interno)

### 🧠 Checklist Rápido

-

### 📎 Próximo Capítulo:

➡️ Capítulo 6 – Componentes Responsivos

