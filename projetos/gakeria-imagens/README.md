# 🖼️ Projeto: Galeria de Imagens Responsiva

> Neste projeto prático, você criará uma galeria de imagens adaptável, com layout fluido e visual moderno, utilizando **CSS Grid**, media queries e boas práticas de acessibilidade.

---

## 🎯 Objetivos do Projeto
- Criar uma galeria que se adapta a diferentes tamanhos de tela
- Utilizar Grid Layout com `auto-fit` e `minmax()`
- Aplicar responsividade progressiva com Mobile First

---

## 🧱 Estrutura da Galeria
### 🔹 Seções principais:
- **Título da galeria** (`<h1>` ou `<header>`)
- **Grid de imagens** com legendas opcionais
- **Rodapé simples** com créditos ou informações adicionais

---

## 🧰 Técnicas Esperadas
- `display: grid` com `grid-template-columns: repeat(auto-fit, minmax(...))`
- Unidades relativas (`vw`, `%`, `rem`)
- `gap` para espaçamento entre itens
- `max-width: 100%` para imagens
- `object-fit: cover` para padronizar cortes
- `:hover` e `:focus` para interações simples
- Media Queries com breakpoints: 480px, 768px, 1024px

---

## 📦 Estrutura de Arquivos Sugerida
```
projetos/
└── galeria-imagens/
    ├── index.html
    ├── style.css
    ├── imagens/
    └── README.md
```

---

## 🧪 Critérios de Avaliação
| Critério                                | Peso |
|----------------------------------------|------|
| Layout adaptável e fluido              | 30%  |
| Código limpo e bem estruturado         | 25%  |
| Uso adequado do CSS Grid               | 25%  |
| Acessibilidade e descrição das imagens | 20%  |

---

## 🧠 Dicas de Desenvolvimento
- Utilize `alt` descritivo para todas as imagens
- Evite deixar imagens distorcidas: use `object-fit: cover`
- Teste com diferentes quantidades de imagens

---

## 🚀 Entrega Final
- Galeria funcional e responsiva em tela cheia e telas móveis
- Código comentado e organizado por seções
- Projeto disponível localmente ou via GitHub Pages

---

### 🏁 Resultado Esperado
Uma **galeria de imagens elegante, responsiva e acessível**, que funciona perfeitamente em dispositivos de diferentes tamanhos e resoluções.

