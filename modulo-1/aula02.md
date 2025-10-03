# SGSA — **Design Tokens** (Guia para Aula 2)

> **Objetivo:** padronizar **cores, tipografia, espaçamentos, bordas e estados** do SGSA para uso desde o protótipo até a integração com Bootstrap. Todos os códigos abaixo usam **a paleta oficial**.

---

## 1) Paleta Base (cores oficiais)

**Hex fornecidos:**

* `#420950` (roxo-escuro)
* `#380047` (roxo-profundo)
* `#682278` (roxo-base)
* `#9E67AD` (lilás)
* `#1E4E05` (verde)
* `#37234F` (roxo-secundário)

### 1.1 Variáveis CSS — escala e semântica

```css
:root {
  /* Escala de marca */
  --sgsa-purple-900: #380047; /* roxo-profundo */
  --sgsa-purple-800: #420950; /* roxo-escuro */
  --sgsa-purple-700: #37234F; /* roxo-secundário */
  --sgsa-purple-600: #682278; /* roxo-base */
  --sgsa-purple-400: #9E67AD; /* lilás (realce/suporte) */
  --sgsa-green-700:  #1E4E05; /* verde (êxito/destaque positivo) */

  /* Neutros (para fundos e textos) */
  --sgsa-black: #111111;
  --sgsa-gray-900: #1a1a1a;
  --sgsa-gray-800: #222222;
  --sgsa-gray-700: #2e2e2e;
  --sgsa-gray-600: #3a3a3a;
  --sgsa-gray-500: #5a5a5a;
  --sgsa-gray-300: #d2d2d2;
  --sgsa-gray-200: #e6e6e6;
  --sgsa-gray-100: #f3f3f3;
  --sgsa-white: #ffffff;

  /* Mapeamento semântico */
  --color-bg-app: var(--sgsa-purple-800);
  --color-surface: var(--sgsa-purple-700);
  --color-surface-alt: var(--sgsa-purple-600);
  --color-primary: var(--sgsa-purple-600);
  --color-primary-contrast: var(--sgsa-white);
  --color-secondary: var(--sgsa-purple-400);
  --color-secondary-contrast: var(--sgsa-black);
  --color-accent: var(--sgsa-green-700);
  --color-accent-contrast: var(--sgsa-white);
  --color-text: var(--sgsa-white);
  --color-text-muted: #e7dff0; /* texto secundário sobre roxo */
  --color-border: rgba(255,255,255,.16);
  --color-focus: #9E67AD; /* anel de foco visível */

  /* Estados (alertas) — derivados da paleta para manter unidade */
  --state-success: var(--sgsa-green-700);
  --state-info: var(--sgsa-purple-400);
  --state-warning: #ffd666; /* neutro quente para contraste */
  --state-danger: #ff6b6b;  /* vermelho de sistema, fora da marca */
}
```

> **Nota:** mantemos os alertas *warning/danger* fora da paleta roxa/verde para contraste e acessibilidade. Use-os com moderação.

### 1.2 Sobre contrastes

