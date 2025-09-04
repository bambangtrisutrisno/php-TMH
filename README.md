# 🎵 php-TMH — Telegram Music Hub (by TCSE)

**Telegram Music Hub** — это open-source система, позволяющая **управлять музыкой и контентом через Telegram-бота**, а отображать его на сайте.

> 🔗 [Демо: tmh.tcse-cms.com](https://tmh.tcse-cms.com)  
> 💬 [Telegram-канал: @chuyakov_project](https://t.me/chuyakov_project)

---

## 🔧 Особенности

- ✅ Автоматический блог из Telegram-канала
- ✅ Загрузка аудио через Telegram
- ✅ Веб-плеер с PWA-поддержкой
- ✅ Плейлисты: M3U, PLS, XSPF
- ✅ Модерация, роли, статистика
- ✅ Безопасный прокси для медиа
- ✅ Mobile-first дизайн
- ✅ Альбомы фото (галерея)
- ✅ Темная/светлая тема

---

## 📁 Структура проекта
/tmh/

├── index.html          # Главная (агрегатор)

├── blog.html           # Блог с фото и аудио

├── player.html         # Веб-плеер

├── config.php          # Единая конфигурация

├── .htaccess           # Роутинг и безопасность

├── core/               # PHP-движок

├── data/               # Базы и логи

└── assets/             # CSS, JS, изображения


---

## 🚀 Установка

1. **Склонируйте репозиторий**:
   ```bash
   git clone https://github.com/tcse/php-TMH.git

2. Загрузите на хостинг в папку /tmh 

3. Создайте бота через @BotFather  и получите bot_token 

4. Настройте config.php:
```
   'bot_token' => 'YOUR_BOT_TOKEN',
'base_url' => 'https://your-site.com/tmh',
'channel' => [
    'channel_username' => 'your_channel_username'
],
'moderation' => [
    'admin_chat_ids' => ['YOUR_CHAT_ID']
]
```
6. Запустите вебхук: https://your-site.com/tmh/core/set_webhook.php 
7. Добавьте бота администратором в канал 

Готово! Бот активен. 
