# 📘 Capítulo 4 – Flexbox

> Este capítulo apresenta o **Flexbox**, um poderoso sistema de layout unidimensional do CSS que facilita a criação de layouts responsivos com alinhamentos flexíveis, distribuição de espaço e reorganização de elementos em diferentes tamanhos de tela.

---

## 📗 Aula 4.1 – Conceitos Principais do Flexbox

### 🎯 Objetivo da Aula

Entender os fundamentos do Flexbox e como ativar seu comportamento em containers.

### 📖 O que é Flexbox?

> **Flexbox (Flexible Box Layout)** é um módulo CSS que organiza os elementos filhos de forma eficiente em um eixo principal e/ou secundário, mesmo quando o tamanho deles é desconhecido.

### 🧱 Terminologia Básica

- **Container Flex**: elemento com `display: flex;`
- **Itens Flex**: filhos diretos do container flex
- **Eixo principal**: direção de fluxo (horizontal ou vertical)
- **Eixo transversal**: perpendicular ao eixo principal

### 💡 Ativando o Flexbox

```css
.container {
  display: flex;
}
```

---

## 📗 Aula 4.2 – Direção, Alinhamento e Espaçamento

### 🎯 Objetivo da Aula

Aplicar propriedades de alinhamento, direção e espaçamento dos itens dentro de um container flexível.

### 📦 Propriedades Essenciais

| Propriedade       | Função                              | Exemplo                   |
| ----------------- | ----------------------------------- | ------------------------- |
| `flex-direction`  | Define o eixo principal             | `row`, `column`           |
| `justify-content` | Alinha os itens no eixo principal   | `center`, `space-between` |
| `align-items`     | Alinha os itens no eixo transversal | `center`, `stretch`       |
| `gap`             | Espaçamento entre os itens          | `gap: 1rem`               |

### 🧠 Exemplo Prático

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  gap: 1rem;
}
```

### 📏 Visualização das Direções

- `row` (padrão): da esquerda para a direita
- `column`: de cima para baixo

### 🧪 Atividade Proposta

Crie um container com três blocos coloridos e teste:

- `justify-content: space-around`
- `align-items: stretch`
- `flex-direction: column`

---

## 📗 Aula 4.3 – Layouts Práticos com Flexbox

### 🎯 Objetivo da Aula

Criar layouts reais e responsivos usando Flexbox para simular seções comuns de sites.

### 📐 Layout de Cabeçalho (Navbar)

```css
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
}
```

### 📐 Layout de Cartões

```css
.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

.card {
  flex: 1 1 300px;
}
```

> 🧠 `flex: 1 1 300px` permite que o cartão cresça, encolha e tenha no mínimo 300px

### 📐 Layout com Sidebar

```css
.container {
  display: flex;
}

.sidebar {
  flex: 0 0 250px;
}

.main {
  flex: 1;
}
```

### 🔍 Observações

- Use `flex-wrap: wrap` para quebrar linhas automaticamente
- Combine Flexbox com Media Queries para tornar os layouts mais adaptáveis

### 🧪 Atividade Proposta

Crie um layout com três seções:

1. Cabeçalho fixo no topo
2. Barra lateral à esquerda
3. Conteúdo principal que ocupa o restante do espaço

Teste o comportamento ao redimensionar a tela.

---

## 📌 Conclusão do Capítulo 4

- **Flexbox** é ideal para layouts lineares (menu, cabeçalho, lista de itens)
- Facilita o alinhamento vertical e horizontal com poucas linhas de código
- Suporta reorganização e espaçamento dinâmico entre itens

### 🧠 Checklist Rápido

-

### 📎 Próximo Capítulo:

➡️ Capítulo 5 – CSS Grid

