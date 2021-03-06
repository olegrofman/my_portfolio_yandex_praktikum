**Название проекта**: Машинное обучение моделей по прогнозированию оттока клиентов сети фитнес-центров

**Цели и задачи проекта**: 

Провести анализ данных сети фитнес-центров с целью разработки прогноза вероятности оттока клиентов и последующей подготовки стратегии по их удержанию. Входными данными
являются анкеты клиентов фитнес-центра, объединённые в датасет по ряду признаков, включающих пол и возраст клиента, район проживания/работы относительно фитнес-центра, участие клиента в партнёрской программе, использование промо-кода, наличие контактного телефона и время с момента первогообращения. Во входных данных также содержится информация на основе журнала посещений, где указана длительность абонемента и срок его истечения, факт посещения групповых занятий, средняя частота посещений фитнес-центра, суммарная выручка от использования других услуг центра. В данных также отражен факт оттока в текущем месяце.

**План работы** над проектом включает в себя выполнение следующих шагов:

- *Импорт данных и предобработка данных.* На этом этапе получаем общую информацию об имеющихся у нас в распоряжении данных, их типах, полноте и правильности представления. Предварительно оцениваем объем данных в исходном датасете, а также присутствие пропусков и дубликатов. Обращаем пристальное внимание на недостатки исходных данных и их релевантность: анализируем пропуски (если есть), приводим названия колонок-признаков к нижнему регистру, преобразуем данные в верный тип, проверяем их на присутствие ошибочных значений и обрабатываем дубликаты с целью исключения искажений в результатах.

- *Исследовательский анализ данных.* Изучим средние значения и стандартные отклонения, характерные для каждого признака в датасете. Рассмотрим средние значения признаков применительно к двум группам — тех, кто ушел в отток и тех, кто остался. Построим гистограммы распределения признаков для тех, кто ушёл(отток) и тех, кто остался (не попали в отток). Сформируем матрицу корреляций признаков с целью проверки на наличие сильной линейной корреляции между парами признаков.

- *Построение модели прогнозирования оттока клиентов.* В данной части работы, построим модели бинарной классификации клиентов, с использованием обучающих алгоритмов на основе логистической регрессии и "случайного леса". Оценим качество предсказаний моделей на валидационной выборке с использованием метрик. Выделим модель, которая показала себя лучше на основании метрик.

- *Кластеризация клиентов.* Эта часть проекта будет направлена на построение матрицы расстояний между признаками, с последующим получением дендрограммы связей. В результате будет выделено число кластеров, по которым модель может разделить клиентов. Следующим шагом будет разработка связанной модели кластеризации с использованием алгоритма K-Means. В заключение, построим распределения признаков для кластеров и для каждого полученного кластера посчитаем долю оттока клиентов. Проанализируем полученные результаты.

- *Общие выводы и рекомендации.* На заключительном этапе приводится сумма выводов и рекомендаций по каждой части выполненного проекта. В общем выводе, на основе имеющихся данных и анализа, мы отразим ключевые рекомендации для владельцев фитнес-клуба по стратегии взаимодействия с клиентами и их удержания.

**Ключевые слова проекта:** KMeans, Machine Learning, RandomForestClassifier, LogisticRegression, дендрограмма

**Навыки и инструменты:**: ```Python```, ```Pandas```, ```Scikit-learn```, ```Matplotlib```, ```Seaborn```, машинное обучение, классификация, кластеризация
