# Git команди для команди

## Перший запуск

```bash
git clone https://github.com/f1lef/squad404.git
cd squad404
git fetch origin
git switch develop
```

## Нова задача

Починаємо від свіжого `develop`:

```bash
git switch develop
git pull
git switch -c feature/task-name
```

Коли є Jira-задача:

```bash
git switch -c feature/S4-12-menu
```

## Зберегти роботу

```bash
git status
git add .
git commit -m "Describe change"
git push -u origin feature/task-name
```

Наступні рази в цій самій гілці:

```bash
git add .
git commit -m "Describe change"
git push
```

## Коли задача готова

Створи Pull Request:

```text
feature/... -> develop
```

Після тестування інтегрованої версії:

```text
develop -> main
```

## Корисне

```bash
git branch
git status
git log --oneline
git fetch
git pull
```

Безпечне скасування вже створеного commit:

```bash
git revert HASH
```

Не робіть `force push` у спільні гілки.
