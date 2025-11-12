---
theme: default
layout: cover
background: linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #24243e 100%)
title: Веб компоненты
info: |
   ## Веб компоненты в современной веб-разработке
   Подробная лекция о стандартах, применении и интеграции
transition: fade
---

# Веб компоненты

## Стандарты, применение и микрофронтенды

<div class="absolute bottom-10 left-10 opacity-80">
  <p class="text-sm">Лекция по веб-разработке • 2025</p>
</div>

<style>
h1 {
  background: linear-gradient(135deg, #00d4ff 0%, #7c3aed 50%, #ec4899 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: glow 3s ease-in-out infinite;
}

@keyframes glow {
  0%, 100% { filter: drop-shadow(0 0 20px rgba(0, 212, 255, 0.5)); }
  50% { filter: drop-shadow(0 0 40px rgba(124, 58, 237, 0.5)); }
}
</style>

---
layout: intro
---

# Содержание лекции

<div class="space-y-3 pb-6">
  <div v-click class="flex items-center gap-3 p-2 rounded-lg bg-gradient-to-r from-cyan-500/20 to-blue-500/20 hover:from-cyan-500/30 hover:to-blue-500/30 transition-all duration-300 transform hover:scale-105">
    <span class="text-xl">📚</span>
    <span class="text-sm">Что такое веб компоненты?</span>
  </div>
  <div v-click class="flex items-center gap-3 p-2 rounded-lg bg-gradient-to-r from-purple-500/20 to-pink-500/20 hover:from-purple-500/30 hover:to-pink-500/30 transition-all duration-300 transform hover:scale-105">
    <span class="text-xl">⚙️</span>
    <span class="text-sm">Основные технологии и стандарты</span>
  </div>
  <div v-click class="flex items-center gap-3 p-2 rounded-lg bg-gradient-to-r from-blue-500/20 to-cyan-500/20 hover:from-blue-500/30 hover:to-cyan-500/30 transition-all duration-300 transform hover:scale-105">
    <span class="text-xl">🛠️</span>
    <span class="text-sm">Практическое применение</span>
  </div>
  <div v-click class="flex items-center gap-3 p-2 rounded-lg bg-gradient-to-r from-indigo-500/20 to-purple-500/20 hover:from-indigo-500/30 hover:to-purple-500/30 transition-all duration-300 transform hover:scale-105">
    <span class="text-xl">🏗️</span>
    <span class="text-sm">Веб компоненты в микрофронтенде</span>
  </div>
  <div v-click class="flex items-center gap-3 p-2 rounded-lg bg-gradient-to-r from-pink-500/20 to-rose-500/20 hover:from-pink-500/30 hover:to-rose-500/30 transition-all duration-300 transform hover:scale-105">
    <span class="text-xl">🅰️</span>
    <span class="text-sm">Интеграция с Angular</span>
  </div>
  <div v-click class="flex items-center gap-3 p-2 rounded-lg bg-gradient-to-r from-amber-500/20 to-orange-500/20 hover:from-amber-500/30 hover:to-orange-500/30 transition-all duration-300 transform hover:scale-105">
    <span class="text-xl">✨</span>
    <span class="text-sm">Лучшие практики и паттерны</span>
  </div>
</div>

<style>
.dark {
  background: linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #24243e 100%);
}
</style>

---
layout: section
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%)
---

# Введение в веб компоненты

---

# Определение веб компонентов

<div class="grid grid-cols-2 gap-6 pt-2">

<div v-motion :initial="{ opacity: 0, x: -50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

## Что это?

Веб компоненты — это набор **веб-стандартов**, позволяющих создавать:

- Переиспользуемые компоненты
- Инкапсулированные функциональность и стили
- Независимые от фреймворка элементы
- Стандартный DOM API

</div>

<div v-motion :initial="{ opacity: 0, x: 50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }" class="bg-gradient-to-br from-cyan-500/20 via-purple-500/20 to-pink-500/20 p-6 rounded-2xl border border-purple-500/30 backdrop-blur-sm">

## Ключевые преимущества

<div class="space-y-2 text-sm">
  <div class="flex items-center gap-2">
    <span class="text-lg">✨</span>
    <span><strong>Инкапсуляция</strong> — изоляция стилей</span>
  </div>
  <div class="flex items-center gap-2">
    <span class="text-lg">🔄</span>
    <span><strong>Переиспользуемость</strong> — везде</span>
  </div>
  <div class="flex items-center gap-2">
    <span class="text-lg">🚀</span>
    <span><strong>Производительность</strong> — нативно</span>
  </div>
  <div class="flex items-center gap-2">
    <span class="text-lg">🛠️</span>
    <span><strong>Стандартизация</strong> — W3C</span>
  </div>
  <div class="flex items-center gap-2">
    <span class="text-lg">🎯</span>
    <span><strong>Framework-агностичность</strong></span>
  </div>
</div>

</div>

</div>

---

# История веб компонентов

<div class="space-y-4 pb-4">

<div v-click class="flex gap-4 items-start p-3 rounded-xl bg-gradient-to-r from-blue-500/20 to-cyan-500/20 hover:from-blue-500/30 hover:to-cyan-500/30 border-l-4 border-cyan-500 transition-all duration-300 transform hover:translate-x-2">
  <div class="text-2xl font-bold text-cyan-400 min-w-16">2011</div>
  <div class="text-sm">
    <strong>Первые идеи</strong>
    <p class="opacity-80">Алекс Рассель предложил концепцию компонентизации веб</p>
  </div>
</div>

<div v-click class="flex gap-4 items-start p-3 rounded-xl bg-gradient-to-r from-purple-500/20 to-pink-500/20 hover:from-purple-500/30 hover:to-pink-500/30 border-l-4 border-pink-500 transition-all duration-300 transform hover:translate-x-2">
  <div class="text-2xl font-bold text-pink-400 min-w-24">2013-2015</div>
  <div class="text-sm">
    <strong>Разработка стандартов</strong>
    <p class="opacity-80">Polymer от Google, создание спецификации W3C</p>
  </div>
</div>

<div v-click class="flex gap-4 items-start p-3 rounded-xl bg-gradient-to-r from-indigo-500/20 to-blue-500/20 hover:from-indigo-500/30 hover:to-blue-500/30 border-l-4 border-indigo-500 transition-all duration-300 transform hover:translate-x-2">
  <div class="text-2xl font-bold text-indigo-400 min-w-24">2016-2017</div>
  <div class="text-sm">
    <strong>Стабилизация</strong>
    <p class="opacity-80">Поддержка главными браузерами (Chrome, Firefox, Safari)</p>
  </div>
</div>

<div v-click class="flex gap-4 items-start p-3 rounded-xl bg-gradient-to-r from-emerald-500/20 to-cyan-500/20 hover:from-emerald-500/30 hover:to-cyan-500/30 border-l-4 border-emerald-500 transition-all duration-300 transform hover:translate-x-2">
  <div class="text-2xl font-bold text-emerald-400 min-w-16">2020+</div>
  <div class="text-sm">
    <strong>Массовое использование</strong>
    <p class="opacity-80">Интеграция в фреймворки, микрофронтенды, дизайн системы</p>
  </div>
