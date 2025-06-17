# 🧪 Desafio 01 – Transformar Layout Fixo em Responsivo

> Este desafio irá testar sua habilidade em refatorar um layout estático tradicional (baseado em `px`) para um layout **responsivo**, utilizando as técnicas aprendidas nos capítulos anteriores.

---

## 🎯 Objetivo

Converter um layout fixo (largura definida em `px`) para um layout responsivo que se adapta a diferentes tamanhos de tela.

---

## 📋 Requisitos do Layout Inicial

Você receberá um HTML e CSS com as seguintes características:

- `width: 960px;`
- Fontes com `px`
- Espaçamentos em `px`
- Sem media queries
- Layout quebrando em telas menores que 768px

---

## 🛠️ O que você deve fazer

- ✅ Substituir unidades fixas por **unidades relativas** (`%`, `rem`, `vw`, etc.)
- ✅ Aplicar **Media Queries** com breakpoints apropriados
- ✅ Usar **Flexbox** ou **CSS Grid** para estruturar colunas e seções
- ✅ Tornar textos legíveis em telas menores
- ✅ Garantir boa organização visual entre 320px e 1440px

---

## 📐 Breakpoints Recomendados

```css
@media (max-width: 480px) {}
@media (max-width: 768px) {}
@media (min-width: 1024px) {}
```

---

## 📦 Arquivos Sugeridos

```
desafios/
└── desafio-01/
    ├── index.html      # Layout fixo original
    ├── style.css       # CSS base com px
    └── README.md       # Instruções do desafio
```

---

## 🧠 Dicas

- Comece definindo o `meta viewport` corretamente
- Utilize `flex-wrap` ou `auto-fit` para adaptação automática
- Teste com DevTools simulando diferentes dispositivos

---

## 🧪 Critérios de Avaliação

| Critério                                    | Peso |
| ------------------------------------------- | ---- |
| Uso correto de unidades relativas           | 25%  |
| Aplicação de media queries                  | 25%  |
| Organização visual em diferentes resoluções | 25%  |
| Código limpo, indentado e comentado         | 25%  |

---

## ✅ Entrega

- Um novo arquivo CSS (`style-responsivo.css`) pode ser criado ou substitua o original.
- Inclua comentários no CSS justificando as escolhas de layout.
- Crie um GIF ou captura de tela mostrando o layout em diferentes tamanhos.

---

### 🏁 Boa sorte!

> Esse é o momento de aplicar tudo que você aprendeu: do `meta viewport` ao `flex: 1 1 auto`. Vamos colocar em prática o **design responsivo de verdade**!

