# 🧪 Desafio 03 – Refatorar uma Página para Mobile First

> Este desafio tem como objetivo reforçar o conceito de **Mobile First**, aplicando-o na refatoração de um site construído originalmente com abordagem Desktop First.

---

## 🎯 Objetivo do Desafio

Transformar uma página com Media Queries escritas em ordem descendente (ex: `max-width`) para uma abordagem **Mobile First**, com `min-width`, adaptando o layout para telas pequenas como prioridade.

---

## 📋 Requisitos da Página Original

A estrutura fornecida contém:

- Layout com largura fixa (`width: 1024px` ou similar)
- Media queries com `max-width`
- Elementos visualmente desorganizados em telas menores
- Possivelmente, uso excessivo de `px`

---

## 🛠️ O que você deve fazer

- ✅ Reescrever o CSS com **abordagem Mobile First** (`min-width`)
- ✅ Ajustar a ordem das regras CSS e reorganizar as Media Queries
- ✅ Refatorar unidades fixas para **unidades relativas** (`rem`, `%`, `vw`, etc.)
- ✅ Testar o layout de **baixo para cima** (320px → 1440px)

---

## 📐 Breakpoints Mínimos Sugeridos

```css
@media (min-width: 480px) {}
@media (min-width: 768px) {}
@media (min-width: 1024px) {}
```

---

## 📦 Estrutura de Arquivos Sugerida

```
desafios/
└── desafio-03/
    ├── index.html               # Página com CSS Desktop First
    ├── style-original.css       # Código legado (não editar)
    ├── style-mobile-first.css   # Seu novo CSS
    └── README.md
```

---

## 🧠 Dicas de Refatoração

- Comece resetando os estilos com `box-sizing: border-box`
- Aplique os estilos base sem Media Queries
- Insira Media Queries progressivas com `min-width`
- Teste sempre que modificar uma seção

---

## 🧪 Critérios de Avaliação

| Critério                                | Peso |
| --------------------------------------- | ---- |
| Uso correto da estratégia Mobile First  | 30%  |
| Clareza e organização do CSS            | 25%  |
| Responsividade e fluidez entre tamanhos | 25%  |
| Código limpo, comentado e acessível     | 20%  |

---

## ✅ Entrega

- Inclua ambos os arquivos CSS no projeto
- Documente suas decisões de refatoração no `README.md`
- Apresente comparativos (antes/depois) com capturas ou vídeo

---

### 🏁 Resultado Esperado

Uma página que **prioriza a experiência em dispositivos móveis**, com **Media Queries progressivas** e um layout fluido e escalável, conforme os princípios de **design responsivo moderno**.