</div>

</div>

---
layout: section
background: linear-gradient(135deg, #00d4ff 0%, #7c3aed 50%, #ec4899 100%)
---

# Технологические основы

---

# Четыре столпа веб компонентов

<div class="grid grid-cols-2 gap-4 pt-2">

<div v-motion :initial="{ opacity: 0, y: 50 }" :enter="{ opacity: 1, y: 0, transition: { duration: 500, delay: 0 } }" class="group relative overflow-hidden rounded-2xl p-5 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-cyan-500/30 hover:border-cyan-400 transition-all duration-300 hover:shadow-lg hover:shadow-cyan-500/20">
  <div class="absolute inset-0 bg-gradient-to-br from-cyan-500/10 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="text-lg font-bold mb-2 text-cyan-400">🏷️ Custom Elements</h3>
    <p class="text-xs opacity-90 mb-3">API для определения собственных HTML элементов</p>
    <div class="bg-slate-950 p-2 rounded font-mono text-xs text-cyan-300 border border-cyan-500/20">customElements.define(...)</div>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, y: 50 }" :enter="{ opacity: 1, y: 0, transition: { duration: 500, delay: 100 } }" class="group relative overflow-hidden rounded-2xl p-5 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-purple-500/30 hover:border-purple-400 transition-all duration-300 hover:shadow-lg hover:shadow-purple-500/20">
  <div class="absolute inset-0 bg-gradient-to-br from-purple-500/10 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="text-lg font-bold mb-2 text-purple-400">👁️ Shadow DOM</h3>
    <p class="text-xs opacity-90 mb-3">Инкапсуляция DOM структуры и стилей</p>
    <div class="bg-slate-950 p-2 rounded font-mono text-xs text-purple-300 border border-purple-500/20">attachShadow({...})</div>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, y: 50 }" :enter="{ opacity: 1, y: 0, transition: { duration: 500, delay: 200 } }" class="group relative overflow-hidden rounded-2xl p-5 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-pink-500/30 hover:border-pink-400 transition-all duration-300 hover:shadow-lg hover:shadow-pink-500/20">
  <div class="absolute inset-0 bg-gradient-to-br from-pink-500/10 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="text-lg font-bold mb-2 text-pink-400">📝 HTML Templates</h3>
    <p class="text-xs opacity-90 mb-3">Переиспользуемые шаблоны, не рендерятся</p>
    <div class="bg-slate-950 p-2 rounded font-mono text-xs text-pink-300 border border-pink-500/20">&lt;template&gt;...&lt;/template&gt;</div>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, y: 50 }" :enter="{ opacity: 1, y: 0, transition: { duration: 500, delay: 300 } }" class="group relative overflow-hidden rounded-2xl p-5 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-amber-500/30 hover:border-amber-400 transition-all duration-300 hover:shadow-lg hover:shadow-amber-500/20">
  <div class="absolute inset-0 bg-gradient-to-br from-amber-500/10 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="text-lg font-bold mb-2 text-amber-400">🔌 ES Modules</h3>
    <p class="text-xs opacity-90 mb-3">Модульная загрузка компонентов</p>
    <div class="bg-slate-950 p-2 rounded font-mono text-xs text-amber-300 border border-amber-500/20">import '...'</div>
  </div>
</div>

</div>

---

# Custom Elements API

<div class="max-h-[420px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-cyan-500/30 p-5 hover:border-cyan-400/50 transition-all duration-300">

```javascript
class MyButton extends HTMLElement {
  constructor() {
    super();
    this.attachShadow({ mode: 'open' });
  }

  connectedCallback() {
    this.render();
  }

  disconnectedCallback() {
    // Вызывается при удалении из DOM
  }

  attributeChangedCallback(name, oldValue, newValue) {
    if (name === 'disabled') {
      this.updateState();
    }
  }

  static get observedAttributes() {
    return ['disabled', 'label'];
  }

  render() {
    this.shadowRoot.innerHTML = `
      <style>
        button {
          padding: 10px 20px;
          background: linear-gradient(135deg, #00d4ff, #7c3aed);
          border-radius: 8px;
          cursor: pointer;
        }
      </style>
      <button>${this.getAttribute('label') || 'Click me'}</button>
    `;
  }
}

customElements.define('my-button', MyButton);
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #00d4ff, #7c3aed);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #7c3aed, #ec4899);
}
</style>

---

# Shadow DOM: Инкапсуляция

<div class="grid grid-cols-3 gap-4 pt-2">

<div v-motion :initial="{ opacity: 0, x: -50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

## Shadow Root структура

<div class="max-h-[340px] overflow-y-auto rounded-lg bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-purple-500/30 p-3 mt-3">

```html
<!-- Внешний DOM -->
<my-card>
  <!-- Shadow root -->
  #shadow-root
    <style>
      :host { display: block; }
      .card {
        background: linear-gradient(
          135deg,
          #667eea,
          #764ba2
        );
      }
    </style>
    <div class="card">
      <slot></slot>
    </div>
</my-card>
```

</div>

</div>

<div v-motion :initial="{ opacity: 0, x: 50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

## Режимы Shadow DOM

<div class="space-y-3">
  <div class="p-3 rounded-lg bg-gradient-to-r from-cyan-500/20 to-blue-500/20 border border-cyan-500/30">
    <div class="font-bold text-xs text-cyan-300 mb-1">open</div>
    <p class="text-xs opacity-80">JS имеет доступ к shadowRoot</p>
  </div>

  <div class="p-3 rounded-lg bg-gradient-to-r from-purple-500/20 to-pink-500/20 border border-purple-500/30">
    <div class="font-bold text-xs text-pink-300 mb-1">closed</div>
    <p class="text-xs opacity-80">Скрыт от внешнего JavaScript</p>
  </div>

  <div class="p-3 rounded-lg bg-gradient-to-r from-amber-500/20 to-orange-500/20 border border-amber-500/30">
    <div class="font-bold text-xs text-amber-300 mb-1">delegatesFocus</div>
    <p class="text-xs opacity-80">Фокус делегируется элементам</p>
  </div>
</div>
</div>
<div v-motion :initial="{ opacity: 0, x: 50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

## Изоляция

<div class="mt-3 space-y-1 text-xs">
  <div class="flex items-center gap-2">
    <span class="text-cyan-400">✅</span>
    <span>Стили не влияют на родителя</span>
  </div>
  <div class="flex items-center gap-2">
    <span class="text-cyan-400">✅</span>
    <span>Глобальные стили не влияют</span>
  </div>
  <div class="flex items-center gap-2">
    <span class="text-cyan-300">✅</span>
    <span>CSS переменные для кастомизации</span>
  </div>
</div>

</div>

</div>

<style>
::-webkit-scrollbar {
  width: 6px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
}

::-webkit-scrollbar-thumb {
  background: rgba(124, 58, 237, 0.4);
  border-radius: 3px;
}

::-webkit-scrollbar-thumb:hover {
  background: rgba(124, 58, 237, 0.7);
}
</style>

---

# HTML Templates и Slots

<div class="text-xs pb-3">

## Что такое Template и Slot?

<div class="grid grid-cols-2 gap-4 mb-4">
  <div class="p-3 rounded-lg bg-gradient-to-r from-cyan-500/20 to-blue-500/20 border border-cyan-500/30">
    <strong class="text-cyan-300">Template</strong>
    <p class="text-xs opacity-80 mt-1">Блок HTML кода, который не отображается при загрузке страницы. Используется для многократного клонирования.</p>
  </div>
  <div class="p-3 rounded-lg bg-gradient-to-r from-purple-500/20 to-pink-500/20 border border-purple-500/30">
    <strong class="text-pink-300">Slot</strong>
    <p class="text-xs opacity-80 mt-1">Точка «вставки» внутри Shadow DOM, куда помещается содержимое из Light DOM (HTML внутри компонента).</p>
  </div>
</div>

## Как они используются в веб компонентах?

<div class="p-3 rounded-lg bg-gradient-to-r from-emerald-500/20 to-cyan-500/20 border border-emerald-500/30 mb-3">
  <p class="text-xs opacity-90"><strong>Template</strong> определяет структуру компонента один раз, а <strong>Slot</strong> позволяет передать кастомный контент внутрь компонента. Вместе они создают гибкую и переиспользуемую архитектуру.</p>
</div>
</div>

--- 

<div class="text-xs pb-3">
## Пример связи Template → Slot → Компонент

</div>

<div class="max-h-[330px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-pink-500/30 p-4 hover:border-pink-400/50 transition-all duration-300">

```html
<!-- ШАБЛОН: Определяется один раз -->
<template id="card-template">
  <style>
    .card { padding: 1.5rem; border-radius: 12px; }
    .header { font-weight: bold; margin-bottom: 0.5rem; }
    .content { color: rgba(255,255,255,0.8); }
    .footer { margin-top: 1rem; border-top: 1px solid rgba(255,255,255,0.1); }
  </style>
  <div class="card">
    <div class="header">
      <!-- SLOT 1: Место для заголовка -->
      <slot name="title">Default Title</slot>
    </div>
    <div class="content">
      <!-- SLOT 2: Место для основного контента -->
      <slot>Default content</slot>
    </div>
    <div class="footer">
      <!-- SLOT 3: Место для кнопок действий -->
      <slot name="actions"></slot>
    </div>
  </div>
</template>

<!-- ИСПОЛЬЗОВАНИЕ: Передаём кастомный контент через slots -->
<my-card>
  <h2 slot="title">Заголовок карточки</h2>
  <p>Содержимое карточки с описанием</p>
  <button slot="actions">Действие</button>
</my-card>

<!-- РЕЗУЛЬТАТ: Light DOM контент вставляется в соответствующие слоты -->
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #ec4899, #7c3aed);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #00d4ff, #ec4899);
}
</style>

