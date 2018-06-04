# matplotlib

## Основные элементы
**Figure**

Самый верхний объект изобржанеия, который включает все остальные элемены: графики, подписи.
Создание объекта Figure и установка заголовка для него:

    import matplotlib.pyplot as plt
    fig = plt.figure()
    fig.suptitle('Main title')
    fig.show() # или plt.show()

Упрощенный вариант:

    ptl.suptitle('Main title')
    plt.show()

**Axes**

Непосредственно сам график, с осями и подписями к ним представляется объектом Axes. Одни объект Figure может содержать несколько объектов Axes. Объек Axes создается с помошью метода `fig.subplots()`. Метод `subplots` имеет несколько форм:

    ax = fig.add_subplot(rows, cols, index)
    ax = fig.add_subplot(rci) # если rows*cols < 10, то rows, cols, index можно заменить на трехзначное число rci
    fig, (ax1, ax2,...,axN) = fig.subplots(rows, cols) # N = rows*cols

Упрощенный вариант:

    plt.<функция_рисования_графика>(... # если создается один subplot, то явно Figure и Axes можно не создавать
    # для нескольких subplot-ов:
    plt.subplot(rci)

Установка заголовка для subplot-а:

    ax.set_title('Subplot title')
    # упрощенный вариант
    plot.title('Subplot title') # применяется к текущему subplot-у

    
    
