### BMSTU

#### Выпускная квалификационная работа по курсу "Data Science"
#### Тема "Прогнозирование конечных свойств новых материалов (композиционных материалов)"
#### Слушатель Горшков Андрей Вячеславович

Модели целевых переменных построены на трех вариантах наборов данных – базовый датасет (первые 23 строки), полный датасет (1023 строки) и очищенный от шума датасет.
Для очистки датасета от шума разработан фильтр, ядром (маской) которого являются объекты базового датасета.
На данных очищенного датасета для целевых переменных 'Модуль упругости при растяжении' и 'Прочность при растяжении' обучены модели регрессоров, для которых наибольшие 𝑅^2 = 0,490 и 𝑅^2 = 0,737, соответственно. Для целевой переменной 'Соотношение матрица - наполнитель' обучена модель нейронной сети, для которой 𝑅^2 = 0,227.