---

# Жизненный цикл компонента

<div class="space-y-3 pb-4">
  <div v-click class="flex items-start gap-3 p-3 rounded-lg bg-gradient-to-r from-cyan-500/20 to-blue-500/20 border-l-4 border-cyan-500 hover:shadow-lg hover:shadow-cyan-500/20 transition-all duration-300">
    <div class="text-2xl min-w-12">①</div>
    <div class="text-sm">
      <h3 class="font-bold text-cyan-300">constructor()</h3>
      <p class="opacity-80">Инициализация свойств, создание Shadow DOM</p>
    </div>
  </div>

  <div v-click class="flex items-start gap-3 p-3 rounded-lg bg-gradient-to-r from-purple-500/20 to-pink-500/20 border-l-4 border-purple-500 hover:shadow-lg hover:shadow-purple-500/20 transition-all duration-300">
    <div class="text-2xl min-w-12">②</div>
    <div class="text-sm">
      <h3 class="font-bold text-purple-300">connectedCallback()</h3>
      <p class="opacity-80">Добавлен в DOM, начальный рендер, добавление слушателей</p>
    </div>
  </div>

  <div v-click class="flex items-start gap-3 p-3 rounded-lg bg-gradient-to-r from-indigo-500/20 to-blue-500/20 border-l-4 border-indigo-500 hover:shadow-lg hover:shadow-indigo-500/20 transition-all duration-300">
    <div class="text-2xl min-w-12">③</div>
    <div class="text-sm">
      <h3 class="font-bold text-indigo-300">attributeChangedCallback()</h3>
      <p class="opacity-80">При изменении наблюдаемого атрибута</p>
    </div>
  </div>

  <div v-click class="flex items-start gap-3 p-3 rounded-lg bg-gradient-to-r from-emerald-500/20 to-cyan-500/20 border-l-4 border-emerald-500 hover:shadow-lg hover:shadow-emerald-500/20 transition-all duration-300">
    <div class="text-2xl min-w-12">④</div>
    <div class="text-sm">
      <h3 class="font-bold text-emerald-300">disconnectedCallback()</h3>
      <p class="opacity-80">Удален из DOM, очистка ресурсов, удаление слушателей</p>
    </div>
  </div>
</div>

---
layout: section
background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%)
---

# Практическое применение

---

# Пример: Компонент рейтинга

<div class="max-h-[400px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-amber-500/30 p-5 hover:border-amber-400/50 transition-all duration-300">

