% PERSONALIZATION GUIDE - DOSSIER

## 🔐 НАСТРОЙКА БЕЗОПАСНОСТИ

### 1. Смена пароля admin-панели

Открой `/admin.html` в текстовом редакторе и найди строку:

```javascript
const ADMIN_PASSWORD = "admin123";
```

Замени `"admin123"` на свой пароль:

```javascript
const ADMIN_PASSWORD = "твой_супер_пароль_123";
```

**Совет:** Используй пароль из букв, цифр и символов (минимум 8 символов).

---

## 🎨 НАСТРОЙКА ДИЗАЙНА

### Смена цветовой схемы

В файлах `index.html` и `admin.html` найди блок `<style>` и измени эти цвета:

| Переменная | Текущее значение | Назначение |
|-----------|------------------|-----------|
| Main Title | `#b8b8ff` | Заголовок (DOSSIER) |
| Accents | `#9090ff` | Фиолетовые акценты |
| Text Labels | `#7080a0` | Серо-голубой текст |
| Main Text | `#d0d0ff` | Основной текст |
| Background | `#0a0e27` | Фон |

### Пример смены цветов

Найди:
```css
.title {
    color: #b8b8ff;  ← Меняй это!
    ...
}
```

И поменяй на:
```css
.title {
    color: #00d9ff;  ← Новый цвет!
    ...
}
```

**Генератор HEX цветов:** https://www.color-hex.com/

---

## 📝 ИЗМЕНЕНИЕ ОСНОВНОЙ ИНФОРМАЦИИ

Открой `/index.html` и найди секцию:

```html
<!-- Основная информация -->
<section class="section">
    <h2 class="section-title">ОСНОВНЫЕ ДАННЫЕ</h2>
    <div class="info-grid">
        <div class="info-item">
            <span class="label">Полное имя</span>
            <span class="value">Курносова Ольга Николаевна</span>  ← Меняй здесь
        </div>
        ...
    </div>
</section>
```

Просто замени текст в тегах `<span class="value">`.

---

## ➕ ДОБАВЛЕНИЕ НОВЫХ СЕКЦИЙ

### Шаблон новой секции

Скопируй этот блок и добавь в `index.html` перед закрывающим тегом `</div>`:

```html
<section class="section">
    <h2 class="section-title">НАЗВАНИЕ СЕКЦИИ</h2>
    
    <div class="info-grid">
        <div class="info-item">
            <span class="label">Параметр 1</span>
            <span class="value">Значение 1</span>
        </div>
        <div class="info-item">
            <span class="label">Параметр 2</span>
            <span class="value">Значение 2</span>
        </div>
    </div>
</section>
```

### Список информации

```html
<section class="section">
    <h2 class="section-title">МОЙ СПИСОК</h2>
    
    <ul class="info-list">
        <li>Первый пункт</li>
        <li>Второй пункт</li>
        <li>Третий пункт</li>
    </ul>
</section>
```

---

## 🔗 ИЗМЕНЕНИЕ ССЫЛОК

Найди в `index.html`:

```html
<div class="links-container">
    <a href="https://vk.com/id733148411" class="link-btn" target="_blank">
        VK
    </a>
    ...
</div>
```

Замени:
- `href="НОВАЯ_ССЫЛКА"` — ссылка на профиль
- Текст между `<a>` и `</a>` — название кнопки

---

## 📱 ЛОГОТИП И ИКОНКИ

### Добавление иконок

Используй эмодзи прямо в тексте:

```html
<a href="..." class="link-btn">
    🎬 YouTube
</a>
```

Или Unicode символы:
```
☎️  — телефон
✉️  — письмо
🌐 — интернет
🔐 — ключ
```

---

## 🌙 ТЕМНЫЕ РЕЖИМЫ (дополнительно)

Если хочешь еще более темный вид, найди:

```css
background: linear-gradient(135deg, #0a0e27 0%, #1a1f3a 50%, #0f1428 100%);
```

И замени на:

```css
background: linear-gradient(135deg, #000000 0%, #0a0a1a 50%, #000000 100%);
```

---

## ⚠️ ВАЖНО!

1. **Сохраняй резервные копии**
   ```bash
   cp index.html index.html.backup
   cp admin.html admin.html.backup
   ```

2. **Проверяй изменения**
   - Открой файл в браузере (Ctrl+O или Cmd+O)
   - Проверь все ссылки и текст

3. **Загружай изменения на GitHub**
   ```bash
   git add .
   git commit -m "Обновление дизайна"
   git push
   ```

4. **Очистка кэша браузера** (если изменения не видны)
   - Нажми Ctrl+Shift+Del (или Cmd+Shift+Del на Mac)
   - Выбери "Все время"
   - Нажми "Очистить"

---

## 📞 ПОДДЕРЖКА

Если что-то не работает:

1. Проверь консоль браузера (F12 → Console)
2. Убедись что синтаксис HTML правильный (теги закрыты)
3. Проверь пароль в админ-панели
4. Очисти localStorage: `F12 → Application → localStorage → delete`

---

**Готово! Твой сайт готов к запуску!** 🚀
