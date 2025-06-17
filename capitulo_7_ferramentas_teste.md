# 📘 Capítulo 7 – Ferramentas de Teste

> Neste capítulo, você aprenderá a utilizar ferramentas profissionais para testar, validar e melhorar seus layouts responsivos. O foco está no uso do DevTools, da extensão Lighthouse e da aplicação de frameworks como Bootstrap e Tailwind para agilizar o processo.

---

## 📗 Aula 7.1 – Usando o Modo Dispositivo no DevTools

### 🎯 Objetivo da Aula

Testar o comportamento do site em diferentes resoluções utilizando o DevTools do navegador.

### 🧪 Acessando o DevTools

1. Abra o navegador (Google Chrome recomendado)
2. Pressione `Ctrl + Shift + I` (ou clique com o botão direito → “Inspecionar”)
3. Clique no ícone 📱 **“Toggle device toolbar”** (atalho: `Ctrl + Shift + M`)

### 📱 Recursos Disponíveis

- Simulação de resoluções de smartphones e tablets
- Alteração da densidade de pixels (DPI)
- Geração de **screenshots responsivos**
- Acesso direto ao código CSS/HTML para edições ao vivo

### 🔍 Dica Extra

Use o menu suspenso para testar em dispositivos como:

- iPhone SE / iPhone 12 Pro
- Galaxy S20 / Pixel 5
- iPad / iPad Pro

### 🧪 Atividade Proposta

Abra um dos seus projetos em HTML/CSS e teste com pelo menos 5 resoluções diferentes. Faça ajustes ao vivo e salve as melhorias no código.

---

## 📗 Aula 7.2 – Auditando com Lighthouse

### 🎯 Objetivo da Aula

Realizar auditorias de performance, acessibilidade e responsividade utilizando o Lighthouse, uma extensão do Google Chrome.

### 🚀 Como usar o Lighthouse

1. Com o DevTools aberto, vá até a aba **“Lighthouse”**
2. Selecione as opções desejadas: `Performance`, `Accessibility`, `Best Practices`, `SEO`
3. Clique em **Generate report**

### 📊 Interpretação dos Resultados

- Pontuações de 0 a 100 para cada categoria
- Sugestões de melhorias com links para documentação
- Diagnóstico sobre tempo de carregamento, legibilidade e uso de viewport

### 🧪 Atividade Proposta

Rode uma auditoria Lighthouse em um site próprio e corrija pelo menos 2 pontos sinalizados no relatório.

---

## 📗 Aula 7.3 – Frameworks Auxiliares (Bootstrap e Tailwind)

### 🎯 Objetivo da Aula

Conhecer frameworks CSS que aceleram a criação de layouts responsivos e consistentes.

### 🔧 Bootstrap

- Classes pré-definidas para grid, espaçamento e componentes
- Responsividade com breakpoints como `col-md`, `d-none`, `d-sm-block`
- Sistema de 12 colunas com `row` e `col`

```html
<div class="row">
  <div class="col-md-6">Coluna 1</div>
  <div class="col-md-6">Coluna 2</div>
</div>
```

### 🎨 Tailwind CSS

- Utiliza utilitários como `p-4`, `grid-cols-2`, `md:hidden`
- Customização direta na marcação HTML

```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-4">
  <div class="bg-blue-300 p-4">Bloco 1</div>
  <div class="bg-blue-300 p-4">Bloco 2</div>
</div>
```

### ✅ Comparativo Rápido

| Critério     | Bootstrap            | Tailwind CSS             |
| ------------ | -------------------- | ------------------------ |
| Facilidade   | Mais amigável        | Requer prática           |
| Customização | Limitada via classes | Altamente personalizável |
| Estilo base  | Opinionado           | Minimalista              |

### 🧪 Atividade Proposta

Refatore uma seção do seu site usando **Bootstrap** ou **Tailwind**. Compare o tempo de desenvolvimento e legibilidade do código.

---

## 📌 Conclusão do Capítulo 7

- Testar seu layout é parte essencial do processo de responsividade
- Ferramentas como **DevTools** e **Lighthouse** ajudam a identificar problemas reais
- **Frameworks CSS** podem agilizar muito a prototipação e desenvolvimento

### 🧠 Checklist Rápido

-

### 📎 Próximo Capítulo:

➡️ Capítulo 8 – Desafios Práticos