```javascript
class StarRating extends HTMLElement {
  constructor() {
    super();
    this.attachShadow({ mode: 'open' });
    this.rating = 0;
  }

  connectedCallback() {
    this.render();
    this.setupEventListeners();
  }

  render() {
    const rating = this.getAttribute('rating') || 0;
    const stars = Array(5).fill(0).map((_, i) =>
      `<span class="star ${i < rating ? 'filled' : ''}">${i < rating ? '★' : '☆'}</span>`
    ).join('');

    this.shadowRoot.innerHTML = `
      <style>
        .stars { display: flex; gap: 8px; font-size: 2.5rem; }
        .star { cursor: pointer; transition: all 0.3s ease; color: rgba(255, 193, 7, 0.3); }
        .star:hover { color: #ffc107; transform: scale(1.1); }
        .star.filled { color: #ffc107; }
      </style>
      <div class="stars">${stars}</div>
    `;
  }

  setupEventListeners() {
    this.shadowRoot.querySelectorAll('.star').forEach((star, index) => {
      star.addEventListener('click', () => {
        this.rating = index + 1;
        this.setAttribute('rating', this.rating);
        this.dispatchEvent(new CustomEvent('rating-changed', {
          detail: { rating: this.rating }
        }));
        this.render();
      });
    });
  }

  static get observedAttributes() {
    return ['rating'];
  }

  attributeChangedCallback() {
    this.render();
  }
}

customElements.define('star-rating', StarRating);
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #ffc107, #ff9800);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #ffb74d, #ffb74d);
}
</style>

---

# Использование компонента рейтинга

<div class="max-h-[400px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-lime-500/30 p-5 hover:border-lime-400/50 transition-all duration-300">

```html
<!DOCTYPE html>
<html>
<head>
  <script src="star-rating.js"></script>
  <style>
    body {
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      color: white;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      padding: 2rem;
    }
    h1 {
      background: linear-gradient(135deg, #00d4ff, #7c3aed);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    .container {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.1);
      border-radius: 16px;
      padding: 2rem;
      max-width: 400px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>🎬 Оцените фильм</h1>

    <star-rating rating="3"></star-rating>

    <script>
      const rating = document.querySelector('star-rating');

      rating.addEventListener('rating-changed', (e) => {
        console.log('Новый рейтинг:', e.detail.rating);
        fetch('/api/rate', {
          method: 'POST',
          headers: { 'Content-Type': 'application/json' },
          body: JSON.stringify({ rating: e.detail.rating })
        });
      });
    </script>
  </div>
</body>
</html>
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #84cc16, #65a30d);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #a3e635, #84cc16);
}
</style>

---

# Современные инструменты для веб компонентов

<div class="grid grid-cols-2 gap-4 pt-2">

<div v-motion :initial="{ opacity: 0, scale: 0.8 }" :enter="{ opacity: 1, scale: 1, transition: { duration: 500, delay: 0 } }" class="group relative overflow-hidden rounded-2xl p-4 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-purple-500/30 hover:border-purple-400 transition-all duration-300 hover:shadow-xl hover:shadow-purple-500/30">
  <div class="absolute inset-0 bg-gradient-to-br from-purple-500/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="font-bold text-sm mb-2 text-purple-300">📚 Lit</h3>
    <p class="text-xs mb-3">Минималистичная библиотека от Google</p>
    <ul class="space-y-1 text-xs">
      <li class="flex items-center gap-2"><span class="text-purple-400">→</span> Reactive properties</li>
      <li class="flex items-center gap-2"><span class="text-purple-400">→</span> HTML шаблоны</li>
      <li class="flex items-center gap-2"><span class="text-purple-400">→</span> Маленький размер</li>
    </ul>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, scale: 0.8 }" :enter="{ opacity: 1, scale: 1, transition: { duration: 500, delay: 100 } }" class="group relative overflow-hidden rounded-2xl p-4 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-cyan-500/30 hover:border-cyan-400 transition-all duration-300 hover:shadow-xl hover:shadow-cyan-500/30">
  <div class="absolute inset-0 bg-gradient-to-br from-cyan-500/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="font-bold text-sm mb-2 text-cyan-300">🔷 Polymer</h3>
    <p class="text-xs mb-3">Полнофункциональный фреймворк</p>
    <ul class="space-y-1 text-xs">
      <li class="flex items-center gap-2"><span class="text-cyan-400">→</span> Данные привязка</li>
      <li class="flex items-center gap-2"><span class="text-cyan-400">→</span> Маршрутизация</li>
      <li class="flex items-center gap-2"><span class="text-cyan-400">→</span> Большое сообщество</li>
    </ul>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, scale: 0.8 }" :enter="{ opacity: 1, scale: 1, transition: { duration: 500, delay: 200 } }" class="group relative overflow-hidden rounded-2xl p-4 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-pink-500/30 hover:border-pink-400 transition-all duration-300 hover:shadow-xl hover:shadow-pink-500/30">
  <div class="absolute inset-0 bg-gradient-to-br from-pink-500/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="font-bold text-sm mb-2 text-pink-300">🎨 Stencil</h3>
    <p class="text-xs mb-3">Компилятор от Ionic</p>
    <ul class="space-y-1 text-xs">
      <li class="flex items-center gap-2"><span class="text-pink-400">→</span> TypeScript</li>
      <li class="flex items-center gap-2"><span class="text-pink-400">→</span> JSX синтаксис</li>
      <li class="flex items-center gap-2"><span class="text-pink-400">→</span> Оптимизация сборки</li>
    </ul>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, scale: 0.8 }" :enter="{ opacity: 1, scale: 1, transition: { duration: 500, delay: 300 } }" class="group relative overflow-hidden rounded-2xl p-4 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-amber-500/30 hover:border-amber-400 transition-all duration-300 hover:shadow-xl hover:shadow-amber-500/30">
  <div class="absolute inset-0 bg-gradient-to-br from-amber-500/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="font-bold text-sm mb-2 text-amber-300">⚡ Hybrids</h3>
    <p class="text-xs mb-3">Легкий фреймворк</p>
    <ul class="space-y-1 text-xs">
      <li class="flex items-center gap-2"><span class="text-amber-400">→</span> Объектная модель</li>
      <li class="flex items-center gap-2"><span class="text-amber-400">→</span> Вычисляемые свойства</li>
      <li class="flex items-center gap-2"><span class="text-amber-400">→</span> Простота обучения</li>
    </ul>
  </div>
</div>

</div>

---

# Пример с Lit

<div class="max-h-[400px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-rose-500/30 p-5 hover:border-rose-400/50 transition-all duration-300">

