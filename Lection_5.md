# Тестирование гипотез (параметрические тесты)
## Алгоритм проведение тестирования гипотез
В реальной жизни часто прибегают к выборочному контролю. Предположим, у нас есть случайная величина (далее СВ) «Рост». Мы берем первую выборку, измеряем по ней среднее арифметическое и получаем некоторую точечную оценку генеральной совокупности, затем можем взять еще одну выборку и получить по ней новую точечную оценку генеральной совокупности, потом взять третью выборку и снова получить  какую-то новую точечную оценку генеральной совокупности и т.д. Т.е. точечная оценка будет меняться от выборки к выборке. Т.е. средняя по выборке есть случайная величина. Значит, мы не можем взять какую-то одну точечную оценку и сказать, что вот именно эта точечная оценка и будет истинным средним арифметическим всей генеральной совокупности. Не можем, потому что мы этого не знаем наверняка. И вот здесь нам как раз и помогает такой метод, как тестирование гипотез. Он позволяет нам сравнивать параметры распределений. Т.е. с помощью тестирования гипотез мы хотим ответить на вопрос видим ли мы статистически значимые различия, например, между 2мя средними арифметическими. Что это значит?
Еще раз вспомним центральную предельную теорему, которая гласит, что среднее выборочное стремится к нормальному распределению с Mu таким же, как у генеральной совокупности и дисперсией, равной дисперсии генеральной совокупности, деленой на объем выборки. 
Т.е. средняя выборочная – это случайная величина, т.е. меняется от выборки к выборке, иным словами, это не фиксированное одно и то же значение, которое мы будем получать во всех выборках. (Еще раз посмотрите на знакомый уже рисунок, где изображено распределение среднего выборочного значения)
![Alt text](image-14.png)

Т.о. если различия случайны, то мы считаем, что различий между тем, что мы измерили и тем, что заявлено поставщиком о генеральной совокупности, не являются статистически значимыми. Но если различие велико, то мы обнаруживаем статистически значимое различие.

Статистическая гипотеза – это предположение о неизвестном распределении случайных величин, соответствующих каким-либо представлениям о том явлении, которое изучается.

При тестировании гипотез формулируется 2 гипотезы. Одна из них нулевая, которая гласит, что различий нет, и противоположная гипотеза, альтернативная, которая заявляет, что  есть статистически значимые различия.

## Метод тестирования гипотез имеет определенный алгоритм.
	
1. Формулирование нулевой  H_0 и  альтернативной гипотез H_1
2. Выбор уровня статистической значимости α
3. Выбор статистического критерия
4. Расчет наблюдаемого критерия
5. Сравнение табличного и наблюдаемого значений критерия
6. Вывод

### Нулевая гипотеза  H_0 и  альтернативная гипотез H_1
Нулевая и альтернативная гипотезы – это две противоположные гипотезы. Если принимается нулевая гипотеза, то альтернативная гипотеза отвергается, и наоборот, если принимается альтернативная, то нулевая отвергается. 

Нулевая гипотеза H_0 всегда звучит едино. Различий нет. Математически мы можем записать это, как μ=μ_0. Пока не будет доказано, что верна альтернативная гипотеза, верной считается H_0.
𝐻_0: μ = μ_0

В альтернативную гипотезу H_1 мы вкладываем наше заявление о статистически значимых различиях. Она может быть сформулирована тремя способами, все зависит от поставленной задачи.

	μ > μ_0 (вариант для нашего примера, т.к. мы получили μ = 10.3 больше, чем заявлял производитель)
	μ < μ_0
	μ ≠ μ_0 (двусторонний тест)

![Alt text](image-15.png)

## Выбор уровня статистической значимости α
Чаще всего для  α выбирают значения: 
0.01  (1%)
0.05  (5%)
0.1   (10%)

## Выбор статистического критерия и вывод
Критерии делятся на параметрические и непараметрические. Z и t критерии применяются для параметрических тестов. 

Идея теста сводится к тому, чтобы найти расчетное значение и сравнить его с табличным значением, соответствующим выбранному уровню значимости  α.

Z критерий - известна 𝞼  генеральной совокупности

t - критерий (критерий Стьюдента) - если 𝞼 генеральной совокупности  неизвестна

### Расчет наблюдаемого критерия

![Alt text](image-18.png)

![Alt text](image-22.png)

