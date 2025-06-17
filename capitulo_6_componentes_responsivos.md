# 📘 Capítulo 6 – Componentes Responsivos

> Neste capítulo, vamos desenvolver componentes web adaptáveis: menus hambúrguer, imagens fluidas e estruturas como tabelas e cards que se ajustam automaticamente em diferentes tamanhos de tela.

---

## 📗 Aula 6.1 – Criando um Menu Hambúrguer Responsivo

### 🎯 Objetivo da Aula

Implementar um menu de navegação que se transforma em botão hambúrguer em telas pequenas.

### 📐 Estrutura HTML

```html
<nav class="navbar">
  <div class="logo">Logo</div>
  <button class="menu-toggle">☰</button>
  <ul class="menu">
    <li><a href="#">Início</a></li>
    <li><a href="#">Sobre</a></li>
    <li><a href="#">Serviços</a></li>
    <li><a href="#">Contato</a></li>
  </ul>
</nav>
```

### 🎨 Estilos CSS

```css
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
}

.menu {
  display: flex;
  gap: 1rem;
  list-style: none;
}

.menu-toggle {
  display: none;
  font-size: 2rem;
  background: none;
  border: none;
  cursor: pointer;
}

@media (max-width: 768px) {
  .menu {
    display: none;
    flex-direction: column;
  }
  .menu-toggle {
    display: block;
  }
  .menu.active {
    display: flex;
  }
}
```

### 🧠 Interatividade com JavaScript (opcional)

```js
document.querySelector('.menu-toggle').addEventListener('click', () => {
  document.querySelector('.menu').classList.toggle('active');
});
```

### 🧪 Atividade Proposta

Implemente um menu com os estilos acima e teste em dispositivos móveis e desktop.

---

## 📗 Aula 6.2 – Imagens Adaptáveis com `srcset` e `picture`

### 🎯 Objetivo da Aula

Exibir imagens apropriadas para cada tipo de dispositivo, economizando largura de banda e garantindo nitidez.

### 📷 Exemplo com `srcset`

```html
<img src="img-medium.jpg"
     srcset="img-small.jpg 480w, img-medium.jpg 768w, img-large.jpg 1200w"
     sizes="(max-width: 480px) 100vw, (max-width: 768px) 50vw, 33vw"
     alt="Imagem Responsiva">
```

### 🖼️ Exemplo com `picture`

```html
<picture>
  <source media="(max-width: 768px)" srcset="img-mobile.jpg">
  <source media="(min-width: 769px)" srcset="img-desktop.jpg">
  <img src="img-desktop.jpg" alt="Imagem com fallback">
</picture>
```

### ✅ Boas Práticas

- Usar imagens otimizadas
- Testar diferentes densidades de tela
- Fornecer sempre um `alt` descritivo

### 🧪 Atividade Proposta

Crie uma `<picture>` com diferentes imagens para celular e desktop. Inspecione com DevTools simulando vários tamanhos.

---

## 📗 Aula 6.3 – Tabelas e Cards Adaptáveis

### 🎯 Objetivo da Aula

Adaptar estruturas complexas como tabelas e cards para visualização em telas pequenas.

### 📊 Tabelas com Scroll Horizontal

```css
.tabela-responsiva {
  overflow-x: auto;
  display: block;
  max-width: 100%;
}
```

```html
<div class="tabela-responsiva">
  <table>
    <tr><th>Nome</th><th>Email</th><th>Cargo</th></tr>
    <tr><td>João</td><td>joao@email.com</td><td>Dev</td></tr>
  </table>
</div>
```

### 📦 Cards Flexíveis

```css
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
}
```

### 🧪 Atividade Proposta

Crie uma lista de cards com `grid-template-columns` usando `auto-fit` e `minmax`. Teste a adaptação em telas menores.

---

## 📌 Conclusão do Capítulo 6

- Componentes devem se adaptar de forma fluida ao tamanho da tela
- Menus, imagens e estruturas como tabelas exigem atenção especial
- A combinação de **CSS**, **HTML semântico** e **interatividade opcional com JS** garante usabilidade em todos os dispositivos

### 🧠 Checklist Rápido

-

### 📎 Próximo Capítulo:

➡️ Capítulo 7 – Ferramentas de Teste

