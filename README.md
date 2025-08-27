# tg-scrape-comments

CLI для выгрузки **постов и комментариев** из публичных Telegram-каналов в **JSONL** (отдельный файл на канал).  
Реализация на [Telethon]. Логин — через ваш Telegram-аккаунт (номер/код/2FA).

- Python ≥ 3.10
- Поддерживаемые ОС: Linux, macOS, Windows

## Установка

### Из PyPI (для всех)
```bash
pip install tg-scrape-comments

## Быстрый старт

1. Получите ключи на https://my.telegram.org → **API development tools** (API ID и API HASH).
2. Запустите скрейпер (пример — первые 5 постов для проверки):
   ```bash
   tg-scrape @durov --out-dir ./out --post-limit 5 \
     --api-id 123456 --api-hash xxxxxxxxxxxxxxxxxxxxxxxx
3. При первом запуске вы введёте номер телефона, код из Telegram и (если включено) пароль 2FA. Будет создан файл сессии.