Пример: Диаметры следуют нормальному распределению и пусть у нас известно среднее квадратичное отклонение генеральной совокупности, равное 1 мм. Значит, нам следует использовать критерий Z. Производитель заявляет среднее арифметическое 10 мм, но мы получили 10.3 мм и к тому же мы знаем сигму генеральной совокупности. Давайте измерим расстояние в универсальной единице измерения в нормальном распределении, а именно посмотрим, а в скольких сигмах лежит 10.3 мм от 10 мм. 10.3-10 = 0.3 мм. Сколько же сигм лежит в этом отрезке 0.3 мм. 

В условии задачи нам дана сигма генеральной совокупности 1 мм. Значит, сигма для изображенного ниже распределения на рисунке, будет являться стандартной ошибкой среднего (SE). Согласно центральной предельной теореме SE = 𝞼/√n. Поскольку выборка была из 16 деталей, то  получаем 1/4.

![Alt text](image-20.png)

Осталось посчитать в скольких SE 10.3 лежит от 10 мм.
(10.3-10)/ (1/4) = 1.2
1.2 – это наш расчетный Z критерий по выборке.
А вот табличный критерий надо найти для α = 5%. Поскольку на рисунке α отсекает 0.05 справа, то ниже отсечки лежат 0.95 или 95% всех значений стандартного нормального распределения. По таблице Z-значений сначала ищем долю 0.95 ( обвела в рамочку на рисунке ниже). А потом смотрим, на пересечении каких составных частей Z лежит эта доля. Т.е. мы делаем обратное действие тому, которое изучили на прошлом уроке. Приблизительное Z табличное 1.645

![Alt text](image-21.png)

Получается, что расчетное значение 1.2 попадает в область принятия гипотезы H_0. Оно меньше 1.645. Т.е. делаем вывод, что верна нулевая гипотеза о том, что размер деталей на самом деле и есть 10 мм на уровне значимости 5%.

## Ошибки при тестировании гипотез.
Ошибка I рода : мы отвергаем Н0,когда она верна 

 Уровень значимости  α –вероятность ошибки I рода
 
Ошибка II рода : мы принимаем Н0,когда она неверна

 β- вероятность ошибки II рода 

 (1- β)–мощность теста – вероятность отклонить Н0, когда верна Н1 

 ![Alt text](image-23.png)

## Критерий Стьюдента.
Если **неизвестна сигма генеральной совокупности** и соблюдаются остальные условия применимости параметрических тестов, то следует использовать критерий Стьюдента. 
Как и любой тест гипотезы, идея та же. Найти расчетное значение критерия и сравнить с табличным. Формула для нахождения расчетного критерия та же.
Сигму рассчитываем по выборке, используем формулу для **несмещенного стандартного отклонения**. Для нахождения табличного значения используем таблицу распределения Стьюдента.
Распределение Стьюдента зависит от степеней свободы. Степени свободы здесь будут находиться как разность объема выборки и 1. Т.е. распределение Стьюдента зависит от объема выборки. С увеличением объема выборки оно стремится к нормальному стандартному распределению.
Например, по таблице ниже найдем табличное значение для α = 5%. На графике заштрихована площадь p, а α не заштрихована. Значит, надо найти p = 95%. И, предположим, что объем выборки был 10. Т.е. 9 степеней свободы. Табличное значение будет равно 1,833. 

![Alt text](image-24.png)

Таблица Стьюдента    https://fsd.multiurok.ru/viewImage.php?image=http://nice-diplom.ru/templates/blue/images/img/form_69.gif

Чтобы сделать вывод, мы схематично рисуем графики, как для тестирования гипотезы с использованием Z критерия (помним, что распределение Стьюдента с увеличением выборки стремится к стандартному нормальному распределению).

![Alt text](image-25.png)

Такие схематичные рисунки универсальны для критерия Z и t, только пользуемся разными таблицами для нахождения табличного критерия.

## P-value
P-value  – это вероятность увидеть такое же или более экстремальное значение, чем наблюдаемое, при условии, что гипотеза H_0 верна.

P-value на графике – это вероятность в распределение тест-статистика, которая лежит за пределами наблюдаемого значения

Р-value > α,  мы принимаем H_0
Р-value < α,  отвергаем нулевую гипотезу

![Alt text](image-26.png)

Произведем эти действия в Python  и мы видим, что  t≈0.814,  а табличное значение критерия Стьюдента около 1.8 (для 11 степеней свободы и p= 0.95)

![Alt text](image-27.png)

А теперь давайте воспользуемся готовой функцией.

