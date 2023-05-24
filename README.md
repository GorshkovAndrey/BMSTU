### BMSTU

#### Выпускная квалификационная работа по курсу "Data Science"
#### Тема "Прогнозирование конечных свойств новых материалов (композиционных материалов)"
#### Слушатель Горшков Андрей Вячеславович
------------------------------------------

Математические модели целевых переменных построены на трех вариантах наборов данных – базовый датасет (первые 23 строки), полный датасет (1023 строки) и очищенный от шума датасет.

По данным базового датасета выявлены линейные функциональные зависимости для целевых переменных 'Модуль упругости при растяжении' и 'Прочность при растяжении' от признаков 'Поверхностная плотность' и 'Потребление смолы'.

На данных полного датасета построить неконстантные модели с обобщающей способностью для целевых переменных не удалось. Значения коэффициентов детерминации 𝑅2 для обученных моделей получились практически нулевыми.

Для оценки принципиальной возможности построения неконстантных моделей на данных полного датасета вычислялся множественный коэффициент корреляции (аналитический коэффициент детерминации). В результате проведенных расчетов множественного коэффициента корреляции сделаны следующие выводы:
- на данных полного датасета построить неконстантные модели с обобщающей способностью для целевых переменных в принципе невозможно, т.к. большую часть полного датасета составляет шум;
- для построения пригодных для практического применения неконстантных моделей с обобщающей способностью необходимо полный датасет очистить от шума. 

Для очистки полного датасета от шума разработан фильтр, ядром (маской) которого являются объекты (элементы) базового датасета.

На данных очищенного датасета для целевой переменной 'Модуль упругости при растяжении' обучены модели различных регрессоров, для которых коэффициент детерминации на тестовой выборке составил 𝑅2 = 0,7 – 0,86.

На данных очищенного датасета для целевой переменной 'Прочность при растяжении' обучены модели различных регрессоров, для которых коэффициент детерминации на тестовой выборке составил 𝑅2 = 0,73 – 0,83.

Для целевой переменной 'Соотношение матрица - наполнитель' обучена модель полносвязной нейронной сети, для которой коэффициент детерминации на тестовой выборке составил 𝑅2 = 0,38.
