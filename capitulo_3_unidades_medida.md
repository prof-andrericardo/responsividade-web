# 📘 Capítulo 3 – Unidades de Medida

> Este capítulo explora as diferentes unidades de medida no CSS, destacando as melhores práticas para criar layouts verdadeiramente responsivos. Você aprenderá a diferença entre unidades fixas e relativas, com foco em adaptabilidade e escalabilidade.

---

## 📗 Aula 3.1 – Unidades Fixas vs Relativas

### 🎯 Objetivo da Aula

Entender a diferença entre unidades fixas e relativas no CSS e como elas afetam o comportamento responsivo.

### 📐 Unidades Fixas

- `px` (pixels): valor absoluto e não escalável
- `cm`, `mm`, `in` (pouco usadas em telas, mais comuns em impressão)

```css
h1 {
  font-size: 24px;
}
```

🔴 **Desvantagem**: não se adapta ao tamanho da tela ou preferências do usuário.

---

### 📐 Unidades Relativas

- `em`: relativo ao tamanho da fonte do elemento pai
- `rem`: relativo ao tamanho da fonte raiz (`html`)
- `%`: relativo ao elemento pai (largura, altura, padding)
- `vw` / `vh`: relativo à largura e altura da viewport

```css
h1 {
  font-size: 2rem;
  padding: 5%;
  width: 80vw;
}
```

🟢 **Vantagem**: adaptável a múltiplos tamanhos de tela e preferências de acessibilidade

---

## 📗 Aula 3.2 – Quando Usar Cada Unidade?

### 🎯 Objetivo da Aula

Aprender a escolher a unidade ideal para cada situação em um layout responsivo.

### 📊 Comparação Rápida

| Unidade | Uso Ideal                               | Exemplo             |
| ------- | --------------------------------------- | ------------------- |
| `px`    | Bordas finas, linhas, ícones            | `border: 1px solid` |
| `rem`   | Tamanhos globais de fonte e espaçamento | `margin: 2rem`      |
| `em`    | Componentes internos escaláveis         | `padding: 1em`      |
| `%`     | Largura de contêineres, imagens         | `width: 100%`       |
| `vw`    | Largura de elementos baseados na tela   | `width: 50vw`       |
| `vh`    | Altura de seções full-screen            | `height: 100vh`     |

### 💡 Boas Práticas

- Use `rem` para tamanhos de fonte consistentes
- Evite `px` para largura, altura ou `font-size`
- Combine `%` com `max-width` para evitar estouros
- Use `vw` e `vh` com moderação (podem causar rolagem indesejada)

---

## 🧪 Atividade Prática

1. Crie três caixas lado a lado:

   - Uma com `px`
   - Uma com `%`
   - Uma com `vw`

2. Redimensione a janela do navegador e compare o comportamento de cada uma.

3. Experimente alterar o `font-size` do elemento `<html>` e veja como `rem` e `em` reagem.

---

## 📌 Conclusão do Capítulo 3

- Unidades **relativas são essenciais** para responsividade
- `rem` e `%` são as mais usadas para **layout fluido e escalável**
- Conhecer as unidades ajuda a evitar erros como elementos estourando ou textos ilegíveis

### 🧠 Checklist Rápido

-

### 📎 Próximo Capítulo:

➡️ Capítulo 4 – Flexbox

