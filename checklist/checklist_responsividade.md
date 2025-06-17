# ✅ Checklist de Responsividade Web

> Use este checklist como guia de verificação técnica e visual para garantir que seu site esteja verdadeiramente responsivo. Ideal para revisões finais de projetos, correção entre pares ou autoavaliação.

---

## 📐 Estrutura e Layout
- [ ] O layout **não usa larguras fixas** (ex: `width: 960px`)
- [ ] Utiliza **unidades relativas** como `%`, `rem`, `vw`, `min()` e `clamp()`
- [ ] Usa **Flexbox** e/ou **Grid Layout** de forma apropriada
- [ ] Os elementos se **adaptam ao tamanho da viewport** sem quebrar
- [ ] O conteúdo **não ultrapassa a largura da tela** (overflow-x)
- [ ] O layout é construído com abordagem **Mobile First** (`min-width`)

---

## 🔎 Media Queries
- [ ] Media Queries são utilizadas com **breakpoints bem escolhidos**
- [ ] A organização das Media Queries é clara e consistente
- [ ] O conteúdo muda de forma fluida entre os diferentes pontos de quebra
- [ ] Há **ao menos 3 breakpoints** implementados (ex: 480px, 768px, 1024px)

---

## 🖼️ Imagens e Componentes Visuais
- [ ] Imagens utilizam **`max-width: 100%`** e mantêm proporção
- [ ] Quando necessário, utiliza-se **`srcset`** ou **`<picture>`**
- [ ] Menus, tabelas e cards são **totalmente responsivos**
- [ ] O menu hamburguer é funcional e intuitivo em telas pequenas

---

## 🛠️ Testes e Usabilidade
- [ ] A página foi testada em **mínimo 3 tamanhos de tela** (mobile, tablet, desktop)
- [ ] Testado no **DevTools** com diferentes dispositivos simulados
- [ ] O layout mantém boa **legibilidade e espaçamento** em todas as resoluções
- [ ] A performance foi avaliada com **Lighthouse**

---

## 📦 Acessibilidade e Código
- [ ] Tags semânticas HTML5 são utilizadas (`header`, `main`, `nav`, `section`, `footer`)
- [ ] O contraste de cor está adequado (verificado com Lighthouse ou ferramentas)
- [ ] Os elementos são **navegáveis por teclado** (sem obstáculos)
- [ ] O CSS está organizado, indentado e comentado

---

## 🧠 Extra: Boas Práticas de Responsividade
- [ ] O projeto utiliza fontes escaláveis com `rem` ou `clamp()`
- [ ] Scroll horizontal é evitado
- [ ] Layouts que combinam **Flexbox e Grid** são utilizados estrategicamente
- [ ] Foi adotado um **reset ou normalização de CSS** (`normalize.css`, `reset.css` ou `box-sizing: border-box`)

---

### 🏁 Conclusão
Marcar todos os itens não garante um layout perfeito, mas indica uma forte aplicação de **boas práticas em design responsivo**. Use este checklist em todos os seus projetos para entregar páginas funcionais, adaptáveis e acessíveis!

📌 *Dica*: imprima esse checklist ou inclua como parte do seu repositório README.md para revisões contínuas.

