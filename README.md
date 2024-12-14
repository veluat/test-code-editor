# Упрощённый онлайн редактор кода

## Краткое описание

Проект представляет собой онлайн-редактор кода, который поддерживает написание кода на JavaScript и Python. Пользователи могут писать код, запускать его и получать вывод или ошибки в удобном интерфейсе. **Примечание**: Эта версия редактора кода не выполняет реальный код, а возвращает моковые ответы на команды `console.log()` для JavaScript и `print()` для Python. Редактор использует библиотеку AceEditor для синтаксического выделения и удобного редактирования кода. Для мокирования API используется MirageJS.

## Технологии

Проект разработан с использованием следующих технологий:

- **React**: для создания пользовательского интерфейса.
- **Vite**: для быстрой сборки и разработки.
- **pnpm**: для управления зависимостями.
- **Ace Editor**: библиотека для редактирования кода с поддержкой синтаксического выделения и автозавершения.
- **MirageJS**: инструмент для мокирования API, позволяющий эмулировать серверные ответы без настройки отдельного сервера.
- **Sass**: препроцессор CSS, который помогает в написании более структурированного и поддерживаемого стиля.
- **ESLint**: инструмент для анализа кода, который помогает находить и исправлять проблемы в JavaScript и React-коде.

## Инструкции по установке и запуску

### Установка

1. **Склонируйте репозиторий**:

    ```bash
    git clone https://github.com/veluat/test-code-editor.git
    cd test-code-editor  # Замените на фактическое имя папки, если оно отличается
    ```

2. **Установите зависимости**:

    ```bash
    pnpm install
    ```

### Запуск

1. **Запустите приложение**:

    ```bash
    pnpm run dev
    ```

   Откройте браузер и перейдите по адресу: `http://localhost:5173`

## Использование MirageJS

Проект использует **MirageJS** для мокирования API. Это позволяет эмулировать серверные ответы без необходимости настройки отдельного сервера.

### Функции MirageJS

- **Обработка POST-запросов**: MirageJS обрабатывает запросы на маршрут `/api/run`, возвращая мокированные данные.
- **Поддержка JavaScript и Python**: MirageJS возвращает моковые ответы на команды `console.log()` для JavaScript и `print()` для Python.

## Ограничения функционала

- **Поддержка только JavaScript и Python**: В текущей версии редактор поддерживает выполнение кода только на этих двух языках. Другие языки не поддерживаются.
- **Ограничения по выполнению кода**: Эта версия редактора кода не выполняет реальный код, а возвращает моковые ответы на команды `console.log()` для JavaScript и `print()` для Python.
- **Отсутствие управления состоянием**: Редактор не сохраняет код между сессиями. После перезагрузки страницы все несохраненные изменения будут потеряны.

## Варианты расширения приложения

- **Исполнение кода**: В будущем реализовать функционал, который позволит выполнять код в реальном времени, как в действующих редакторах, предоставляя пользователям возможность видеть результаты выполнения и отладку их программ.
- **Добавление поддержки других языков**: Реализовать выполнение кода на других языках программирования, таких как Ruby, PHP или Java.
- **Сохранение кода**: Внедрить функциональность для сохранения кода в базу данных, чтобы пользователи могли возвращаться к своим проектам.
- **Поддержка библиотек**: Позволить пользователям подключать сторонние библиотеки и модули для более сложных задач.
- **Обработка ошибок**: Улучшить механизм обработки ошибок, чтобы предоставлять более подробную информацию пользователям о возможных проблемах в их коде.
- **Интерфейс пользователя**: Улучшить интерфейс с помощью дополнительных функций, таких как автозаполнение, подсказки и темная тема.
