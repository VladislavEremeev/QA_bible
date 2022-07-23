# Пирамида / уровни тестирования (Test Pyramid / Testing Levels)

«Пирамида тестов» - метафора, которая означает группировку динамических тестов программного обеспечения по разным уровням. Она также дает представление, какое количество тестов должно быть в каждой из этих групп. Основной принцип разделения уровней - тест должен быть на том же уровне, что и тестируемый объект. В тесте более высокого уровня вы не тестируете всю условную логику и пограничные случаи, которые уже покрыты тестами более низкого уровня.

![](https://lh6.googleusercontent.com/yDN1s-lXbEFI5tsd429c2fT5DkHxfDNFpTotktfGZe2tdXVAdo218WSOksJIhBx5VDJffYvMOcadII\_r7ln-kvX4iKFuuQ75io5IEimepSLJq\_qkkZ\_JH5x5UfdSXdF2PqbBPqpV)

Уровни тестирования:

* Unit/component/program/module testing - тестируется минимально-атомарный модуль программы, чаще всего это одна функция или метод. Таких тестов должно быть больше всего;
* Integration testing - несколько модулей программы тестируются вместе;
* System testing - вся программа тестируется полностью;
* Acceptance testing - программа принимается заказчиком на соответствие заявленным требованиям либо тестировщики проходят end-to-end сценарии с точки зрения пользователя;

Доп. материал:

* [Test Pyramid](https://martinfowler.com/bliki/TestPyramid.html)
* [The Practical Test Pyramid](https://martinfowler.com/articles/practical-test-pyramid.html) + перевод на русский [Пирамида тестов на практике](https://habr.com/ru/post/358950/)
* [От песочных часов к пирамиде: как усовершенствовать структуру тестов](https://habr.com/ru/company/badoo/blog/652025/)
* [Just Say No to More End-to-End Tests](https://testing.googleblog.com/2015/04/just-say-no-to-more-end-to-end-tests.html)
* [How Much Testing is Enough?](https://testing.googleblog.com/2021/06/how-much-testing-is-enough.html)
* [Software Testing Anti-patterns](http://blog.codepipes.com/testing/software-testing-antipatterns.html)
* [Пирамида Автоматизации Тестирования: Версия 2021 года](https://telegra.ph/Piramida-Avtomatizacii-testirovaniya-Versiya-2021-goda-03-24)
* [Антипаттерны тестирования ПО](https://habr.com/ru/post/358178/)
* [Unit, API и GUI тесты - чем отличаются](https://telegra.ph/Unit-API-i-GUI-testy--chem-otlichayutsya-02-11)
* [Почему тестировать должны не только QA. Распределяем тест-кейсы между Dev, Analyst и QA](https://dou.ua/lenta/columns/test-cases-dev-qa-analyst/)
* [Пирамида тестирования на практике. Как работает QA в Jiji](https://dou.ua/lenta/columns/testing-in-jiji/)
* [Почему «осмысленное тестирование» - это важно?](https://habr.com/ru/post/650937/)
* [Разные подходы к тестированию: в чем их суть и какой выбирать для своих проектов](https://habr.com/ru/company/sbermarket/blog/665260/)
