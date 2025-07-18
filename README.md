# Система сбора параметров с вычислительных устройств для системы мониторинга
В репозитории представлены: прототип системы мониторинга параметров, а также анализ данных вибрационных показателей электродвигателей. 

1. Мониторинг метрик производительности компьютера:

Цель: сбор и отслеживание метрик производительности ПК.

Файлы:
  - monitoring.py — скрипт сбора метрик
  - dashboard.py — визуализация данных
  - metrics_log.csv — журнал собранных данных
  - monitoring.log — лог работы скрипта

Функционал:
Регулярный сбор данных о загрузке CPU, использовании RAM
Сохранение метрик в CSV
Вывод графиков и диаграмм через matplotlib
- Загрузка процессора
- Использование оперативной памяти
- Использование дискового пространства
- Сетевая активность
- Средняя нагрузка системы

Данные собираются с интервалом и сохраняются в CSV-файл. Для визуализации используется веб-интерфейс на [Streamlit](https://streamlit.io ).

___

## Инструкция по запуску

### 1. Установите зависимости:
```pip install psutil pandas streamlit plotly```

### 2. Запустите сбор метрик:
```python monitoring.py```

### 3. Запустите дашборд в отдельном окне терминала:
```python -m streamlit run dashboard.py```
___

## Что можно делать в интерфейсе
- Выбрать временной диапазон отображения данных
- Включить автообновление с заданным интервалом
- Посмотреть графики загрузки CPU, RAM, диска и сети
- Увидеть сырые данные в таблице

___

## Возможные доработки
- Добавить систему оповещений при превышении пороговых значений
- Сохранять данные в БД (например, InfluxDB или PostgreSQL)

___

![image](https://github.com/user-attachments/assets/1b0c8425-8080-4b5e-b2c0-2caa4905bf6d)
![image](https://github.com/user-attachments/assets/956f2ce4-ce84-464b-879b-3d15d2e007b9)
![image](https://github.com/user-attachments/assets/8ba4f2b2-9ea2-474e-82f9-3ce664452954)

2. Анализ данных проомышленных двигателей

Цель: исследование и предварительная обработка данных с двигателей.

Файл:
- engines.ipynb — Jupyter Notebook с анализом

Что сделано:

- Загрузка и осмотр данных
- Построение визуализаций 
- Визуализация вибрационных параметров
- Анализ корелляций
- Постановка задачи классификации

![image](https://github.com/user-attachments/assets/941c1565-7007-4b32-a602-0ed9282edf27)
![image](https://github.com/user-attachments/assets/d1a9a017-3a63-40f7-b932-1e17add3f863)
![image](https://github.com/user-attachments/assets/9d36cd46-44a2-40ea-bf89-45d347d39c4b)
![image](https://github.com/user-attachments/assets/096f3607-799e-4c7d-91c0-63221a200cba)
![image](https://github.com/user-attachments/assets/49f0e72a-65d4-4b94-a008-1907eb3e5f53)
![image](https://github.com/user-attachments/assets/17e1bfed-fa6a-4bea-bde9-6156130cb8c8)