```javascript
import { LitElement, html, css } from 'lit';

class CounterButton extends LitElement {
  static styles = css`
    button {
      padding: 12px 24px;
      font-size: 1rem;
      cursor: pointer;
      background: linear-gradient(135deg, #ec4899, #f43f5e);
      color: white;
      border: none;
      border-radius: 8px;
      font-weight: bold;
      transition: all 0.3s ease;
      box-shadow: 0 4px 15px rgba(244, 63, 94, 0.3);
    }

    button:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 25px rgba(244, 63, 94, 0.5);
    }
  `;

  static properties = {
    count: { type: Number }
  };

  constructor() {
    super();
    this.count = 0;
  }

  render() {
    return html`<button @click=${this.increment}>Нажато: ${this.count}</button>`;
  }

  increment() {
    this.count++;
    this.dispatchEvent(new CustomEvent('count-changed', {
      detail: { count: this.count }
    }));
  }
}

customElements.define('counter-button', CounterButton);
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #ec4899, #f43f5e);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #f43f5e, #fb7185);
}
</style>

---
layout: section
background: linear-gradient(135deg, #fa709a 0%, #fee140 100%)
---

# Веб компоненты в микрофронтенде

---

# Микрофронтенд архитектура

<div class="space-y-4 pb-4">
  <div v-motion :initial="{ opacity: 0, y: 50 }" :enter="{ opacity: 1, y: 0, transition: { duration: 600 } }" class="p-4 rounded-xl bg-gradient-to-r from-amber-500/20 to-yellow-500/20 border border-amber-500/30">
    <div class="font-bold text-sm text-amber-300 mb-1">🏢 Shell Application</div>
    <p class="text-xs">Container / Orchestrator</p>
  </div>

  <div class="grid grid-cols-3 gap-3">
    <div v-click class="p-3 rounded-lg bg-gradient-to-br from-cyan-500/20 to-blue-500/20 border border-cyan-500/30 hover:shadow-lg hover:shadow-cyan-500/20 transition-all duration-300 transform hover:scale-105">
      <div class="text-xl mb-1">📝</div>
      <div class="font-bold text-xs text-cyan-300">MFE 1</div>
      <p class="text-xs opacity-80">Header</p>
    </div>
    <div v-click class="p-3 rounded-lg bg-gradient-to-br from-purple-500/20 to-pink-500/20 border border-purple-500/30 hover:shadow-lg hover:shadow-purple-500/20 transition-all duration-300 transform hover:scale-105">
      <div class="text-xl mb-1">📋</div>
      <div class="font-bold text-xs text-purple-300">MFE 2</div>
      <p class="text-xs opacity-80">Sidebar</p>
    </div>
    <div v-click class="p-3 rounded-lg bg-gradient-to-br from-emerald-500/20 to-cyan-500/20 border border-emerald-500/30 hover:shadow-lg hover:shadow-emerald-500/20 transition-all duration-300 transform hover:scale-105">
      <div class="text-xl mb-1">📄</div>
      <div class="font-bold text-xs text-emerald-300">MFE 3</div>
      <p class="text-xs opacity-80">Content</p>
    </div>
  </div>

  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { duration: 800 } }" class="p-3 text-center rounded-lg bg-gradient-to-r from-pink-500/10 to-rose-500/10 border border-pink-500/20">
    <p class="text-xs text-pink-300">🔌 Все компоненты используют Web Components API</p>
  </div>
</div>

---

# Преимущества веб компонентов в микрофронтенде

<div class="grid grid-cols-2 gap-4 pb-4">

<div v-motion :initial="{ opacity: 0, x: -50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

<h4 class="text-xs font-bold mb-3 text-cyan-300">🎯 Технические преимущества</h4>

<div class="space-y-2">
  <div class="p-2 rounded-lg bg-cyan-500/10 border-l-4 border-cyan-500 text-xs">
    <div class="font-semibold">Framework-независимость</div>
    <p class="opacity-80 text-xs">Каждый MFE может использовать свой фреймворк</p>
  </div>

  <div class="p-2 rounded-lg bg-cyan-500/10 border-l-4 border-cyan-500 text-xs">
    <div class="font-semibold">Загрузка по требованию</div>
    <p class="opacity-80 text-xs">Динамическая загрузка компонентов</p>
  </div>

  <div class="p-2 rounded-lg bg-cyan-500/10 border-l-4 border-cyan-500 text-xs">
    <div class="font-semibold">Версионирование</div>
    <p class="opacity-80 text-xs">Разные версии одновременно</p>
  </div>

  <div class="p-2 rounded-lg bg-cyan-500/10 border-l-4 border-cyan-500 text-xs">
    <div class="font-semibold">Полная инкапсуляция</div>
    <p class="opacity-80 text-xs">Отсутствие конфликтов стилей</p>
  </div>
</div>

</div>

<div v-motion :initial="{ opacity: 0, x: 50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

<h4 class="text-xs font-bold mb-3 text-purple-300">🏢 Организационные преимущества</h4>

<div class="space-y-2">
  <div class="p-2 rounded-lg bg-purple-500/10 border-l-4 border-purple-500 text-xs">
    <div class="font-semibold">Независимые команды</div>
    <p class="opacity-80 text-xs">Разработка в разных командах</p>
  </div>

  <div class="p-2 rounded-lg bg-purple-500/10 border-l-4 border-purple-500 text-xs">
    <div class="font-semibold">Независимое развёртывание</div>
    <p class="opacity-80 text-xs">Обновление без синхронизации</p>
  </div>

  <div class="p-2 rounded-lg bg-purple-500/10 border-l-4 border-purple-500 text-xs">
    <div class="font-semibold">Переиспользование</div>
    <p class="opacity-80 text-xs">Компоненты везде</p>
  </div>

  <div class="p-2 rounded-lg bg-purple-500/10 border-l-4 border-purple-500 text-xs">
    <div class="font-semibold">Масштабируемость</div>
    <p class="opacity-80 text-xs">Добавление новых MFE</p>
  </div>
</div>

</div>

</div>

<style>
::-webkit-scrollbar {
  width: 6px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 3px;
}

::-webkit-scrollbar-thumb {
  background: rgba(96, 125, 237, 0.4);
  border-radius: 3px;
}

::-webkit-scrollbar-thumb:hover {
  background: rgba(96, 125, 237, 0.7);
}
</style>

---

# Паттерн: Host приложение

<div class="max-h-[400px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-indigo-500/30 p-5 hover:border-indigo-400/50 transition-all duration-300">

```javascript
// shell-app.js
class ShellApp extends HTMLElement {
  async connectedCallback() {
    this.setupEventBus();
    await this.loadMicroFrontends();
  }

  setupEventBus() {
    this.eventBus = new EventTarget();
    window.appEventBus = this.eventBus;
  }

  async loadMicroFrontends() {
    const mfes = [
      { name: 'header-mfe', url: '/mfe/header/index.js' },
      { name: 'sidebar-mfe', url: '/mfe/sidebar/index.js' },
      { name: 'content-mfe', url: '/mfe/content/index.js' }
    ];

    for (const mfe of mfes) {
      try {
        await import(mfe.url);
        const container = document.createElement('div');
        container.id = mfe.name;
        const component = document.createElement(mfe.name);
        container.appendChild(component);
        this.appendChild(container);
      } catch (error) {
        console.error(`Failed to load ${mfe.name}:`, error);
      }
    }
  }
}

customElements.define('shell-app', ShellApp);
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #6366f1, #4f46e5);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #4f46e5, #4338ca);
}
</style>

---

# Коммуникация между MFE

<div class="grid grid-cols-2 gap-4 pb-4">

<div>

<h3 class="text-sm font-bold mb-3 text-cyan-300">1️⃣ Event Bus паттерн</h3>

<div class="max-h-[330px] overflow-y-auto rounded-lg bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-cyan-500/30 p-3">

```javascript
// MFE 1 публикует
window.appEventBus
  .dispatchEvent(
    new CustomEvent(
      'user-logged-in',
      {
        detail: {
          userId: 123
        }
      }
    )
  );

// MFE 2 слушает
window.appEventBus
  .addEventListener(
    'user-logged-in',
    (e) => {
      console.log('User:', e.detail);
      this.updateUI(e.detail);
    }
  );
```

</div>

</div>

<div>

<h3 class="text-sm font-bold mb-3 text-purple-300">2️⃣ Message Passing паттерн</h3>

<div class="max-h-[330px] overflow-y-auto rounded-lg bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-purple-500/30 p-3">

```javascript
// MFE отправляет
window.parent.postMessage(
  {
    type: 'MFE_ACTION',
    data: {
      action: 'update-cart',
      item: { id: 1 }
    }
  },
  '*'
);

// Shell приложение
window.addEventListener(
  'message',
  (e) => {
    if (e.data.type === 'MFE_ACTION') {
      this.handleMFEAction(
        e.data
      );
    }
  }
);
```

</div>

</div>

</div>

<style>
::-webkit-scrollbar {
  width: 6px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 3px;
}

::-webkit-scrollbar-thumb {
  background: rgba(96, 125, 237, 0.4);
  border-radius: 3px;
}

::-webkit-scrollbar-thumb:hover {
  background: rgba(96, 125, 237, 0.7);
}
</style>

---
layout: section
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%)
---

# Веб компоненты в Angular

---

# Angular и веб компоненты

<div class="space-y-4 pb-4">

<p class="text-sm">Angular имеет <strong class="text-cyan-300">встроенную поддержку</strong> веб компонентов на двух уровнях:</p>

<div class="grid grid-cols-2 gap-4">

