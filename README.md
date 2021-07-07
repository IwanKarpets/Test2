2. Допустим, что по url
http://любой_домен/filter?size=M&color=1&color=2&manufacturer=aaa&manufacturer=ddd
находится страница, на которой есть такие поля:
● радио для size (значения - S, M, L)
● несколько чекбоксов для color (значения - 1, 2, 3, 4, 5)
● мультиселект (select multiple) для manufacturer (значения - "aaa", "b&c", "ddd",
"eee")
● чекбокс "распродажа" (значение - 1)
Допустим также, что сервер при генерации html ни одно из полей не заполняет, то есть
радио не выбран, чекбоксы пустые и т.д.
Задача : набросать самую элементарную разметку для указанных инпутов и написать
скрипт, который
● при загрузке страницы разберёт значения фильтров из url и расставит их по
соответствующим полям
● при изменении состояния в любом инпуте, кроме "распродажа", выведет в
консоль аналогичный приведённому в условии url с актуальными значениями
фильтров
