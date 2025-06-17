# 📘 Capítulo 2 – Media Queries e Breakpoints

> Este capítulo explora a base técnica para criar layouts adaptáveis: as media queries. Você aprenderá a utilizá-las com eficiência, escolhendo breakpoints estratégicos para adaptar o design a diferentes tamanhos de tela.

---

## 📗 Aula 2.1 – Introdução às Media Queries

### 🎯 Objetivo da Aula

Entender o que são media queries, para que servem e como usá-las de forma eficiente no CSS.

### 📖 O que são Media Queries?

> **Media Queries** são regras CSS condicionais que permitem aplicar estilos diferentes dependendo das características do dispositivo (largura, altura, tipo de tela, etc).

### 🧩 Estrutura Básica

```css
@media (condição) {
  /* estilos aplicados se a condição for verdadeira */
}
```

### 🧠 Exemplo Prático

```css
body {
  background-color: white;
}

@media (max-width: 768px) {
  body {
    background-color: lightgray;
  }
}
```

*Este exemplo altera a cor de fundo para cinza claro quando a largura da tela for menor ou igual a 768px.*

### 🔎 Outras Condições Comuns

- `min-width` / `max-width`
- `orientation: portrait` / `landscape`
- `min-resolution` (para telas retina)

### 🧪 Atividade Proposta

Edite um arquivo CSS para mudar a cor do texto e o tamanho da fonte em telas pequenas (< 600px). Teste no DevTools.

---

## 📗 Aula 2.2 – Breakpoints Comuns e Boas Práticas

### 🎯 Objetivo da Aula

Conhecer os pontos de quebra (breakpoints) mais utilizados e como organizá-los para um CSS limpo e funcional.

### 📏 O que são Breakpoints?

> **Breakpoints** são larguras de tela nas quais o layout “quebra” ou muda para se adaptar melhor ao dispositivo.

### 📊 Exemplos de Breakpoints Recomendados

| Dispositivo        | Breakpoint sugerido |
| ------------------ | ------------------- |
| Celulares pequenos | `max-width: 480px`  |
| Smartphones        | `max-width: 768px`  |
| Tablets            | `max-width: 1024px` |
| Desktops médios    | `max-width: 1280px` |
| Monitores grandes  | `min-width: 1440px` |

### ✅ Boas Práticas

- Comece pelo **Mobile First** usando `min-width`
- Use `em` ou `rem` em vez de `px` para breakpoints escaláveis
- Mantenha os breakpoints consistentes entre arquivos
- Agrupe media queries por componente, não por resolução

### 🧪 Atividade Proposta

Crie uma seção que mude de coluna única para duas colunas a partir de `min-width: 768px`.

---

## 📗 Aula 2.3 – Media Queries Avançadas

### 🎯 Objetivo da Aula

Utilizar media queries com múltiplas condições e aplicar estratégias para testes reais em diferentes dispositivos.

### 🧠 Múltiplas Condições

```css
@media screen and (min-width: 768px) and (orientation: landscape) {
  .container {
    flex-direction: row;
  }
}
```

### 🖥️ Media Types Comuns

- `screen`: telas em geral
- `print`: para impressão
- `all`: todos os dispositivos (default)

### 🛠️ Dica Técnica

Use `only screen` para evitar bugs em navegadores antigos:

```css
@media only screen and (max-width: 600px) {
  /* estilos */
}
```

### 📦 Estratégia Mobile First com Media Queries

```css
.card {
  padding: 1rem;
}

@media (min-width: 768px) {
  .card {
    display: flex;
    padding: 2rem;
  }
}
```

### 🧪 Atividade Proposta

Aplique uma media query que esconda o menu lateral em telas menores que 600px e o exiba novamente acima de 768px.

---

## 📌 Conclusão do Capítulo 2

- **Media Queries** são ferramentas poderosas para adaptar layouts.
- **Breakpoints bem escolhidos** evitam quebras visuais e melhoram a experiência.
- A estratégia **Mobile First com min-width** é preferida na maioria dos casos.

### 🧠 Checklist Rápido

-

### 📎 Próximo Capítulo:

➡️ Capítulo 3 – Unidades de Medida

