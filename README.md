# Labs_AD
Labs_1

Лабораторна робота 1

Базові алгоритми машинного навчання (from scratch, тільки Python і numpy)

1. Лінійна регресія (1D)

Згенеруйте синтетичний набір точок виду y = ax + b + noise. Візуалізуйте результат за
допомогою (matplotlib). Вирішіть задачу лінійної регресії для такого набору точок.
Параметри моделі знайдіть за допомогою градієнтного спуску. Порівняйте знайдені
параметри із значеннями (a, b).

2. Логістична регресія (2D)

Згенеруйте два синтетичних набори точок на площині, додайте ім мітки класів (0 і 1).
Візуалізуйте результат за допомогою (matplotlib). Розділіть дані на класи за допомогою
логістичної регресії. Перевірте якість алгоритма за допомогою метрики accuracy (на
тестових даних).


Labs_2

Лабораторная робота 2

Базові алгоритми класифікації з використанням бібліотеки sklearn

Провести навчання і класифікацію даних. Виконати наступні процедури:
1) Завантажити дані, вивести на екран назви колонок і розмір датасета
2) Опрацювати пропуски (по можливості заповнити їх або видалити)
3) Візуалізувати дані: побудувати графік (heatmap), що відображає кореляції
ознак між собою і з цільовою змінною (розміткою); побудувати гістограми
розподілу ознак і boxplot-и ознак відносно цільової змінної (якщо ознак занадто багато
обмежитися декількома)
4) нормалізувати дані
5) провести навчання наступних класифікаторів
- kNN
- дерево прийняття рішень і візуалізувати його
- SVM
- Random Forest
- AdaBoost

Підібрати оптимальні параметри для
- NN
- я SVM за допомогою GridSearch підібрати оптимальні «C» і «gamma»
- за допомогою GridSearch підібрати оптимальні параметри для Random Forest і AdaBoost

Серед обраних оптимальних моделей кожного класу вибрати найкращу. Відобразити
sklearn.metrics.classification_report і sklearn.metrics.confusion_matrix

Labs_3
1. Зниження розмірності і візуалізація даних
Застосуйте методи зниження розмірності sklearn.decomposition.PCA і
sklearn.manifold.TSNE для візуалізації даних, з якими ви працювали в лабораторній No 2
(знижуючи розмірність до двох). Візуалізуйте результат.

2. Кластерний аналіз

   а) За допомогою алгоритму k-means зробіть квантування зображення (видалення
візуально надлишкової інформації) з глибиною 64, 32, 16 та 8 рівнів для будь-якого
обраного самостійно зображення.

Приклад: https://scikit-learn.org/stable/auto_examples/cluster/plot_color_quantization.html

   б)Згенеруйте набір синтетичних даних у вигляді суміші двох гаусіан за допомогою функції:

https://docs.scipy.org/doc/numpy-1.13.0/reference/generated/numpy.random.multivariate_normal.html

(застосуйте її двічі з різними mean і cov, результат об’єднайте)

Розділіть суміш за допомогою EM алгоритму (sklearn.mixture.GaussianMixture), зверніть
увагу на параметр covariance_type. За допомогою атрибутів weights_ і covariances_
відновіть їхні значення, порівняйте з оригінальними. Візуалізуйте результат.

3. Обробка текстових даних

Завантажте набір текстових даних (з мітками класів). Проведіть передобробку даних
(видаліть стоп-слова, пунктуацію), за допомогою wordcloud зробіть візуалізацію найбільш
поширених слів або n-gram у кожному класі. Векторизуйте тексти (наприклад за
допомогою sklearn.feature_extraction.text .TfidfVectorizer). Проведіть класифікацію
текстових даних, зробіть оцінку якості. Застосуйте алгоритм LDA до кожного класу,
визначте декілька тематик (sklearn.decomposition.LatentDirichletAllocation)

