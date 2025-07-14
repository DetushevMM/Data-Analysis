# 📊 Анализ данных: проекты

Коллекция аналитических проектов, охватывающая различные области - от финансов до социальных инициатив.

## 📋 Список проектов

| № | Проект | Описание | Технологии | Ключевые результаты |
|---|--------|----------|------------|---------------------|
| 1 | [Анализ KIVA](Analysis%20of%20KIVA%20activities.ipynb) | Исследование микрокредитной платформы | Pandas, Seaborn | Выявлены топ-страны по займам |
| 2 | [Прогноз авиатрафика](Forecasting%20passenger%20traffic%20and%20airline%20sales.ipynb) | Прогнозирование спроса на авиабилеты | Prophet, Matplotlib | Сезонные паттерны спроса |
| 3 | [Рейтинг акций Google](Google_Stock_Trust_Rating.ipynb) | Анализ доверия к акциям | NLTK, TextBlob | Sentiment анализ новостей |
| 4 | [Анализ рейтингов фильмов](Movie%20rating%20analysis.ipynb) | Исследование кинопредпочтений | Plotly, Sklearn | Корреляция бюджета и оценок |

##  🔍 Подробнее о проектах
1. Анализ KIVA
Исследование распределения займов по странам

Визуализация с Seaborn:

  sns.barplot(x='country', y='loan_amount', data=top_countries)

2. Прогноз авиатрафика
Прогнозирование методом Facebook Prophet

Анализ сезонности:

  model = Prophet(seasonality_mode='multiplicative')
  
  model.fit(df)

3. Рейтинг акций Google
Сентимент-анализ новостей

Обработка естественного языка:

  from textblob import TextBlob
  
  blob = TextBlob(news_text)
  
  sentiment = blob.sentiment.polarity

4. Анализ фильмов
Интерактивная визуализация с Plotly

Кластеризация фильмов:

  fig = px.scatter(df, x='budget', y='rating', color='genre')
  
  fig.show()

## 🛠 Технологический стек
```python
# Основные инструменты
import pandas as pd  # Анализ данных
import matplotlib.pyplot as plt  # Визуализация
from fbprophet import Prophet  # Прогнозирование
import plotly.express as px  # Интерактивные графики
