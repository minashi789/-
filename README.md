# Анализ и прогнозирование объёма производства электроэнергии

## Описание

Данный проект представляет собой анализ динамики производства электроэнергии за период с 2010 по 2023 год и построение прогноза на 2024 год. В работе используются методы статистического анализа и линейной регрессии.

## Данные

Данные об объёме производства электроэнергии представлены в виде pandas DataFrame и включают следующие столбцы:

*   `Year`: Год (2010-2023).
*   `Production`: Объём производства (TWh).

Данные создаются непосредственно в коде:

```python
import pandas as pd

data = pd.DataFrame({
    'Year': [2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023],
    'Production': [22811, 23084, 23113, 23347, 23710, 24293, 24685, 25058, 25472, 25750, 26368, 27070, 28411, 29281]})
```
## Методы анализа
*В проекте используются следующие методы:

* Расчёт основных статистических показателей:
* Суммарный объём производства по годам.
* Абсолютная динамика (изменение объёма производства между годами).
* Темп роста (в процентах).
* Темп прироста (в процентах).
* Средняя геометрическая.
* Средняя абсолютная динамика.
* Средний темп роста.
* Средний темп прироста.
* Визуализация данных: Построение графиков объёма производства, абсолютной динамики, темпа роста и темпа прироста.
* Проверка нормальности распределения: Использование тестов Шапиро-Уилка и критерия согласия Пирсона (хи-квадрат).
* Корреляционный анализ: Построение корреляционного поля.
* Линейная регрессия: Построение модели линейной регрессии для прогнозирования объёма производства на основе года.
* Прогнозирование: Прогноз объёма производства на 2024 год на основе среднего абсолютного прироста.

## Требования

* Python 3.7+
* pandas
* numpy
* matplotlib
* scipy
* statsmodels

## Запуск

* Клонировать репозиторий: git clone https://github.com/minashi789/Kursovaya
* Установить зависимости: pip install -r requirements.txt (создайте файл requirements.txt с перечисленными выше библиотеками)
* Запустить код: python main.py (или запустить Jupyter Notebook).