* Texto **sobre roxos**: prefira `#fff` (ou `--color-text`).
* Texto **sobre lilás (#9E67AD)**: usar **preto/near-black** (`--sgsa-black`) para leitura.
* Botões: `--color-primary` com texto `--color-primary-contrast`.
* Evite **verde sobre roxo** para texto; use verde apenas como **fundo de feedback** com texto branco.

---

## 2) Tipografia

### 2.1 Pilha de fontes (seguras e performáticas)

```css
:root {
  --font-sans: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, Arial, "Apple Color Emoji", "Segoe UI Emoji";
  --font-mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
}
```

### 2.2 Tamanhos e pesos (escala baseada em 16px)

```css
:root {
  --fs-2xl: 2rem;     /* 32px   títulos de página */
  --fs-xl: 1.5rem;    /* 24px   seções/headers   */
  --fs-lg: 1.25rem;   /* 20px   subtítulos       */
  --fs-md: 1rem;      /* 16px   texto padrão     */
  --fs-sm: 0.875rem;  /* 14px   notas/labels     */
  --fs-xs: 0.75rem;   /* 12px   meta/auxiliar    */

  --fw-regular: 400;
  --fw-medium: 500;
  --fw-semibold: 600;
  --fw-bold: 700;
}

body { font-family: var(--font-sans); font-size: var(--fs-md); line-height: 1.5; }
h1 { font-size: var(--fs-2xl); font-weight: var(--fw-bold); }
h2 { font-size: var(--fs-xl);  font-weight: var(--fw-semibold); }
h3 { font-size: var(--fs-lg);  font-weight: var(--fw-semibold); }
```

> **A11y:** mantenha contraste ≥ 4.5:1 e não use peso leve para textos pequenos.

---

## 3) Espaçamentos, bordas e sombras

```css
:root {
  /* Grid de espaçamento (4px base) */
  --sp-0: 0;
  --sp-1: 0.25rem;  /* 4px  */
  --sp-2: 0.5rem;   /* 8px  */
  --sp-3: 0.75rem;  /* 12px */
  --sp-4: 1rem;     /* 16px */
  --sp-5: 1.5rem;   /* 24px */
  --sp-6: 2rem;     /* 32px */
  --sp-8: 3rem;     /* 48px */

  /* Raios de borda */
  --radius-sm: 6px;
  --radius-md: 10px;
  --radius-lg: 14px;

  /* Borda e foco */
  --border: 1px solid var(--color-border);
  --focus-ring: 0 0 0 3px rgba(158,103,173,.55); /* baseado no lilás */

  /* Sombras sutis, pensadas para fundo escuro */
  --shadow-1: 0 1px 2px rgba(0,0,0,.18);
  --shadow-2: 0 6px 16px rgba(0,0,0,.24);
}
```

---

## 4) Componentes base (tokens aplicados)

### 4.1 Cartão (card)

```css
.sgsa-card {
  background: var(--color-surface);
  color: var(--color-text);
  border: var(--border);
  border-radius: var(--radius-md);
  padding: var(--sp-4);
  box-shadow: var(--shadow-1);
}
.sgsa-card--alt { background: var(--color-surface-alt); }
```

### 4.2 Botões

```css
.btn-sgsa {
  display: inline-flex; align-items: center; justify-content: center;
  gap: var(--sp-2);
  padding: .625rem 1rem; /* 10x16 */
  border-radius: var(--radius-md);
  border: none;
  font-weight: var(--fw-semibold);
  cursor: pointer;
  outline: none;
}
.btn-sgsa:focus-visible { box-shadow: var(--focus-ring); }

.btn-primary   { background: var(--color-primary);   color: var(--color-primary-contrast); }
.btn-secondary { background: var(--color-secondary); color: var(--color-secondary-contrast); }
.btn-success   { background: var(--state-success);   color: var(--sgsa-white); }
.btn-ghost     { background: transparent; color: var(--color-text); border: 1px solid rgba(255,255,255,.24); }
.btn-ghost:hover { background: rgba(255,255,255,.06); }
```

### 4.3 Formulários

```css
.sgsa-field label { display:block; margin-bottom: var(--sp-2); font-size: var(--fs-sm); color: var(--color-text-muted); }
.sgsa-input {
  width: 100%;
  padding: .625rem .75rem;
  border-radius: var(--radius-sm);
  border: 1px solid rgba(255,255,255,.22);
  background: rgba(255,255,255,.06);
  color: var(--sgsa-white);
}
.sgsa-input::placeholder { color: rgba(255,255,255,.6); }
.sgsa-input:focus { outline: none; box-shadow: var(--focus-ring); border-color: transparent; }
```

### 4.4 KPIs (cards do Dashboard)

```css
.kpis { display:grid; gap: var(--sp-4); }
.kpi  { padding: var(--sp-4); background: var(--sgsa-purple-600); border-radius: var(--radius-md); text-align:center; }
.kpi--ok { background: var(--state-success); }
.kpi__value { font-size: var(--fs-xl); font-weight: var(--fw-bold); }
.kpi__label { font-size: var(--fs-sm); opacity:.9; }

@media (min-width: 768px){ .kpis{ grid-template-columns: repeat(2,1fr);} }
@media (min-width:1200px){ .kpis{ grid-template-columns: repeat(4,1fr);} }
```

---

## 5) Integração com **Bootstrap 5** (override seguro)

> Use **variáveis CSS** do Bootstrap para manter componentes nativos com a cara do SGSA.

```css
/* Em um arquivo overrides.css, importado DEPOIS do Bootstrap */
:root {
  --bs-body-bg: var(--color-bg-app);
  --bs-body-color: var(--color-text);
  --bs-border-color: var(--color-border);

  --bs-primary:      var(--color-primary);
  --bs-primary-rgb:  104,34,120; /* #682278 */
  --bs-secondary:    var(--color-secondary);
  --bs-success:      var(--state-success);
  --bs-info:         var(--state-info);
  --bs-warning:      var(--state-warning);
  --bs-danger:       var(--state-danger);

  --bs-link-color:   var(--color-secondary);
  --bs-link-hover-color: #b684c4;
  --bs-focus-ring-color: rgba(158,103,173,.35);
  --bs-border-radius: var(--radius-md);
}

.btn-primary { color: var(--color-primary-contrast); }
```

**Como usar:**

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css">
<link rel="stylesheet" href="/assets/css/overrides.css"> <!-- depois do Bootstrap -->
```

---

## 6) Exemplo completo (trecho HTML)

```html
<header class="py-3" style="background: var(--sgsa-purple-800);">
  <div class="container d-flex justify-content-between align-items-center">
    <h1 class="m-0" style="font-size: var(--fs-lg);">SGSA</h1>
    <button class="btn-sgsa btn-ghost">Sair</button>
  </div>
</header>

<main class="container my-4">
  <div class="kpis">
    <div class="kpi"><div class="kpi__value">12</div><div class="kpi__label">Turmas</div></div>
    <div class="kpi"><div class="kpi__value">384</div><div class="kpi__label">Alunos</div></div>
    <div class="kpi"><div class="kpi__value">21</div><div class="kpi__label">Ocorrências</div></div>
    <div class="kpi kpi--ok"><div class="kpi__value">93%</div><div class="kpi__label">Frequência</div></div>
  </div>

  <div class="sgsa-card mt-4">
    <h2 class="mb-3">Nova Tarefa</h2>
    <div class="sgsa-field mb-3">
      <label for="t">Título</label>
      <input id="t" class="sgsa-input" placeholder="Ex.: Lista de exercícios 02">
    </div>
    <button class="btn-sgsa btn-primary">Salvar</button>
  </div>
</main>
```

---

## 7) Checklist de Qualidade

* [ ] Todas as cores usadas existem nas variáveis declaradas.
* [ ] Contraste de texto ≥ 4.5:1 (texto principal) — *evitar verde como cor de texto sobre roxo*.
* [ ] Foco visível (ring lilás) em links, botões e campos.
* [ ] Espaçamentos seguem a escala de 4px.
* [ ] Raios de borda consistentes (sm/md/lg).
* [ ] Overrides do Bootstrap carregados após o CSS do framework.

---

## 8) Boas práticas e armadilhas

* **Consistência > variedade**: evite criar novos tons fora das variáveis.
* **Sem opacidade em textos** críticos (perde contraste); prefira tons sólidos adequados.
* **Estados**: não use lilás para erro (confunde com info); mantenha vermelho de sistema.
* **Acessibilidade**: tamanho mínimo de alvo 44×44, labels visíveis, `:focus-visible` preservado.

---

## 9) Próximos passos

* Criar `assets/css/overrides.css` no projeto e colar os tokens.
* Aplicar tokens nas páginas **Login** e **Dashboard** primeiro.
* Subir um *PR* inicial apenas com **design system** para revisão visual.
