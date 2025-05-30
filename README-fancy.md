<!--
OmniCore-Robotics
Copyright (C) 2025  Naumov Maxim

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
-->

<style>
:root {
  --primary-color:  rgb(240, 120, 60); 
  --secondary-color: rgb(120, 180, 200);
  --tertiary-color: rgb(120, 80, 220);
  --bg-color: #0d1117;
  --text-color: #c9d1d9;
  --border-color: #30363d;
  --footer-color: #8b949e;
}

body {
  background-color: var(--bg-color);
  color: var(--text-color);
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
  line-height: 1.2;
}

h1, h2, h3, h4 {
  color: #e6edf3;
  font-weight: 600;
}

.custom-quote {
  border-left: 4px solid var(--primary-color);
  padding: 1rem;
  margin: 2rem 0;
  background: rgba(22, 27, 34, 0.5);
  border-radius: 0 8px 8px 0;
  box-shadow: 0 1px 3px rgba(0,0,0,0.12);
}

.custom-quote footer {
  display: block;
  font-size: 0.9rem;
  color: var(--footer-color);
  border-top: 1px solid var(--border-color);
  padding-top: 0.8rem;
  margin-top: 1rem;
}

ul {
  list-style-type: none;
  padding-left: 1.2rem;
  margin: 0.8rem 0;
}

ul li {
  margin-bottom: 0.6rem;
  position: relative;
}

ul li::before {
  content: '—';
  position: absolute;
  left: -1.2rem;
  color: var(--secondary-color);
  font-weight: bold;
}

a {
  color: #58a6ff;
  text-decoration: none;
  transition: color 0.2s;
}

a:hover {
  color: #79c0ff;
  text-decoration: underline;
}

code {
  background: rgba(100, 110, 130, 0.4);
  padding: 0.1rem 0.5rem;
  border-radius: 0.6em;
  font-family: 'SFMono-Regular', Consolas, 'Liberation Mono', Menlo, monospace;
}

hr {
  border: 0;
  height: 1px;
  background: var(--border-color);
  margin: 2rem 0;
}

.header-logo {
  text-align: center;
  margin-bottom: 2rem;
}

.header-logo h1 {
  font-size: 2.5rem;
  margin-bottom: 0.5rem;
}

.header-logo p {
  font-size: 1.2rem;
  color: var(--footer-color);
}

/* Добавлено: Стили для нумерованных списков */
ol {
  padding-left: 1.8rem;
  margin: 0.8rem 0;
}

ol li {
  margin-bottom: 0.6rem;
}
</style>

<div class="header-logo">
  <h1>OmniCore Robotics</h1>
  <p>Открытая модульная платформа для создания мобильных роботов</p>
</div>

<blockquote class="custom-quote">
  <h2>Обзор</h2>
  <p>Проект разрабатывает совместимые модули и шасси для мобильных роботов</p>

  <p>Разработка происходит с использованием:</p>
  <ul>
    <li>3D-печати (FFF/FDM)</li>
    <li>Лазерной резки</li>
    <li>Модульного подхода в проектировании</li>
  </ul>

<h3>Цели</h3>
  <ol>
    <li>Создание экосистемы модулей и шасси для быстрой сборки роботов</li>
    <li>Обеспечение доступности производства (домашние 3D-принтеры или лазерная резка)</li>
    <li>Поддержка модернизации и обратная совместимость</li>
  </ol>

  <footer>Платформа для разработки</footer>
</blockquote>

<h2>Структура репозитория</h2>

<blockquote class="custom-quote">
  <h3><a href="./Модели">Модели</a></h3>
  <p>Основные проектные файлы для аппаратных компонентов</p>

  <ul>
    <li><a href="./Модели/Механика">Механика</a> — Сборочные единицы механики</li>
    <li><a href="./Модели/Модули">Модули</a> — Универсальные модули</li>
    <li><a href="./Модели/Колеса">Колеса</a> — Серии дисков и шин</li>
    <li><a href="./Модели/Электроника">Электроника</a> — Модели электрических компонентов</li>
    <li><a href="./Модели/Конструктив">Конструктив</a> — Конструкционные элементы</li>
    <li><a href="./Модели/Шасси">Шасси</a> — Серии шасси</li>
    <li><a href="./Модели/Профили">Профили</a> — Вспомогательные модели</li>
    <li><a href="./Модели/Формы">Формы</a> — Формы для отливки</li>
  </ul>

  <footer>
    Для проектирования используется КОМПАС 3D v23: <code>.m3d</code>, <code>.a3d</code> <br>
    Подготовка к печати - PrusaSlicer: <code>.3mf</code>, <code>.stp</code>
  </footer>
</blockquote>

<blockquote class="custom-quote" style="border-left-color: var(--secondary-color)">
  <h3><a href="./Код">Код</a></h3>
  <p>Программное обеспечение для управления роботами</p>

  <ul>
    <li><a href="./Код/Arduino">Arduino</a> — Скетчи (Примеры)</li>
    <li><a href="./Код/PlatformIO">PlatformIO</a> — Проекты PIO</li>
  </ul>

  <footer>Используется Clion или VS Code для разработки</footer>
</blockquote>

<blockquote class="custom-quote" style="border-left-color: var(--tertiary-color)">
  <h3><a href="./.meta">Meta</a></h3>
  <p>Служебные данные и утилиты проекта</p>

  <footer>Метаданные проекта и вспомогательные инструменты</footer>
</blockquote>

<h2>Участие в проекте</h2>

<p>Для вклада в разработку:</p>
<ol>
  <li>Создайте форк репозитория</li>
  <li>Ознакомьтесь с <a href="./CONTRIBUTING.md">правилами участия</a></li>
  <li>Выполните pull request с вашими изменениями</li>
</ol>

<h2>Лицензия</h2>
<p>Проект распространяется под лицензией <strong>GNU General Public License v3.0</strong>.<br>
Любые производные работы должны оставаться открытыми и распространяться под той же лицензией.</p>
<p>Подробнее: <a href="LICENSE">LICENSE</a></p>