<div v-motion :initial="{ opacity: 0, scale: 0.8 }" :enter="{ opacity: 1, scale: 1, transition: { duration: 500 } }" class="group relative overflow-hidden rounded-2xl p-4 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-cyan-500/30 hover:border-cyan-400 transition-all duration-300 hover:shadow-xl hover:shadow-cyan-500/30">
  <div class="absolute inset-0 bg-gradient-to-br from-cyan-500/10 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="font-bold text-sm mb-2 text-cyan-300">📦 Использование веб компонентов</h3>
    <p class="text-xs mb-3">Импорт сторонних веб компонентов в Angular приложение</p>
    <div class="bg-slate-950 p-2 rounded font-mono text-xs text-cyan-300 border border-cyan-500/20">CUSTOM_ELEMENTS_SCHEMA</div>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, scale: 0.8 }" :enter="{ opacity: 1, scale: 1, transition: { duration: 500, delay: 200 } }" class="group relative overflow-hidden rounded-2xl p-4 bg-gradient-to-br from-slate-800 via-slate-900 to-slate-950 border border-purple-500/30 hover:border-purple-400 transition-all duration-300 hover:shadow-xl hover:shadow-purple-500/30">
  <div class="absolute inset-0 bg-gradient-to-br from-purple-500/10 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
  <div class="relative z-10">
    <h3 class="font-bold text-sm mb-2 text-purple-300">🏗️ Создание веб компонентов</h3>
    <p class="text-xs mb-3">Экспорт Angular компонентов как веб компонентов</p>
    <div class="bg-slate-950 p-2 rounded font-mono text-xs text-purple-300 border border-purple-500/20">@angular/elements</div>
  </div>
</div>

</div>

</div>

---

# Angular @angular/elements

<div class="max-h-[320px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-emerald-500/30 p-5 hover:border-emerald-400/50 transition-all duration-300">

```typescript
import { NgModule, Injector } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { createCustomElement } from '@angular/elements';

import { MyCardComponent } from './my-card.component';

@NgModule({
  imports: [BrowserModule],
  declarations: [MyCardComponent],
  entryComponents: [MyCardComponent] // Angular 11 и ниже
})
export class AppModule {
  constructor(private injector: Injector) {}

  ngDoBootstrap() {
    // Конвертирование Angular компонента в веб компонент
    const customElement = createCustomElement(
      MyCardComponent,
      { injector: this.injector }
    );

    customElements.define('my-card', customElement);
    console.log('✅ my-card компонент зарегистрирован');
  }
}

// Результат: Angular компонент становится обычным HTML элементом
// <my-card title="Заголовок"></my-card>
```

</div>

<div class="mt-2 p-3 rounded-lg bg-gradient-to-r from-emerald-500/20 to-cyan-500/20 border border-emerald-500/30 text-xs">
  <strong class="text-emerald-300">✅ Результат:</strong>
  <p class="text-xs opacity-90 mt-1">Angular компонент можно использовать везде — React, Vue, ванильный JS</p>
</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #10b981, #059669);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #059669, #047857);
}
</style>

---

# Пример Angular компонента для экспорта

<div class="max-h-[400px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-sky-500/30 p-5 hover:border-sky-400/50 transition-all duration-300">

```typescript
// my-card.component.ts
import { Component, Input, Output, EventEmitter } from '@angular/core';

@Component({
  selector: 'app-my-card',
  template: `
    <div class="card">
      <div class="card-header">
        <h2>{{ title }}</h2>
      </div>
      <div class="card-body">
        <p>{{ description }}</p>
      </div>
      <div class="card-footer">
        <button (click)="onAction()">{{ actionLabel }}</button>
      </div>
    </div>
  `,
  styles: [`
    .card {
      border: 2px solid rgba(0, 212, 255, 0.2);
      border-radius: 12px;
      overflow: hidden;
      background: linear-gradient(135deg, rgba(0, 212, 255, 0.05), rgba(124, 58, 237, 0.05));
    }
    .card-header { padding: 1.5rem; background: linear-gradient(135deg, #00d4ff, #7c3aed); }
    .card-body { padding: 1.5rem; }
    .card-footer { padding: 1rem 1.5rem; border-top: 1px solid rgba(255, 255, 255, 0.1); }
    button {
      padding: 8px 16px;
      background: linear-gradient(135deg, #00d4ff, #7c3aed);
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-weight: bold;
    }
  `]
})
export class MyCardComponent {
  @Input() title: string = 'Card Title';
  @Input() description: string = 'Card description';
  @Input() actionLabel: string = 'Action';
  @Output() actionClick = new EventEmitter<void>();

  onAction() {
    this.actionClick.emit();
  }
}
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #0ea5e9, #06b6d4);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #06b6d4, #0891b2);
}
</style>

---

# CUSTOM_ELEMENTS_SCHEMA в Angular

<div class="max-h-[420px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-violet-500/30 p-5 hover:border-violet-400/50 transition-all duration-300">

```typescript
// app.module.ts
import { NgModule, CUSTOM_ELEMENTS_SCHEMA } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';

import { AppComponent } from './app.component';

@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  schemas: [CUSTOM_ELEMENTS_SCHEMA] // ← Ключевая строка!
})
export class AppModule { }

// ============================================

// app.component.ts
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  template: `
    <div class="app-container">
      <!-- Использование веб компонента -->
      <star-rating
        [attr.rating]="userRating"
        (rating-changed)="onRatingChanged($event)">
      </star-rating>

      <!-- Веб компонент от Material -->
      <mdc-button (click)="handleClick()">
        Click me
      </mdc-button>

      <!-- Произвольный веб компонент -->
      <my-custom-element
        [attr.data-id]="itemId"
        (custom-event)="handleCustomEvent($event)">
      </my-custom-element>
    </div>
  `,
  styles: [`.app-container { display: grid; gap: 1rem; padding: 2rem; }`]
})
export class AppComponent {
  userRating = 3;
  itemId = 42;

  onRatingChanged(event: any) {
    this.userRating = event.detail.rating;
  }

  handleClick() {
    console.log('Button clicked!');
  }

  handleCustomEvent(event: any) {
    console.log('Custom event:', event.detail);
  }
}
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #8b5cf6, #7c3aed);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #7c3aed, #6d28d9);
}
</style>

---

# Angular Material Web Components

<div class="space-y-4 pb-4">

<div v-motion :initial="{ opacity: 0, y: 50 }" :enter="{ opacity: 1, y: 0, transition: { duration: 600 } }" class="p-4 rounded-2xl bg-gradient-to-br from-cyan-500/20 to-blue-500/20 border border-cyan-500/30 hover:border-cyan-400 transition-all duration-300">
  <h3 class="text-sm font-bold mb-2 text-cyan-300">🎨 Material Design Components</h3>
  <p class="text-xs mb-2">Google's Material Web — полный набор веб компонентов Material Design</p>
  <div class="text-xs text-gray-300">
    Доступно: <span class="text-cyan-400">Button</span>, <span class="text-cyan-400">Card</span>, <span class="text-cyan-400">Dialog</span>, <span class="text-cyan-400">TextField</span>, <span class="text-cyan-400">Switch</span>, <span class="text-cyan-400">Menu</span>
  </div>
</div>

