# Исследование данных Spotify
## Введение
Этот проект представляет собой комплексное исследование данных Spotify, включающее предварительный анализ данных, инженерию признаков и создание полносвязной нейронной сети для рекомендаций музыки. 

---

## цель исследования
разработать эффективную систему рекомендаций музыки, использующую данные Spotify для предсказания популярности песен и предложения пользователю похожих треков. Задача заключается в выявлении ключевых факторов, влияющих на успех песни, и использовании этой информации для улучшения рекомендаций.

---

## Основные этапы работы
1. Извлечение данных из API Spotify
2. Проведение предварительного анализа данных
3. Инженерия признаков
4. Создание полносвязной нейронной сети для прогнозирования популярности песен

---

## методы работы
1. **Извлечение данных**: используются данные о характеристиках треков в формате csv
2. **Предварительный анализ данных**:
  1. Анализируется распределение популярности песен
  2. Исследуются корреляции между различными характеристиками треков
  3. Выявляются тренды в popularity
3. **Инженерия признаков**:
  1. Преобразуются категориальные переменные в числовые
  2. Создаются новые признаки на основе существующих
  3. Выбираются наиболее важные признаки для прогнозирования popularity
4. **Создание модели**
  1. Разработана полносвязная нейронная сеть с несколькими слоями
  2. Использована функция активации ReLU и регуляризация
  3. Применена кросс-валидация для оценки производительности модели

---
## Результаты и обсуждение

Эксперименты показали эффективность модели в предсказании популярности песен на основе их аудио-функций и метаданных. Однако были выявлены следующие вызовы:
- Низкая корреляция между признаками и целевой переменной popularity
- Асимметричное распределение popularity в данных
- Скудость данных для очень популярных песен
Для улучшения результатов рассмотрены следующие подходы:
- Удаление менее популярных песен из набора данных
- Применение методов балансировки данных
