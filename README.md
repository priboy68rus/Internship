# Internship  
Перед тем, как перейти к основным заданиям, предлагаем ознакомиться поближе с Python и GitHub:  
- http://www.datacommunitydc.org/blog/2013/07/python-for-data-analysis-the-landscape-of-tutorials  
- http://git-scm.com/doc  
- https://github.com/GSoft-SharePoint/Dynamite/wiki/Getting-started-with-SourceTree,-Git-and-git-flow (sourcetree - это типа юзер френдли альтернатива, чтобы не пользоваться консолью для гита)  
  
					**Задание 1. Прогнозирование временного ряда**    
       В файле Trend_task.txt представлена информация о месячном обороте компании Wheely в трех городах с апреля 2013 по январь 2015 гг. Необходимо построить модель для предсказания выручки на следующие пять месяцев (февраль-июнь 2015 года).  
Как мы видим это задание в наиболее простой форме:  
1. Выделить тренд  
2. Рассчитать коэффициенты сезонности (желательно, чтобы они были одинаковые для всех городов)  
3. Предсказать оборот в каждом отдельном городе  
Как можно легко рассчитать коэффициенты сезонности (два способа):  
а) Разделить реальные значения временного ряда на спрогнозированный тренд  
б) Построить регрессионную модель, уже включающую коэффициенты сезонности (смотрим страницу 24 в источнике 1, где используются дамми переменные для каждого из месяцев)  
Однако, если у вас есть заинтересованность, то вы можете реализовать несколько прогнозных моделей (в том числе, более сложных) и посмотреть, что даст лучший результат.  
Что можно почитать и посмотреть о временных рядах:  
1)	http://www.udel.edu/FREC/ilvento/BUAD820/MOD604.pdf (общее краткое введение)  
2)	http://www.business.unr.edu/faculty/rtl/Seasonality-Final16.pdf (еще немного про простые способы прогнозирования)  
3)	http://www.youtube.com/watch?v=RdTxLXmbvjY (Лекция Воронцова из ШАДа – введение в то, как уже по-серьезному подходить ко временным рядам)  
  
				**Задание 2. Подобрать функцию для фиксированного тарифа**  
	В файле Rates_task.txt представлены данные о цене поездки (price), ее дистанции (distance) и длительности (duration). Исходим из расчета, что:
					price = max(60 + 14 * distance + 9 * duration, 120)
Необходимо подобрать функцию, которая будет зависеть только от километров, которая наиболее точно прогнозирвала цену поездки.
Функция может быть любой формы, какой пожелаете.
Что почитать и посмотреть об оптимизации функции:
1)	https://ru.wikipedia.org/wiki/%D0%9E%D0%BF%D1%82%D0%B8%D0%BC%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F_(%D0%BC%D0%B0%D1%82%D0%B5%D0%BC%D0%B0%D1%82%D0%B8%D0%BA%D0%B0) (там внизу перечислены основные методы оптимизации, вы можете использовать любой, но следует понимать, что в случае невыпуклой функции нестохастические методы могут вести себя странно)
2)	http://docs.scipy.org/doc/scipy/reference/tutorial/optimize.html (пример оптимизации функции в питоне)
3)	http://scipy-lectures.github.io/advanced/mathematical_optimization/ (еще один пример по питону)
Задание 3. Чистка трека (line simplification)
	В файле Tracks_task.txt представлена информация по 6 трекам, которые необходимо свести к, максимум, 250 точкам.
Если захотите что-то визуализировать, используйте библиотеку matplotlib