<div v-motion :initial="{ opacity: 0, y: 50 }" :enter="{ opacity: 1, y: 0, transition: { duration: 600, delay: 200 } }" class="p-4 rounded-2xl bg-gradient-to-br from-purple-500/20 to-pink-500/20 border border-purple-500/30 hover:border-pink-400 transition-all duration-300">
  <h3 class="text-sm font-bold mb-2 text-purple-300">✨ CDK (Component Dev Kit)</h3>
  <p class="text-xs mb-2">Angular CDK предоставляет базовую функциональность для создания компонентов</p>
  <div class="text-xs text-gray-300">
    Применяется для: <span class="text-purple-400">accessibility</span>, <span class="text-purple-400">overlay</span>, <span class="text-purple-400">drag-drop</span>
  </div>
</div>

</div>

<div v-click class="p-3 rounded-lg bg-gradient-to-r from-emerald-500/20 to-cyan-500/20 border border-emerald-500/30 font-mono text-xs pb-4">
  <span class="text-emerald-400">$</span> npm install @material/web
</div>

---
layout: section
background: linear-gradient(135deg, #a8edea 0%, #fed6e3 100%)
---

# Лучшие практики и паттерны

---

# Проектирование веб компонента

<div class="grid grid-cols-2 gap-4 pb-4">

<div v-motion :initial="{ opacity: 0, x: -50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

<h3 class="text-sm font-bold mb-3 text-cyan-300">🎯 Жизненный цикл разработки</h3>

<div class="space-y-2">
  <div class="p-2 rounded-lg bg-gradient-to-r from-cyan-500/20 to-blue-500/20 border-l-4 border-cyan-500 text-xs">
    <div class="font-bold text-xs text-cyan-300">1. Интерфейс</div>
    <p class="text-xs opacity-80 mt-0.5">Props, Slots, Events</p>
  </div>

  <div class="p-2 rounded-lg bg-gradient-to-r from-purple-500/20 to-pink-500/20 border-l-4 border-purple-500 text-xs">
    <div class="font-bold text-xs text-purple-300">2. Логика</div>
    <p class="text-xs opacity-80 mt-0.5">Lifecycle, State, Events</p>
  </div>
</div>

</div>

<div v-motion :initial="{ opacity: 0, x: -50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

<div class="space-y-2">

  <div class="p-2 rounded-lg bg-gradient-to-r from-indigo-500/20 to-blue-500/20 border-l-4 border-indigo-500 text-xs">
    <div class="font-bold text-xs text-indigo-300">3. Стилизация</div>
    <p class="text-xs opacity-80 mt-0.5">CSS Variables, ::part</p>
  </div>

  <div class="p-2 rounded-lg bg-gradient-to-r from-emerald-500/20 to-cyan-500/20 border-l-4 border-emerald-500 text-xs">
    <div class="font-bold text-xs text-emerald-300">4. Тестирование</div>
    <p class="text-xs opacity-80 mt-0.5">Unit, Integration, A11y</p>
  </div>

  <div class="p-2 rounded-lg bg-gradient-to-r from-amber-500/20 to-orange-500/20 border-l-4 border-amber-500 text-xs">
    <div class="font-bold text-xs text-amber-300">5. Документация</div>
    <p class="text-xs opacity-80 mt-0.5">Props, Events, Examples</p>
  </div>
</div>

</div>
</div>

---

<div class="grid grid-cols-1 gap-4 pb-4">
<div v-motion :initial="{ opacity: 0, x: 50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

<h3 class="text-sm font-bold mb-3 text-pink-300">✨ Правила именования</h3>

<div class="space-y-1 max-h-[360px] overflow-y-auto rounded-lg bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-pink-500/30 p-3">

```javascript
// ❌ Плохо
class Card extends HTMLElement {}
customElements.define('card', Card);

// ✅ Хорошо
class MyCard extends HTMLElement {}
customElements.define('my-card', MyCard);

// ✅ Отлично
class HeaderComponent extends HTMLElement {}
customElements.define(
  'app-header-v2',
  HeaderComponent
);

// ✅ Библиотека UI
class Button extends HTMLElement {}
customElements.define('ui-button', Button);

// ✅ Компания
class DashboardWidget extends HTMLElement {}
customElements.define(
  'acme-dashboard-widget',
  DashboardWidget
);
```

**Правила:**
- Дефис (минимум один)
- Начинаться с буквы
- Нижний регистр
- Описательное имя

</div>

</div>

</div>

<style>
::-webkit-scrollbar {
  width: 6px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 3px;
}

::-webkit-scrollbar-thumb {
  background: rgba(236, 72, 153, 0.4);
  border-radius: 3px;
}

::-webkit-scrollbar-thumb:hover {
  background: rgba(236, 72, 153, 0.7);
}
</style>

---

# CSS Custom Properties для темизации

<div class="max-h-[420px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-fuchsia-500/30 p-5 hover:border-fuchsia-400/50 transition-all duration-300">

```javascript
class ThemedCard extends HTMLElement {
  connectedCallback() {
    this.attachShadow({ mode: 'open' });
    this.render();
  }

  render() {
    this.shadowRoot.innerHTML = `
      <style>
        :host {
          --card-bg: #ffffff;
          --card-border: #e0e0e0;
          --card-text: #333333;
          --card-padding: 1rem;
          --card-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
          --card-radius: 8px;
        }

        .card {
          background: var(--card-bg);
          border: 2px solid var(--card-border);
          color: var(--card-text);
          padding: var(--card-padding);
          border-radius: var(--card-radius);
          box-shadow: var(--card-shadow);
          transition: all 0.3s ease;
        }

        .card:hover {
          transform: translateY(-4px);
          box-shadow: 0 12px 24px rgba(0, 0, 0, 0.15);
        }
      </style>
      <div class="card">
        <slot></slot>
      </div>
    `;
  }
}

customElements.define('themed-card', ThemedCard);
```
```css
/* Использование с CSS переменными */
themed-card {
  --card-bg: #f5f5f5;
  --card-text: #666;
  --card-padding: 2rem;
}

/* Тёмная тема */
[data-theme="dark"] themed-card {
  --card-bg: #2a2a2a;
  --card-text: #ffffff;
  --card-border: #444;
}
```
</div>



<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #ec4899, #d946ef);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #d946ef, #c084fc);
}
</style>

---

# Performance: Ленивая загрузка компонентов

<div class="max-h-[420px] overflow-y-auto rounded-xl bg-gradient-to-br from-slate-900 via-slate-950 to-black border border-teal-500/30 p-5 hover:border-teal-400/50 transition-all duration-300">

```javascript
class LazyComponent extends HTMLElement {
  connectedCallback() {
    const observer = new IntersectionObserver(
      (entries) => {
        entries.forEach((entry) => {
          if (entry.isIntersecting) {
            this.loadComponent();
            observer.unobserve(this);
          }
        });
      },
      { threshold: 0.1 }
    );

    observer.observe(this);
  }

  async loadComponent() {
    try {
      const { HeavyComponent } = await import('./heavy.js');

      this.attachShadow({ mode: 'open' });
      this.render(HeavyComponent);

      this.dispatchEvent(
        new CustomEvent('component-loaded', { bubbles: true })
      );
    } catch (error) {
      console.error('Failed to load component:', error);
      this.showError();
    }
  }

  render(Component) {
    this.shadowRoot.innerHTML = `
      <style>
        .loading {
          background: linear-gradient(90deg, rgba(0, 212, 255, 0.1), rgba(124, 58, 237, 0.1));
          padding: 2rem;
          border-radius: 8px;
          animation: shimmer 1.5s infinite;
        }
        @keyframes shimmer {
          0% { opacity: 0.5; }
          50% { opacity: 1; }
          100% { opacity: 0.5; }
        }
      </style>
      <div class="loading">Загрузка компонента...</div>
    `;
  }

  showError() {
    this.shadowRoot.innerHTML = `
      <div style="color: red; padding: 1rem;">
        ❌ Ошибка при загрузке
      </div>
    `;
  }
}

customElements.define('lazy-component', LazyComponent);
```

