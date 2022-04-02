# Что нужно автоматизировать?

![](https://lh6.googleusercontent.com/yDbU5SIioPOuXUCODDzKU\_bID9PTPggk12UDYTBN9UTdP02fGiaKqbV5YL0KgWbnz-HLpzLQje\_5ROaA1t0GHhrappPZZOQxvABAQaAHMhllGxmPmRFnMlT\_j\_R0OhVDoubluW70)

**Какие модули и места следует подвергать автоматизации?**

* Участки кода, исполнение которых трудно визуализировать и получить осязаемую информацию о протекающих процессах (back-end процессы, занесение в базу данных, занесение логов в файл);
* Функциональность продукта, которая будет использоваться наиболее часто и возникновение ошибок которой связано с достаточно высоким риском. Автоматизированное тестирование узловых моментов функциональности потребует меньше времени для поиска ошибок. И соответственно, сократит время на их устранение;
* Типовые часто выполняемые операции, которые обычно связаны с обработкой данных (CRUD). Например - формы, в которых количество заполняемых граф и полей довольно значительное. Цель - автоматизировать занесение требуемых данных в нужное поле и проверить правильность выполнения задачи после сохранения результата;
* Сообщения об ошибках. Требуется автоматизация разнесения некорректных данных по соответствующим полям и тестирование корректности проверки правильности данных и сообщений об ошибках;
* Комплексная проверка поведения всей системы, как целостного объекта (end-to-end testing);
* Проверка числовых массивов, нужных для достоверных математических операций;
* Тестирование корректности отображаемых результатов поиска в ответ на запрос по нужным данным;
* Предложенный список только ориентировочный. Всё зависит от предъявляемых к проверяемой системе требований, возможностей, которые позволяет реализовать выбранный для автоматического тестирования инструмент.

Источники:

* [Какие места в проекте нужно автоматизировать в первую очередь?](https://software-testing.org/automation-testing/kakie-mesta-v-proekte-nuzhno-avtomatizirovat-v-pervuyu-ochered.html)

Доп. материал:

* [Автоматизировать или нет: спорные кейсы, плюсы и минусы автотестов](https://habr.com/ru/post/653721/)
* [How To Select Correct Test Cases For Automation Testing (And Ultimately Achieve A Positive Automation ROI)](https://www.softwaretestinghelp.com/manual-to-automation-testing-process-challenges/)
* [How To Implement Efficient Test Automation In The Agile World](https://www.softwaretestinghelp.com/automation-in-agile-world/)
* [Right Tests for Automation](https://www.softwaretestinghelp.com/automation-testing-tutorial-1/#:\~:text=to%20strategize%20automation.-,Right%20Tests%20for%20Automation,-The%20best%20way)
* [Решаем, что и когда автоматизировать, и нужно ли](https://testengineer.ru/reshaem-chto-i-kogda-avtomatizirovat/)
* [Не автоматизируйте test cases](https://habr.com/ru/post/652499/)
* [Автоматизация тестирования: что можно, а что не нужно](https://cleverics.ru/digital/2021/01/sw-testing-automation/)
* [Лучшие практики автоматизации тестирования: решение, что и когда автоматизировать](https://telegra.ph/Luchshie-praktiki-avtomatizacii-testirovaniya-reshenie-chto-i-kogda-avtomatizirovat-05-06)
