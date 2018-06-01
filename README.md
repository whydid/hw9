## №1. Удалить все пустые строки

Я работала в Notepad++

Чтобы удалить все пустые строки, использовала регулярное выражение \n\r и заменила все вхождения на \0.
![](https://github.com/whydid/hw9/blob/master/%D1%81%D0%BA%D1%80%D0%B8%D0%BD1..png)

Для оставшихся пустых строк использовала регулярное выражение \s*$, заменила на \0
![](https://github.com/whydid/hw9/blob/master/%D1%81%D0%BA%D1%80%D0%B8%D0%BD2..png)

## №2. Найти всех князей и города, имя и название которых оканчивается на "слав". В выдаче должны быть такие слова как "Ярославля, Ростиславъ, Ростиславу, Переяславлъ" и т.п. Но не должно быть "славу, выславше" и т.п. 

Я использовала регулярное выражение [А-Я]+\w+слав+\w+ для того, чтобы найти имена князей и города, которые оканчиваются на "слав". 

Получилось 564 вхождения
![](https://github.com/whydid/hw9/blob/master/%D1%81%D0%BA%D1%80%D0%B8%D0%BD3.png)

## "3. Найти все упоминания Новгорода. Учтите, что написание может быть разным . В выдаче должны быть такие слова как "Новѣгородѣ, Новъгородъ, Новгородцю, Новагорода, Новугороду". 

Я испоьзовала регулярное выражение (Новѣ?город[а-я]?|Новъ?город[а-я]?|Новгородц[а-я]?| Новугород[а-я]?|Новгород[а-я]?) ,чтобы найти все упоминания Новгорода в летописи.

Получилось 54 вхождения.

![](https://github.com/whydid/hw9/blob/master/%D1%81%D0%BA%D1%80%D0%B8%D0%BD4.png)

## Бонусное задание 

Я использовала регулярное выражение ([.,;:!?](?![.>)) , заменила на (\1).

![](https://github.com/whydid/hw9/blob/master/%D0%B1%D0%BE%D0%BD%D1%83%D1%81%D0%BD%D0%BE%D0%B5.png)
