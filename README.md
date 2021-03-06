# Выгрузка и обработка данных сайтов образовательных программ НИУ ВШЭ

**Цель проекта**: Автоматизация мониторинга сайтов образовательных программ, осуществляемого сотрудниками Дирекции основных образовательных программ.

## Описание хода выполнения проектного задания
В ходе выполнения проекта была осуществлена выгрузка html страниц всех сайтов образовательных программ НИУ ВШЭ, а также страниц, являющихся обязательными согласно Стандарту оформления и наполнения интернет-страниц образовательных программ (бакалавриат, магистратура, специалитет) на корпоративном сайте Национального исследовательского университета «Высшая школа экономики». Выгрузка произведена как для русскоязычных версий сайтов, так и для англоязычных.  

Далее была выполнена автоматическая проверка наличия всех блоков, указанных в Стандарте для каждой образовательной программы, а также проверка на наличие ключевых слов и фраз.

## Описание результатов проекта
В качестве результатов проекта предоставляются таблицы формата .xlsx с результатами проверки, а также файлы формата .ipynb, в которых находится код, необходимый для реализации.  

В таблицах указано наличие или отсутствие того или иного блока, являющегося обязательным для всех страниц образовательных программ. Если блок присутствует, то указывается ссылка (например, ссылка на Учебные курсы) или же текст блока (например, адрес и телефон). Если блок отсутствует, то в ячейке указывается «Нет».

Также отдельно предоставляется таблица («Количество знаков.xlsx») с подсчетом количества знаков на каждой странице, указанной в блоке (например, Учебные курсы). Данная таблица является **метрикой** наполненности страниц.

## Описание использованных в проекте способов и технологий
Для реализации проекта использовался язык программирования Python, а также библиотеки bs4 (parser), numpy (для работы с массивами), pandas (для работы с таблицами), time (для подсчета времени выполнения) и другие.

## Описание отклонений и трудностей, возникших в ходе выполнения проекта
В качестве трудностей можно назвать большое количество разных вариантов заполнения образовательными программами тех или иных обязательных блоков согласно Стандарту.  

К примеру, Академический Руководитель на сайте некоторых программ указывается как Руководитель. Более того, он указывается в разных частях страницы для разных ОП, также как и телефон учебного офиса. Адреса указываются с индексами и без. Наконец, присутствует большое множество вариантов названий обязательных пунктов разделов «Студентам» и «Абитуриентам».

## Заключение
В результате создан Jupyter Notebook, позволяющий проводить автоматическую проверку сайтов образовательных программ НИУ ВШЭ сейчас и в будущем, а также были получены текущие результаты проверки.