![Alt text](image-28.png)

И мы получили **statistic - расчетное значение критерия** около 0.814. Такое же значение мы получили при расчете по формуле. p-value ≈ 0.433

Давайте изобразим результаты на графике

![Alt text](image-29.png)

Голубым изображена площадь, соответствующая p-value (0.433), а красным – площадь отсечки α (0.05). Эта площадь соответствует табличному значению критерия Стьюдента 1.8.
По графику видим, что верна нулевая гипотеза, p-value > α. Т.о. чтобы интерпретировать результат функции необходимо просто посмотреть на p-value и сравнить его с заранее установленным уровнем статистической значимости α.

**Запомнить! Если p-value < α, то верна альтернативная гипотеза H_1**

## Виды статистических гипотез
Двухвыборочные тесты – это тесты, где данные представляют разные совокупности. Например. Мы хотим сравнить вес людей на диете и вес людей на обычном питании. Сравниваем средние арифметические двух выборок. Или сравниваем среднее давление в выборке до приема лекарства со средним давлением после приема лекарства. До приема лекарства – это были люди, не принимающие лекарство, а после приема эти люди представляют другую генеральную совокупность, ту, где люди принимают это лекарство.
Двухвыборочные тесты в свою очередь бывают с зависимыми и независимыми выборками.

![Alt text](image-30.png)

## Проверка на нормальность (Шапиро - тест и QQ-график)
Критерии нормальности — это группа статистических критериев, предназначенных для проверки нормальности распределения. Критерии нормальности являются частным случаем критериев согласия.
Тестирование данных на нормальность часто является первым этапом их анализа, так как большое количество статистических методов исходит из предположения нормальности распределения изучаемых данных.
Проверить выборку на нормальность с помощью разных тестов на нормальность. Например, **тест Шапиро- Уилка**, где нулевая гипотеза в том, что нет отличий от нормального распределения и альтернативная гипотеза, что  распределение отлично от нормального. 
***Помним, в альтернативную гипотезу мы вкладываем наличие различий!***

Пример: сгенерируем выборку S объемом 50 из нормально распределенной генеральной совокупности со средним арифметическим 0 и стандартным отклонением 1.

![Alt text](image-31.png)

Применим Шапиро-тест
Статистик получился 0.9925, а p-value  ≈ 0.987, что свидетельствует в пользу нулевой гипотезы, что нет отличий от нормального распределения.
А теперь рассмотрим QQ- график

![Alt text](image-33.png)

Красная линия на этом графике символизирует нормальное распределение, а синие точки - это 50 значений выборки S. Чем ближе к красной прямой лежат точки, тем лучше аппроксимация нормальному распределению. Здесь практически все точки лежат на красной прямой, что выборка следует нормальному распределению.
Идея графика заключается в следующем:
по оси X теоретические квантили, а по оси Y упорядоченные значения. Теоретические квантили – это квантили нормального стандартного распределения. Т.е. это Z значения. Помним таблицу Z-значений, например, какая доля лежит ниже 1.96 и получали 97.5% значений. Вот 1.96 – это и есть квантиль.
А теперь нашу выборку S упорядочим по возрастанию. Мы можем узнать, какому перцентилю соответствует каждое значение этой выборки. Вспоминаем описательную статистику на 3й лекции.  Мы искали 1 квартиль, помните? Т.е. мы искали, а ниже какого значения в выборке, лежат 25% значений. А у нас в выборке 50 значений. И мы можем находить, какому перцентилю соответствует каждое из этих значений. Но эти же перцентили мы можем взять и для нормального стандартного распределения и найти для них квартили.

Рисунок ниже: Черным схематично обозначено нормальное стандартное распределение, а фиолетовым схематично обозначено распределение 50 значений выборки S. Отсечем 30% выборки S и получим «практическое» значение (п), а затем отсечем точно такую же долю у нормального распределения и получим «теоретический» квантиль (т). Так вот это значение, которое соответствует 30-му перцентилю в выборке как бы имеет две координаты на QQ-графике (т,п) и соответственно  откладывается по оси х и у (теоретический квантиль и упорядоченное значение в выборке). Но если бы наше распределение точно бы повторяла форму нормального распределения, то мы бы видели только одну черную колоколообразную кривую и квантили теоретические совпадали бы с практическими. Вот именно так и строится красная линия на QQ - графике. Поэтому, чем ближе к красной линии, тем надежнее наше предположение о нормальности распределения.

![Alt text](image-34.png)

