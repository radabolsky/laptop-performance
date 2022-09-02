# laptop-performance


Для реализации регрессионного анализа согласно алгоритма могут пригодиться:

* [Google Colab](https://colab.research.google.com/?utm_source=scs-index) или [Jupyter Notebook](https://jupyter.org/) для того, чтобы выполнять код построчно и экспериментировать с данными
* [pandas](https://pandas.pydata.org/) - для удобной работы с данными в виде таблицы
* [numpy](https://numpy.org/) - для работы с векторами чисел и быстрой обработки массивов
* [matplotlib.pyplot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.html) - для работы с графиками
* [statsmodels](https://www.statsmodels.org/stable/index.html) - библиотека для построения моделей
* [scipy.stats](https://docs.scipy.org/doc/scipy/reference/stats.html) - для работы со статистикой


<img src="flow-charts/main.png" alt="База" title="База" align="center">

## Подготовка данных к анализу

стр 38


Данные приходят в виде .csv файла. Его нужно распарсить и обработать согласно блок-схеме. Некоторые числа могут считываться как строки, их нужно привести к соответствующему формату (float, int и т.д.). Лучше всего для этого подходит [pandas](https://pandas.pydata.org/docs/). Также может пригодиться One-hot-encoding, чтобы вручную не обрабатывать номинальные (категориальные) признаки


<img src="flow-charts/preprocessing.png" alt="Предобработка" title="Предобработка" align="center">


## Анализ критических значений

стр 39


В этой части необходимо проанализировать данные, полученные после предобработки (они будут в формате DataFrame, см pandas), и удалить данные не соответсвующие условиям согласно алгоритма. Для построения диаграмм - [matplotlib.pyplot](https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.boxplot.html). Также может пригодится [scipy.stats](https://docs.scipy.org/doc/scipy/reference/stats.html)



<img src="flow-charts/critical-values.png" alt="Критические значения" title="Критические значения" align="center">


## Построение регрессии

стр 29


стр 42


стр 70


На этом этапе строится модель согласно алгоритму. Для построения могут пригодится: [sklearn.linear_models](https://scikit-learn.org/stable/modules/linear_model.html), [scipy.stats](https://docs.scipy.org/doc/scipy/reference/stats.html)



<img src="flow-charts/regression.png" alt="Регрессия" title="Регрессия" align="center">



## Проверка работоспособности модели

стр 46


Готовую модель нужно проверить согласно алгоритму:


<img src="flow-charts/validation.png" alt="Валидация" title="Валидация" align="center">
