# Sports Analytics Pro

Продвинутое учебное приложение для спортивной аналитики.

**Возможности:**
- Реальные матчи через API-Football
- Коэффициенты через The Odds API
- Поиск value-ставок и Kelly Criterion
- Управление банкроллом
- Журнал ставок
- Мобильная адаптация
- Работает на демо-данных без ключей

---

## Быстрый запуск локально

```bash
pip install -r requirements.txt
streamlit run app.py
```

---

## Деплой на Streamlit Community Cloud (рекомендуется)

### 1. Создайте репозиторий на GitHub

1. Зарегистрируйтесь / войдите на [GitHub](https://github.com)
2. Создайте новый репозиторий (например `sports-analytics-pro`)
3. Загрузите все файлы из этой папки:
   - `app.py`
   - `requirements.txt`
   - `README.md`
   - папку `.streamlit/` с файлом `config.toml`

### 2. Подключите к Streamlit Cloud

1. Зайдите на [share.streamlit.io](https://share.streamlit.io)
2. Войдите через GitHub
3. Нажмите **New app**
4. Выберите ваш репозиторий
5. Main file path: `app.py`
6. Нажмите **Deploy**

Через 1–2 минуты вы получите публичную ссылку вида:
```
https://sports-analytics-pro-xxxxx.streamlit.app
```

Эту ссылку можно открывать с iPhone и добавить на домашний экран.

### 3. Добавьте API-ключи (секреты)

1. В настройках приложения на Streamlit Cloud откройте **Settings → Secrets**
2. Вставьте:

```toml
API_FOOTBALL_KEY = "ваш_ключ_от_rapidapi"
ODDS_API_KEY = "ваш_ключ_от_the_odds_api"
```

3. Сохраните. Ключи подставятся автоматически.

---

## Как получить бесплатные API-ключи

### API-Football
1. https://rapidapi.com/api-sports/api/api-football
2. Зарегистрируйтесь → подпишитесь на бесплатный план
3. Скопируйте `X-RapidAPI-Key`

### The Odds API
1. https://the-odds-api.com
2. Зарегистрируйтесь
3. Скопируйте API Key (500 запросов/месяц бесплатно)

---

## Структура проекта

```
sports_app/
├── app.py                 # Основное приложение
├── requirements.txt       # Зависимости
├── README.md              # Документация
└── .streamlit/
    └── config.toml        # Тема и настройки
```

---

## Важно

Это **учебный** инструмент.  
Ставки на спорт связаны с риском потери денег.  
Играйте ответственно (18+).  
Прошлые результаты не гарантируют будущую прибыль.
