# Internship  
<p>
    <strong>Internship</strong>
</p>
<p>
    Перед тем, как перейти к основным заданиям, предлагаем ознакомиться поближе с Python и GitHub:
</p>
<ol>
    <li>
        <a href="http://www.datacommunitydc.org/blog/2013/07/python-for-data-analysis-the-landscape-of-tutorials">
            http://www.datacommunitydc.org/blog/2013/07/python-for-data-analysis-the-landscape-of-tutorials
        </a>
    </li>
    <li>
        <a href="http://git-scm.com/doc">
            http://www.datacommunitydc.org/blog/2013/07/python-for-data-analysis-the-landscape-of-tutorials
        </a>
    </li>
    <li>
        <a href="https://github.com/GSoft-SharePoint/Dynamite/wiki/Getting-started-with-SourceTree,-Git-and-git-flow">
            http://www.datacommunitydc.org/blog/2013/07/python-for-data-analysis-the-landscape-of-tutorials
        </a>
    </li>
</ol>
<p>
    <strong>Задание 1. Прогнозирование временного ряда</strong>
</p>
<p>
    В файле Trend_task.txt представлена информация о месячном обороте компании Wheely в трех городах с апреля 2013 по январь 2015 гг. Необходимо построить
    модель для предсказания выручки на следующие пять месяцев (февраль-июнь 2015 года).
</p>
<p>
    Как мы видим это задание в наиболее простой форме:
</p>
<ol>
    <li>
        1) Выделить тренд
    </li>
    <li>
        2) Рассчитать коэффициенты сезонности (желательно, чтобы они были одинаковые для всех городов)
    </li>
    <li>
        3) Предсказать оборот в каждом отдельном городе
    </li>
</ol>
<p>
    Как можно легко рассчитать коэффициенты сезонности (два способа):
</p>
<p>
    а) Разделить реальные значения временного ряда на спрогнозированный тренд
</p>
<p>
    б) Построить регрессионную модель, уже включающую коэффициенты сезонности (смотрим страницу 24 в источнике 1, где используются дамми переменные для каждого
    из месяцев)
</p>
<p>
    Однако, если у вас есть заинтересованность, то вы можете реализовать несколько прогнозных моделей (в том числе, более сложных) и посмотреть, что даст
    лучший результат.
</p>
<p>
    Что можно почитать и посмотреть о временных рядах:
</p>
<ol>
    <li>
        1) <a href="http://www.udel.edu/FREC/ilvento/BUAD820/MOD604.pdf">http://www.udel.edu/FREC/ilvento/BUAD820/MOD604.pdf</a> (общее краткое введение)
    </li>
    <li>
        2) <a href="http://www.business.unr.edu/faculty/rtl/Seasonality-Final16.pdf">http://www.business.unr.edu/faculty/rtl/Seasonality-Final16.pdf</a> (еще
        немного про простые способы прогнозирования)
    </li>
    <li>
        3) <a href="http://www.youtube.com/watch?v=RdTxLXmbvjY">http://www.youtube.com/watch?v=RdTxLXmbvjY</a> (Лекция Воронцова из ШАДа – введение в то, как
        уже по-серьезному подходить ко временным рядам)
    </li>
</ol>
<p>
    <strong></strong>
    <br/>
</p>
<p>
    <strong>Задание 2. Подобрать функцию для фиксированного тарифа</strong>
</p>
<p>
    В файле Rates_task.txt представлены данные о цене поездки (price), ее дистанции (distance) и длительности (duration). Исходим из расчета, что:
</p>
<p>
    price = max(60 + 14 * distance + 9 * duration, 120)
</p>
<p>
    Необходимо подобрать функцию, которая будет зависеть только от километров, которая наиболее точно прогнозирвала цену поездки.
</p>
<p>
    Функция может быть любой формы, какой пожелаете.
</p>
<p>
    Что почитать и посмотреть об оптимизации функции:
</p>
<ol>
    <li>
        1)
        <a
            href="https://ru.wikipedia.org/wiki/%D0%9E%D0%BF%D1%82%D0%B8%D0%BC%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F_(%D0%BC%D0%B0%D1%82%D0%B5%D0%BC%D0%B0%D1%82%D0%B8%D0%BA%D0%B0)"
        >
            https://ru.wikipedia.org/wiki/%D0%9E%D0%BF%D1%82%D0%B8%D0%BC%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F_(%D0%BC%D0%B0%D1%82%D0%B5%D0%BC%D0%B0%D1%82%D0%B8%D0%BA%D0%B0)
        </a>
        (там внизу перечислены основные методы оптимизации, вы можете использовать любой, но следует понимать, что в случае невыпуклой функции нестохастические
        методы могут вести себя странно)
    </li>
    <li>
        2) <a href="http://docs.scipy.org/doc/scipy/reference/tutorial/optimize.html">http://docs.scipy.org/doc/scipy/reference/tutorial/optimize.html</a>
        (пример оптимизации функции в питоне)
    </li>
    <li>
3)        <a href="http://scipy-lectures.github.io/advanced/mathematical_optimization/">http://scipy-lectures.github.io/advanced/mathematical_optimization/</a>
        (еще один пример по питону)
    </li>
</ol>
<p>
    Задание 3. Чистка трека (line simplification)
</p>
<p>
    В файле Tracks_task.txt представлена информация по 6 трекам, которые необходимо свести к, максимум, 250 точкам.
</p>
<p>
    Если захотите что-то визуализировать, используйте библиотеку matplotlib
</p>


