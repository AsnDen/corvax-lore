# Руководство для начинающих контрибьюторов 🌱

Добро пожаловать! Этот гайд проведёт вас через весь процесс шаг за шагом — даже если вы никогда не работали с GitHub.

---

## 🎮 Часть 1: Первые шаги на GitHub

### 1. Регистрация аккаунта
1. Зайдите на [github.com](https://github.com/)
2. Нажмите "Sign up" в правом верхнем углу
3. Заполните форму (email, пароль, имя пользователя)
4. Подтвердите email (проверьте папку "Спам")

### 2. Установите Git
1. Скачайте Git: [git-scm.com/downloads](https://git-scm.com/downloads)
2. Запустите установщик (всё время жмите "Next")

---

## 🍴 Часть 2: Работа с репозиторием

### 1. Создание копии (Fork)
1. Откройте наш репозиторий: [https://github.com/AsnDen/corvax-lore]
2. Нажмите кнопку "Fork" справа вверху
3. Выберите свой аккаунт в появившемся окне

![Кнопка Fork](https://i.imgur.com/5v8gFd1.png)

### 2. Копирование на компьютер (Clone)
1. На странице вашего форка нажмите зелёную кнопку "Code"
2. Скопируйте ссылку (HTTPS)
3. Откройте терминал/командную строку и выполните:
```bash
git clone ВСТАВЬТЕ_ССЫЛКУ_ЗДЕСЬ
cd corvax-lore  # Переход в папку проекта
```

---

## 🌿 Часть 3: Работа с ветками

### 1. Создание новой ветки
Всегда создавайте отдельную ветку для изменений:
```bash
git checkout -b мои-изменения
```

**Пояснение**:  
`мои-изменения` — название вашей ветки (можно писать по-английски, например `fix-typos`)

### 2. Переключение между ветками
- Посмотреть все ветки: `git branch`
- Переключиться на ветку: `git checkout имя_ветки`

---

## ✍️ Часть 4: Внесение изменений

### 1. Редактирование файлов
1. Откройте файл в любом редакторе:
   - Рекомендуем [VS Code](https://code.visualstudio.com/)
   - Или обычный Блокнот
2. Внесите изменения и сохраните

### 2. Сохранение версий (Commit)
```bash
git add .                      # Добавить все изменения
git commit -m "Описание правок" # Создать "сохранение"
```

**Пример хорошего описания**:  
"Добавил описание расы Слаймолюды в раздел Расы"

---

## 🚀 Часть 5: Отправка изменений

### 1. Загрузка в ваш форк
```bash
git push origin мои-изменения
```

### 2. Создание Pull Request (PR)
1. На странице вашего форка нажмите "Compare & pull request"
2. Заполните форму:
   - **Title**: Краткое описание ("Добавлена статья о плазменных мечах")
   - **Description**: Подробности и скриншоты (если нужно)
3. Нажмите "Create pull request"

![Создание PR](https://i.imgur.com/qb5WXya.png)

---

## 🔄 Часть 6: Обновление локальной копии

### 1. Добавление основного репозитория
```bash
git remote add upstream https://github.com/AsnDen/corvax-lore.git
```

### 2. Получение обновлений
```bash
git fetch upstream
git checkout main      # Переключиться на основную ветку
git merge upstream/main # Объединить изменения
git push origin main   # Обновить ваш форк
```

---

## 🆘 Помощь и советы

### Частые проблемы
1. **Конфликты версий**:  
   Если GitHub пишет "This branch has conflicts" — [руководство по решению](https://docs.github.com/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts)

2. **Потеря изменений**:  
   Всегда делайте `git commit` перед закрытием терминала

### Где задавать вопросы?
- В комментариях к вашему PR
- В нашем [Discord-чате](https://discord.gg/corvax)
- Через Issues в репозитории

---

## 📚 Полезные ссылки
1. [Интерактивный учебник по Git](https://learngitbranching.js.org/)
2. [Официальная документация GitHub](https://docs.github.com/ru)

**Не бойтесь ошибаться!** Даже опытные разработчики постоянно учатся.  
Ваш вклад важен для нас! 