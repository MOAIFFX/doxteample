% QUICK START - DOSSIER

## ⚡ 2 минуты на запуск

### Шаг 1️⃣: Локальный просмотр

```bash
# Открой в браузере
# Просто двойной клик на index.html
# ИЛИ
cd /workspaces/doxteample
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

### Шаг 2️⃣: Пуш на GitHub

```bash
# Проверка статуса
git status

# Добавить все файлы
git add .

# Сделать коммит
git commit -m "Initial dossier setup"

# Загрузить на GitHub
git push origin main
```

### Шаг 3️⃣: Включить GitHub Pages

1. Перейди на GitHub репозиторий
2. Settings → Pages
3. Source: Deploy from a branch
4. Branch: `main` | Folder: `/ (root)`
5. Save

**✅ Готово!** Твой сайт доступен на:
```
https://[твой-github-username].github.io/doxteample/
```

---

## 🔑 Важные точки

| Файл | Для чего |
|------|----------|
| `index.html` | Основной сайт |
| `admin.html` | Управление контентом |
| `README.md` | Документация |
| `PERSONALIZATION.md` | Как изменять |

---

## 🛡️ Безопасность

⚠️ **Примечание о пароле:**

Текущий пароль: `admin123`

**Измени сейчас!** (открой `admin.html`, найди строку ~115)

```javascript
// НАЙДИ:
const ADMIN_PASSWORD = "admin123";

// ЗАМЕНИ НА:
const ADMIN_PASSWORD = "твой-крутой-пароль";
```

**Да, это видно в коде**, он не скрыт. Используй внешний способ аутентификации если нужна高 безопасность, или просто используй сложный пароль.

---

## 📋 Чек-лист первого запуска

- [ ] Просмотрел index.html локально
- [ ] Проверил что информация отобразилась правильно
- [ ] Измени пароль в admin.html
- [ ] Загрузил на GitHub (git push)
- [ ] Включил GitHub Pages
- [ ] Проверил сайт по ссылке https://...

---

## 💡 Следующие шаги

1. **Персонализируй дизайн**
   → Посмотри `PERSONALIZATION.md`

2. **Добавь новые данные**
   → Отредактируй `index.html` или используй admin-панель

3. **Поделись ссылкой**
   → Показывай свой сайт!

---

**Вопросы? Проблемы?**

Проверь консоль браузера (F12):
- Нет ошибок в консоли?
- Все стили загружены?
- localStorage работает? (F12 → Application → localStorage)

**Готово! Твой сайт в air! 🚀**