</div>

<style>
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 0, 0, 0.1);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #14b8a6, #06b6d4);
  border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #06b6d4, #0891b2);
}
</style>

---
layout: section
background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%)
---

# Заключение и будущее

---

# Основные выводы

<div class="grid grid-cols-2 gap-4 pb-4">

<div v-motion :initial="{ opacity: 0, x: -50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

<h3 class="text-sm font-bold mb-3 text-cyan-300">💡 Ключевые преимущества</h3>

<div class="space-y-2">
  <div class="flex items-start gap-2 p-2 rounded-lg bg-cyan-500/10 border-l-4 border-cyan-500 text-xs">
    <span class="text-lg min-w-8">1️⃣</span>
    <div>
      <div class="font-bold">Framework-независимость</div>
      <p class="opacity-80 text-xs">Работают везде</p>
    </div>
  </div>

  <div class="flex items-start gap-2 p-2 rounded-lg bg-purple-500/10 border-l-4 border-purple-500 text-xs">
    <span class="text-lg min-w-8">2️⃣</span>
    <div>
      <div class="font-bold">Долгосрочность</div>
      <p class="opacity-80 text-xs">Веб-стандарт — актуально</p>
    </div>
  </div>

  <div class="flex items-start gap-2 p-2 rounded-lg bg-pink-500/10 border-l-4 border-pink-500 text-xs">
    <span class="text-lg min-w-8">3️⃣</span>
    <div>
      <div class="font-bold">Микрофронтенды</div>
      <p class="opacity-80 text-xs">Идеальны для распределённых</p>
    </div>
  </div>

  <div class="flex items-start gap-2 p-2 rounded-lg bg-emerald-500/10 border-l-4 border-emerald-500 text-xs">
    <span class="text-lg min-w-8">4️⃣</span>
    <div>
      <div class="font-bold">Производительность</div>
      <p class="opacity-80 text-xs">Нативная поддержка браузерами</p>
    </div>
  </div>
</div>

</div>

<div v-motion :initial="{ opacity: 0, x: 50 }" :enter="{ opacity: 1, x: 0, transition: { duration: 600 } }">

<h3 class="text-sm font-bold mb-3 text-pink-300">⚠️ Когда использовать</h3>

<div class="space-y-2">
  <div class="p-2 rounded-lg bg-gradient-to-r from-green-500/20 to-emerald-500/20 border border-green-500/30 text-xs">
    <div class="font-bold text-green-300 mb-0.5">✅ Используй веб компоненты</div>
    <ul class="text-xs opacity-80 space-y-0.5">
      <li>→ UI библиотеки</li>
      <li>→ Микрофронтенды</li>
      <li>→ Design Systems</li>
      <li>→ Multi-framework integration</li>
    </ul>
  </div>

  <div class="p-2 rounded-lg bg-gradient-to-r from-red-500/20 to-pink-500/20 border border-red-500/30 text-xs">
    <div class="font-bold text-red-300 mb-0.5">❌ Когда избежать</div>
    <ul class="text-xs opacity-80 space-y-0.5">
      <li>→ Простая одностраничка</li>
      <li>→ Только React/Vue/Angular</li>
      <li>→ Требуется SSR</li>
    </ul>
  </div>
</div>

</div>

</div>

---

# Будущее веб компонентов

<div class="grid grid-cols-2 gap-3 pb-4">

<div v-click class="p-3 rounded-2xl bg-gradient-to-br from-blue-500/20 to-cyan-500/20 border border-blue-500/30 hover:border-blue-400 transition-all duration-300 hover:shadow-lg hover:shadow-blue-500/20">
  <h3 class="text-sm font-bold text-blue-300 mb-1">🚀 Scoped Registry</h3>
  <p class="text-xs">Локальная регистрация элементов</p>
</div>

<div v-click class="p-3 rounded-2xl bg-gradient-to-br from-purple-500/20 to-pink-500/20 border border-purple-500/30 hover:border-purple-400 transition-all duration-300 hover:shadow-lg hover:shadow-purple-500/20">
  <h3 class="text-sm font-bold text-purple-300 mb-1">📦 Улучшение инструментов</h3>
  <p class="text-xs">Лучшая интеграция с TypeScript</p>
</div>

<div v-click class="p-3 rounded-2xl bg-gradient-to-br from-emerald-500/20 to-cyan-500/20 border border-emerald-500/30 hover:border-emerald-400 transition-all duration-300 hover:shadow-lg hover:shadow-emerald-500/20">
  <h3 class="text-sm font-bold text-emerald-300 mb-1">🔄 Стандартизация</h3>
  <p class="text-xs">Встроенная поддержка везде</p>
</div>

<div v-click class="p-3 rounded-2xl bg-gradient-to-br from-amber-500/20 to-orange-500/20 border border-amber-500/30 hover:border-amber-400 transition-all duration-300 hover:shadow-lg hover:shadow-amber-500/20">
  <h3 class="text-sm font-bold text-amber-300 mb-1">🌐 Массовое применение</h3>
  <p class="text-xs">Google, Adobe, Microsoft — production</p>
</div>

</div>

---

# Спасибо за внимание! 🎉

<div class="space-y-6 mt-8 text-center pb-4">

<div class="text-3xl font-bold bg-gradient-to-r from-cyan-400 via-purple-400 to-pink-400 bg-clip-text text-transparent">
  Веб компоненты — будущее переиспользуемого кода
</div>

<div class="text-sm opacity-90">
  Стандарты, микрофронтенды и интеграция с фреймворками
</div>

<div class="space-y-2 text-xs">
  <p class="font-bold text-cyan-300">Главная идея:</p>
  <p class="text-lg bg-gradient-to-r from-cyan-400 to-purple-400 bg-clip-text text-transparent font-bold">Один компонент, везде работает ✨</p>
</div>

<div class="pt-4 border-t border-gray-700">
  <p class="text-xs opacity-60">Спасибо за внимание! Вопросы и обсуждение 🚀</p>
</div>

</div>

---
layout: end
background: linear-gradient(135deg, #0f0c29 0%, #302b63 50%, #24243e 100%)
---

# До встречи! 👋

<div class="text-center space-y-6 pb-10">

<div class="text-6xl">✨</div>

<div class="text-2xl bg-gradient-to-r from-cyan-400 via-purple-400 to-pink-400 bg-clip-text text-transparent font-bold">
  Веб компоненты меняют веб
</div>

<div class="text-sm opacity-70">
  Спасибо за участие в этой лекции!
</div>

</div>
