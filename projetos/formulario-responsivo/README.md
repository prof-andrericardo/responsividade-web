# 📝 Projeto: Formulário Responsivo

> Este projeto propõe a construção de um formulário de contato responsivo, que se adapta a diferentes tamanhos de tela, mantém a legibilidade e oferece uma experiência amigável em dispositivos móveis.

---

## 🎯 Objetivos do Projeto

- Criar um formulário completo com campos de entrada, textarea e botão de envio
- Aplicar boas práticas de responsividade e acessibilidade
- Organizar campos com **Flexbox** ou **Grid**, adaptando o layout em diferentes larguras

---

## 📋 Estrutura do Formulário

### 🔹 Campos obrigatórios:

- Nome completo
- E-mail
- Assunto (dropdown ou input)
- Mensagem (textarea)
- Botão de envio

---

## 🧰 Técnicas Esperadas

- `display: flex` ou `grid` para organizar campos lado a lado em telas largas
- `flex-direction: column` ou `grid-template-columns: 1fr` em telas menores
- `label` vinculado ao `input` com `for` e `id`
- Unidades relativas (`rem`, `%`, `clamp()`, `vw`)
- `max-width`, `min-width`, `margin: auto` para centralização
- `:focus`, `:hover` e `transition` para estados visuais

---

## 📦 Estrutura de Arquivos Sugerida

```
projetos/
└── formulario-responsivo/
    ├── index.html
    ├── style.css
    └── README.md
```

---

## 🧪 Critérios de Avaliação

| Critério                                   | Peso |
| ------------------------------------------ | ---- |
| Layout responsivo com reorganização fluida | 30%  |
| Acessibilidade e usabilidade do formulário | 30%  |
| Organização e semântica do código          | 25%  |
| Estética visual e legibilidade             | 15%  |

---

## 🧠 Dicas de Desenvolvimento

- Utilize `fieldset` e `legend` se desejar agrupar campos
- Teste o formulário com teclado e sem mouse
- Teste campos preenchidos em diferentes larguras

---

## 🚀 Entrega Final

- Formulário responsivo funcional e validado
- Página hospedada ou capturas em diferentes dispositivos
- Código limpo, comentado e acessível

---

### 🏁 Resultado Esperado

Um formulário elegante e funcional que se adapta automaticamente entre 320px e 1440px, oferecendo ótima **experiência ao usuário e acessibilidade**.

