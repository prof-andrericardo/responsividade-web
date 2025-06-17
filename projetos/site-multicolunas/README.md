# 🧭 Projeto: Site Multicolunas Responsivo

> Este projeto tem como objetivo desenvolver um layout com múltiplas colunas que se reorganiza conforme a largura da tela. O foco está em simular um layout de blog, revista ou portal de notícias com boas práticas de grid, responsividade e tipografia.

---

## 🎯 Objetivos do Projeto

- Criar um layout com **duas ou mais colunas** adaptáveis
- Utilizar **CSS Grid** e **Flexbox** para organizar conteúdo
- Trabalhar a responsividade tanto em largura quanto em altura (altura mínima de viewport)

---

## 🧱 Estrutura Esperada

### 🔹 Seções sugeridas:

- **Cabeçalho** com logo e navegação
- **Coluna principal** com conteúdo textual (artigos, posts)
- **Barra lateral (sidebar)** com widgets, links ou categorias
- **Rodapé** com informações complementares

---

## 🧰 Técnicas e Boas Práticas

- `grid-template-columns: 2fr 1fr` (para coluna principal e sidebar)
- `flex-wrap`, `gap`, e `minmax()` para adaptação
- Uso de `clamp()` para fontes e `max-width: 100ch` para controle de largura de leitura
- `min-height: 100vh` para garantir preenchimento de tela
- Breakpoints com `min-width: 768px` e `1024px`

---

## 📦 Estrutura de Arquivos Sugerida

```
projetos/
└── site-multicolunas/
    ├── index.html
    ├── style.css
    ├── imagens/
    └── README.md
```

---

## 🧪 Critérios de Avaliação

| Critério                          | Peso |
| --------------------------------- | ---- |
| Estrutura multicolunas adaptável  | 30%  |
| Organização clara e semântica     | 25%  |
| Experiência de leitura em mobile  | 25%  |
| Estilo visual agradável e legível | 20%  |

---

## 🧠 Dicas de Desenvolvimento

- Colunas devem virar **empilhadas em telas pequenas**
- Sidebar pode ser reposicionada abaixo ou ocultada
- Mantenha o texto com espaçamento confortável (`line-height`, `padding`)

---

## 🚀 Entrega Final

- Site com layout funcional e adaptável de 2 ou 3 colunas
- Testado em diferentes tamanhos de viewport
- Disponível localmente ou em repositório público

---

### 🏁 Resultado Esperado

Um **site multicolunas fluido e moderno**, onde a experiência do usuário é mantida desde smartphones até monitores widescreen, com foco em leitura e organização visual.

