# Squad404

Командний C++ проєкт.

## Гілки

- `main` — стабільна версія. Напряму не пушимо.
- `develop` — спільна тестова версія.
- `feature/...` — окрема гілка під конкретну задачу.

Схема роботи:

```text
feature/... -> Pull Request -> develop -> Pull Request -> main
```

Кожен розробник працює у своїй `feature/...` гілці. `Commit + Push` зберігає тільки його роботу і не змінює гілки інших розробників.

Коли з'являться Jira-задачі, називаємо гілки так:

```text
feature/S4-12-menu
feature/S4-13-map
feature/S4-14-schedule
```

## Структура

```text
src/       C++ source code
assets/    ресурси, зображення, файли карти
docs/      документація
tests/     тести
.github/   GitHub rules/templates
```

Команди Git для команди: [`docs/GIT-COMMANDS.md`](docs/GIT-COMMANDS.md).
