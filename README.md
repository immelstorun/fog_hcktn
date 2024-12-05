# Проектное исследование на основе открытых данных в области биомедицины

Исcледование разделено на 2 раздела - бейзлайн на основе нейронной архитектуры (freezingofgate-mipt_DL.ipynb) и решение на основе классического градиентного бустинга (freezingofgate-mipt_ML.ipynb).

Выполнил Алексей Сейкин Алексей Осипов

В данном прототипе решения приводится исследовательский анализ данных по пациентам с двигательными нарушениями (FOG) при болезни Паркинсона. В прототипе решения приведено применение градиентного бустинга. Методы глубоко обучения в данном решении не рассматриваются, поскольку находятся в стадии разработки.

Примечание: FOG - это сокращение от "Freezing of Gait", что означает замораживание походки.

Задача - классификация типа двигательного события по данным, собранных носимыми акселерометрами. Разметка данных акселерометров по типам событий произведена вручную экспертами, по видозаписям, покадрово.

Открытые данные для анализа - [70 Gb](https://www.kaggle.com/competitions/tlvmc-parkinsons-freezing-gait-prediction/data)

Для воспроизведения требуется видеоускоритель.

# Выводы

Сравнительный анализ результатов данного исследования показывает, что при тщательной подготовке признаков методы классического ML не уступают нейронным архитектурам. В данном случае для Нейронной сети был создан признак категории - скользящее окно. И Для дальнейших исследований остается еще очень большое поле деятельности.

Оптимизация нейронной сети проводилась в 7 эпох - как демонстрация подхода.
Validation Loss: 0.0891, Validation Score: 0.252, ClassWise: 0.046,0.667,0.043
