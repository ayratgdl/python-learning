# Пакеты для работы с математическими понятиями

## math
Модуль `math` входит в стандартную бибилиотеку и содержит базовые математические функции и константы.
Сайт: https://docs.python.org/3/library/math.html#module-math

Примеры функций:

    math.ceil(x) # округление до целого сверху
    math.floor(x) # округление до целого снизу
    math.log(x) # логорифм (по основанию e) числа x
    math.log10(x) # десятичный логорифм
    math.sqrt(x) # квадратный корень
    math.sin(x)
    math.cos(x)
    math.pi # константа pi
    math.e # констатна e

## random
Модуль `random` входит в стандартную библиотеку и содержит функции для генерации псевдослучайных чисел.
Сайт: https://docs.python.org/3/library/random.html#module-random

Примечание: Последовательность сгенерированных чисел с математической точки зрения обладает всеми свойствами случайных чисел.
Но эта последовательность может быть точно предсказана. Поэтому они могут использоваться только для целей математического
анализа, но не для криптографии и защиты данных.

Примеры функций:

    randon.seed(x) # Инициализирует генератор. По умолчанию инициализируется системным временем. x - целое число.
    random.random # вовращает float в диапазоне [0.0; 1.0)
    random.randrange(from, to) # возвращает число от from до to-1
    random.choise(seq) # возвращает случайный элемент из последовательности seq

## statistics
Модуль `statistics` входит в стандартную библиотеку и содержит статистические функции.
Сайт: https://docs.python.org/3/library/statistics.html#module-statistics

Примеры функций:

    statistics.mead(seq) # среднее
    statistics.median(seq) # медиана

## matplotlib
Библиотека для построения графиков
Сайт: https://matplotlib.org/index.html

Установка

    pip install -U matplotlib

Простой пример

    import matplotlib.pyplot as plt
    plt.plot(range(0, 101), [x**2 for x in range(0, 101)])
    plt.show()
    
