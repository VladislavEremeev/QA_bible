# Список ресурсов по инструментам тестировщика

**DevTools**:

В каждый современный браузер встроены инструменты разработчика. Chrome DevTools — это набор инструментов веб-разработчика, встроенных непосредственно в браузер Google Chrome. DevTools позволяет оперативно редактировать страницы и быстро диагностировать проблемы, что помогает быстрее создавать более качественные веб-сайты:
  * [Начало работы с Chrome DevTools](https://developer.chrome.com/docs/devtools/overview?hl=ru)
  * [Имитация мобильных устройств в режиме устройства](https://developer.chrome.com/docs/devtools/device-mode?hl=ru)
  * [Начало работы с просмотром и изменением DOM](https://developer.chrome.com/docs/devtools/dom?hl=ru)
  * [Просмотр сетевой активности](https://developer.chrome.com/docs/devtools/network?hl=ru)
  * [Анализ производительности](https://developer.chrome.com/docs/devtools/performance?hl=ru)
  * [Безопасность: понимание проблем безопасности](https://developer.chrome.com/docs/devtools/security?hl=ru)
  * [Удаленная отладка Android-устройств](https://developer.chrome.com/docs/devtools/remote-debugging?hl=ru)
* [Средства консоли Chrome, которыми вы, возможно, никогда не пользовались](https://habr.com/ru/company/ruvds/blog/486692/)
* [Изучаем DevTools в Google Chrome](https://youtu.be/GyKY5kIRP00?si=gY1Me2opxwkwvg98)
* [Chrome DevTools: что это - обзор на инструменты](https://blog.skillfactory.ru/glossary/chrome-devtools/)
* [QA с Нуля - DevTools, Web Console, Device Toolbar](https://www.youtube.com/watch?v=mP23B6o9uhQ)
* [Курс Тестировщика с нуля. 25 урок. Как тестировщику работать в DevTools](https://www.youtube.com/watch?v=IO14lZynBvM)
* [Основные Use case использования Dev Tools для QA](https://www.youtube.com/watch?v=pxM3f8vyIhA\&t=320s)
* [Изучаем инструменты разработчика Google Chrome (ЧАСТЬ 1)](https://www.youtube.com/watch?v=FStLGMPHSEI\&list=PLvWwA9iDlhHA4kzfpRbu2cH-Z2ss6tB99)
* [DevTools для «чайников»](https://habr.com/ru/post/548898/)
* [Devtools для тестировщика - Devtools chrome - Что такое Devtools](https://www.youtube.com/watch?v=LYEEMWSrOgI)
* [Полезные функции DevTools для тестировщиков](https://habr.com/ru/post/558694/)
* [Chrome DevTools. Обзор основных возможностей веб-инспектора](https://www.youtube.com/watch?v=C8Z-N0y6Sqo)
* [Chrome Developer Tools для тестировщика](https://testengineer.ru/chrome-developer-tools-dlya-testirovshchika/)
* [Lighthouse](https://developers.google.com/web/tools/lighthouse?hl=ru)
* [Советы по инструментам разработчика](https://developer.chrome.com/docs/devtools/tips?hl=ru)

  Официальная документация DevTools:
    * [Chrome DevTools](https://developer.chrome.com/docs/devtools)
    * [Firefox DevTools](https://firefox-source-docs.mozilla.org/devtools-user/)
    * [Safari DevTools](https://support.apple.com/ru-ru/guide/safari/sfri20948/mac)

**Тестирование API**:

API (Application Programming Interface) — это набор правил и механизмов, которые позволяют различным программным приложениям взаимодействовать друг с другом. Тестирование API — это процесс проверки правильности работы этих интерфейсов, их производительности, безопасности и функциональности. В отличие от тестирования пользовательского интерфейса (UI), тестирование API сосредоточено на уровне бизнес-логики и данных.

Основной популярный инструмент для тестирования API - [Postman](https://www.postman.com/).
Postman представляет собой мультитул для тестирования API. В нем можно создавать коллекции запросов, проектировать дизайн API и создавать для него моки (заглушки-имитации ответов реального сервера), настраивать мониторинг (периодическая отправка запросов с журналированием), для запросов возможно написание тестов на JS, есть собственный Runner и т.д. Постман хорошо подойдет в простых случаях автоматизации или как инструмент поддержки а анализа: проверка работоспособности endpoint, дебаг тестов, простая передача информации о дефектах (можно сохранить запрос в curl, ответ в json и т.п.). Postman также может работать без графического интерфейса (newman).

* [Postman для тестировщика. Мини-курс](https://www.youtube.com/playlist?list=PLKbJd47KcbjvLgn-ukTvfpaGoXAqybza0)
* [Курс Тестирование ПО. Занятие 30. POSTMAN. Ручное тестирование API - QA START UP](https://www.youtube.com/watch?v=55l6XIEK9l0\&ab\_channel=QASTARTUP-ITTrainingCenter)
* [Сергей Махетов - Воркшоп: Исследуем возможности Postman (часть 1)](https://www.youtube.com/watch?v=OFGVn-isQyk\&ab\_channel=Heisenbug)
* [Сергей Махетов - Воркшоп: Исследуем возможности Postman (часть 2)](https://www.youtube.com/watch?v=IQ9sjNm11Nc\&ab\_channel=Heisenbug)
* [API testing using Postman](https://robertgorter.medium.com/api-testing-using-postman-87cf1c40b82c)
* [Postman Beginner's Course - API Testing](https://youtu.be/zp5Jh2FIpF0?si=GG352hDvk_A6en4V)
* [Погружение qa junior в пучину API с использованием SoapUI(Open Source)](https://habr.com/ru/company/renins/blog/558436/)
* [Шпаргалка по Postman](https://telegra.ph/SHpargalka-po-Postman-09-01-2)
* [Большой гайд по тестированию с Postman для начинающих](https://testengineer.ru/gajd-po-testirovaniyu-v-postman/)
* [Основы Postman для самых маленьких](https://habr.com/ru/company/maxilect/blog/596789/)
* [Reqover](https://github.com/reqover/docs) is language agnostic tool that gives a picture about coverage of APIs based on Open API (Swagger) or GraphQL
* [Swagger-coverage](https://github.com/viclovsky/swagger-coverage) gives a full picture about coverage of API tests (regression) based on OAS (Swagger)
* [36 частых вопросов по Postman](https://testengineer.ru/postman-sobesedovanie/)
* [Тестирование производительности в Postman](https://testengineer.ru/testirovanie-proizvoditelnosti-v-postman/)
* [curl - учимся тестировать API](https://testengineer.ru/curl-uchimsya-testirovat-api/)
* [Как мы тестируем Rest API в SM 2.0 с помощью Postman: сценарии, запросы, переменные окружения и немного автотестов](https://habr.com/ru/company/sportmaster\_lab/blog/646365/)
* [Swagger: что это такое, и как с ним работать?](https://highload.today/swagger-api/)
* [Основы Cypress: тестирование API](https://www.software-testing.ru/library/testing/testing-tools/3809-cypress-basics-api-testing)
* [SOAP API](https://telegra.ph/SOAP-API-05-08)
* [SOAP UI](https://telegra.ph/SOAP-UI-05-09)
* [Что нужно знать про Postman: максимально коротко о Mock Servers, Flow и Visualize](https://habr.com/ru/company/rostelecom/blog/666766/)
* [Как выбрать инструмент для тестирования API](https://habr.com/ru/company/simbirsoft/blog/675878/)
* **Открытые и тренировочные API**:
  * [Большая подборка открытых API](https://habr.com/p/769384/)
  * [Список открытых API](https://github.com/public-apis/public-apis)
  * [Обзор сайтов с API документацией](https://github.com/docops-hq/learnapidoc-ru/blob/master/Publishing-doc/API-doc-sites-list.md#100-)
  * [Бесплатные API - Ресурсы для практического тестирования веб-сервисов](https://www.youtube.com/watch?v=dvLZDdC9eR0)
  * [100+ сайтов с API документацией](https://starkovden.github.io/API-doc-sites-list.html#100-%D1%81%D0%B0%D0%B9%D1%82%D0%BE%D0%B2-%D1%81-api-%D0%B4%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B0%D1%86%D0%B8%D0%B5%D0%B9)
  * [Mockend](https://mockend.com) is the #1 GitHub app dedicated to API mocking
  * [MockAPI](https://mockapi.io/docs) is a simple tool that lets you easily mock up APIs, generate custom data, and preform operations on it using RESTful interface
  * [Swagger Petstore](https://petstore.swagger.io)
  * [ReqRes](https://reqres.in)
  * [httpbin](http://httpbin.org)
  * [users.bugred.ru](http://users.bugred.ru)
  * [The Star Wars API](https://swapi.dev)
  * [API with auth](https://restful-booker.herokuapp.com/apidoc/index.html#api-Auth-CreateToken)
  * [another API with auth](https://www.weatherapi.com/docs/)
  * [API hh.ru](https://habr.com/ru/company/hh/blog/303168/)
  * [Фокус API](https://developer.kontur.ru/doc/focus?about=2)
  * [API DaData](https://dadata.ru/api/)
  * [API JSON Placeholder](https://jsonplaceholder.typicode.com)
  * [openexchangerates.org](https://openexchangerates.org)
  * [openweather](https://openweathermap.org/api)
  * [Last.fm Music Discovery API](https://www.last.fm/api)

**Proxy (снифферы трафика)**:

Proxy-серверы и снифферы трафика — это инструменты, которые позволяют перехватывать и анализировать сетевой трафик. Они используются для мониторинга данных, проходящих через сеть, и могут помочь тестировщикам в выявлении и исправлении ошибок, анализе производительности и проверке безопасности веб-приложений.

Популярные инструменты Proxy (снифферы трафика):

[Fiddler](https://www.telerik.com/fiddler) - мощный инструмент для перехвата и отладки HTTP/HTTPS трафика. Он позволяет просматривать и изменять входящие и исходящие запросы.

[Charles Proxy](https://www.charlesproxy.com/) - популярный прокси-сервер, используемый для мониторинга и анализа HTTP/HTTPS трафика, а также для тестирования веб-приложений и мобильных приложений.

[Burp Suite](https://portswigger.net/burp/communitydownload) - комплексное средство для тестирования безопасности веб-приложений, включающее прокси-сервер для перехвата и изменения трафика, а также множество других инструментов для анализа безопасности.

[Wireshark](https://www.wireshark.org/) - один из самых известных снифферов, используемый для детального анализа сетевых пакетов на разных уровнях сетевой модели.

* [Web Security Academy - Burp Suite](https://portswigger.net/web-security)
* [Charles: незаменимый тул в арсенале QA-инженера](https://habr.com/ru/company/redmadrobot/blog/269109/)
* [Breakpoints charles proxy Подмена данных](https://www.youtube.com/watch?v=74v5lpOug8c\&feature=youtu.be\&ab\_channel=BogdanOvsiyuk)
* [Как приручить Charles Proxy?](https://habr.com/ru/company/youla/blog/527648/)
* [Using Web Debugging Proxies for Application Testing](https://www.apriorit.com/dev-blog/591-proxies-for-application-testing)
* [Перехват SSL трафика с Android-приложения](https://telegra.ph/Perehvat-SSL-trafika-s-Android-prilozheniya-01-26)
* [Hail Frida!! The Universal SSL pinning bypass for Android applications](https://infosecwriteups.com/hail-frida-the-universal-ssl-pinning-bypass-for-android-e9e1d733d29)
* [Начинающему QA: полезные функции снифферов на примере Charles Proxy](https://habr.com/ru/company/maxilect/blog/554888/)
* [Перехват SSL трафика с Android-приложения](https://telegra.ph/Perehvat-SSL-trafika-s-Android-prilozheniya-01-26)
* [Откручивание SSL пиннинга в Android приложениях](https://habr.com/ru/post/559722/)
* [HTTP Toolkit](https://httptoolkit.tech) is a beautiful & open-source tool for debugging, testing and building with HTTP(S) on Windows, Linux & Mac
* [mitmproxy is a free and open source interactive HTTPS proxy](https://mitmproxy.org)
* [Charles Proxy meetup](https://www.youtube.com/watch?v=gWhvVaoHh70)
* [Open Source Fiddler Alternatives for Mac](https://alternativeto.net/software/fiddler/?license=opensource\&platform=mac)
* [Битва снифферов: Charles vs Proxyman](https://habr.com/ru/company/ozontech/blog/579392/)
* [Почему Proxyman - сын маминой подруги в мире снифферов](https://habr.com/ru/company/indriver/blog/591525/)
* [Плейлист Charles Proxy](https://www.youtube.com/playlist?list=PLof3mAh50UD05mFlTvNpTszOUY9eFrSDX)
* [Погружение в Charles Proxy](https://habr.com/ru/post/663926/)
* [Wireshark — подробное руководство по началу использования](https://habr.com/ru/articles/735866/)
* [Руководство и шпаргалка по Wireshark](https://habr.com/ru/articles/436226/)
* [Первые шаги с Fiddler Classic](https://habr.com/ru/articles/533138/)
* [Fiddler = удобный сниффер + прокси сервер](https://habr.com/ru/articles/554562/)

**Тестирование безопасности**:

Тестирование безопасности — это процесс выявления уязвимостей в системе или приложении с целью предотвращения возможных атак, утечек данных и других угроз. Оно позволяет обеспечить защиту конфиденциальной информации и поддерживать целостность и доступность системы.

Популярные инструменты для тестирования безопасности:

[Burp Suite](https://portswigger.net/burp/communitydownload) — комплексный инструмент для тестирования безопасности веб-приложений, включающий анализаторы, сканеры уязвимостей и средства для автоматизации тестирования.

[OWASP ZAP](https://www.zaproxy.org/) (Zed Attack Proxy) — бесплатный и открытый инструмент для нахождения уязвимостей в веб-приложениях, поддерживающий автоматическое и ручное тестирование.

[Metasploit](https://www.metasploit.com/) — платформа для разработки, тестирования и эксплуатации уязвимостей, широко используемая в пентестинге.

[Wireshark](https://www.wireshark.org/) — сетевой анализатор, который позволяет перехватывать и детально исследовать сетевой трафик, выявляя подозрительные активности и потенциальные угрозы.

* [Рамазан Рамазанов — Тестирование безопасности API: кейсы, инструменты и рекомендации](https://youtu.be/XNwpzNNiWzE?si=3T2RdEe4iGQIE4Pe)
* [Тестирование безопасности. Тестирование на проникновение](https://youtu.be/C0euAbFaT4s?si=4Dme6FvnbOizABt-)
* [Тестирование безопасности. OWASP TOP 10 уязвимостей](https://youtu.be/fgtuLbT4joI?si=hnNfgOJXZRn7AhtR)
* [Иван Румак — Эффективный поиск XSS-уязвимостей](https://youtu.be/EmJnUqFgaK8?si=OThcdoAeoKAcY2_j)
* [Александра Сватикова — Статическое тестирование безопасности инструментами из open source](https://youtu.be/E87YkXhdxAA?si=YuPImtFyBoqzd_HO)
* [Анна Васильева — Поиск уязвимостей IDOR (BOLA)](https://youtu.be/FQROPd_p1ME?si=XHVJpf1BJr7A_0Pr)

* [Сканирование на уязвимости: обзор продуктов, которые есть на рынке](https://habr.com/ru/company/cloud4y/blog/651831/)
* [Чем искать уязвимости веб-приложений: сравниваем восемь популярных сканеров](https://habr.com/ru/company/tomhunter/blog/456892/)
* [10 лучших инструментов сканирования уязвимостей для тестирования на проникновение - 2020](https://itsecforu.ru/2019/08/06/%F0%9F%92%A3-10-%D0%BB%D1%83%D1%87%D1%88%D0%B8%D1%85-%D0%B8%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D0%B2-%D1%81%D0%BA%D0%B0%D0%BD%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F/)
* [20 мощных инструментов тестирования на проникновение в 2019 году](https://itfb.com.ua/instrumenty-testirovaniya-bezopasnosti/)
* [Пентест веб сайта с помощью Owasp Zap](https://habr.com/ru/company/alexhost/blog/530110/)
* [Проверяем безопасность приложений с помощью Drozer](https://habr.com/ru/company/alexhost/blog/535396/)
* [Kali Linux](https://www.kali.org)
* [https://github.com/FSecureLABS/drozer](https://github.com/FSecureLABS/drozer)
* [Тестирование защищенности приложений при помощи SAST (Static Application Security Testing)](https://www.youtube.com/watch?v=Jk8LiaMF2aw)
* [Обзор сканера Nikto для поиска уязвимостей в веб-серверах](https://habr.com/ru/companies/first/articles/731696/)
* [«Осторожно, печеньки!»: советы начинающим тестировщикам в сфере безопасности](https://habr.com/ru/companies/redmadrobot/articles/544198/)

**GIT**:

Git - это [система контроля версий](https://git-scm.com/book/ru/v2/%D0%92%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D0%B5-%D0%9E-%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B5-%D0%BA%D0%BE%D0%BD%D1%82%D1%80%D0%BE%D0%BB%D1%8F-%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D0%B9), которая упрощает работу нескольких человек над одним проектом, помогая разрешать конфликты слияния изменений, следить за историей, откатывать эти изменения и т.п.

Ваш репозиторий может быть локальным и/или находиться в: [GitHub](https://github.com), [Bitbucket](https://bitbucket.org), [GitLab](https://gitlab.com)

Даже ручному тестировщику пригодятся навыки работы с Git: хранить там портфолио для резюме с подтверждением навыков использования инструментов и написания документации, можно само резюме разместить на github pages, уже на работе иногда будет требоваться самостоятельно сбилдить себе сборку на тест или разобраться, в какой момент (в каком коммите) появился баг или наоборот был пофикшен и т.п. Про автоматизацию, очевидно, даже и говорить не стоит - гит там используется ежедневно.

* Learn Git – Full Course for Beginners: [Видео](https://youtu.be/zTjRZNkhiEU?si=v4GP4NVP64TllnaF)
* Система контроля версий - GIT: [Плейлист](https://youtube.com/playlist?list=PLRs8EELOYKc44Y_fKFvADdPXbrYZDQqr0&si=Ff0EFlvxWMSKCUgS)
* GIT - Полный Курс Git и GitHub Для Начинающих [4 ЧАСА]: [Видео](https://youtu.be/O00FTZDxD0o?si=KgFX-GX6Rm920FIs)
* Git for Professionals Tutorial: [Видео](https://youtu.be/Uszj_k0DGsg?si=U6MGdVfC7HQeKuen)
* [Git and GitHub Tutorial – Version Control for Beginners](https://www.freecodecamp.org/news/git-and-github-for-beginners/)
* [Very beautiful GIT documentation](https://www.linkedin.com/posts/fabbasi\_github-activity-6835855126062800896-hAiJ/)
* [GIT PURR! Git Commands Explained with Cats!](https://girliemac.com/blog/2017/12/26/git-purr/)
* [Git для тестировщиков](https://www.youtube.com/playlist?list=PLKbJd47KcbjuHU3AhyeOPJ9p\_GDB6yGL7)
* [Git для новичков (часть 1)](https://habr.com/ru/post/541258/)
* [Git изнутри и на практике](https://habr.com/ru/company/oleg-bunin/blog/468177/)
* [Git, я хочу все отменить! Команды исправления допущенных ошибок](https://habr.com/ru/company/skillbox/blog/534972/)
* [Getting solid at Git rebase vs. merge](https://medium.com/@porteneuve/getting-solid-at-git-rebase-vs-merge-4fa1a48c53aa)
* [Git How To - это интерактивный тур, который познакомит вас с основами Git](https://githowto.com/ru)
* [Плейлист “Основы использования GIT”](https://www.youtube.com/playlist?list=PLvItDmb0sZw8WmkxzGJUZl6S3KU\_-7-aP)
* [GIT-практикум](https://www.youtube.com/watch?v=nRXacgNHNVw\&list=PLvItDmb0sZw-KsqUenM2jyBpNslNzDJLO\&index=1)
* [Octotree](https://www.octotree.io) - GitHub on steroids
* [Плейлист “GIT для тестировщиков с нуля за 1 час”](https://www.youtube.com/playlist?list=PL9mn2EBC\_SSynAcYKFAtMTIhsKD0OGqWX)
* [Как установить Git и выкачать репозиторий](https://www.youtube.com/watch?v=lZdGWJtrsNw)
* [GitFlic](https://gitflic.ru) - первый российский сервис для хранения кода и работы с ним
* [Шпаргалка по консольным командам Git](https://github.com/cyberspacedk/Git-commands)
* [Шпаргалка по Git, в которой представлены основные команды](https://proglib.io/p/git-cheatsheet)
* [Работа с Git в Visual Studio Code](https://htmlacademy.ru/blog/git/git-in-vscode)
* [15 ресурсов по Git. Что почитать/посмотреть?](https://habr.com/ru/companies/yandex_praktikum/articles/768492/)
* _Практическое задание: форкнуть себе репозиторий QA bible :)_

**SQL**:

Это язык программирования, применяемый для создания, модификации и управления данными в базе данных.

Самые популярные базы данных:
1. SQLite

    * Описание: Легковесная, встроенная реляционная база данных, часто используемая в мобильных и настольных приложениях.
    * Официальный сайт: [SQLite](https://www.sqlite.org)

2. MySQL

    * Описание: Одна из самых популярных реляционных баз данных, широко используемая для веб-приложений и корпоративного ПО.
    * Официальный сайт: [MySQL](https://www.mysql.com/)

3. PostgreSQL

    * Описание: Мощная, открытая реляционная база данных с поддержкой расширенных функций, таких как масштабируемость и расширяемость.
    * Официальный сайт: [PostgreSQL](https://www.postgresql.org/)

4. MongoDB

    * Описание: Документо-ориентированная база данных NoSQL, популярная благодаря своей гибкости и масштабируемости, особенно для облачных приложений.
    * Официальный сайт: [MongoDB](https://www.mongodb.com/)

5. Oracle Database

    * Описание: Мощная реляционная база данных, широко используемая в крупных корпоративных системах благодаря высокой производительности и надежности.
    * Официальный сайт: [Oracle](https://www.oracle.com/database)

6. Microsoft SQL Server

    * Описание: Реляционная база данных от Microsoft, известная своей интеграцией с продуктами Microsoft и высокой производительностью.
    * Официальный сайт: [Microsoft SQL Server](https://www.microsoft.com/sql-server)

7. Redis

    * Описание: Высокопроизводительная база данных ключ-значение, часто используемая для кэширования и временного хранения данных.
    * Официальный сайт: [Redis](https://redis.io/)

* GUI клиенты
  * [DataGrip от JetBrains](https://www.jetbrains.com/ru-ru/datagrip/)
  * [dBeaver](https://dbeaver.com)
  * [MySQL Workbench](https://www.mysql.com/products/workbench/)
  * [HeidiSQL](https://www.heidisql.com)
  * [Navicat for MySQL](https://www.navicat.com/en/products/navicat-for-mysql)
  * [dbForge Studio for MySQL](https://www.devart.com/dbforge/mysql/studio/)
* Основы SQL
  * [Алан Бьюли "Изучаем SQL"](https://www.amazon.com/Learning-SQL-Generate-Manipulate-Retrieve/dp/1492057614/ref=sr\_1\_1?dchild=1\&keywords=sQL\&qid=1613292997\&s=books\&sr=1-1)
  * [Линн Бейли "Изучаем SQL"](https://www.amazon.com/Head-First-SQL-Brain-Learners/dp/0596526849/ref=sr\_1\_10?dchild=1\&keywords=sQL\&qid=1613292997\&s=books\&sr=1-10)
  * [W3C Introduction to SQL](https://www.w3schools.com/sql/sql\_intro.asp)
  * [Официальная дока](https://dev.mysql.com/doc/)
  * [guru99 - SQL Tutorial for Beginners: Learn SQL in 7 Days](https://www.guru99.com/sql.html)
  * [SQL запросы быстро. Часть 1](https://habr.com/ru/post/480838/)
  * [Понимание джойнов сломано. Это точно не пересечение кругов, честно](https://habr.com/ru/post/448072/)
  * [Плейлист](https://www.youtube.com/playlist?list=PLvItDmb0sZw9-yTHNWpfXDyPPg8aXYb-B) по основам
  * [Видеокурс “How to… SQL Essential”](https://www.youtube.com/playlist?list=PLvItDmb0sZw8BsPPGyZwGBDFjUgoxadKJ)
* Продвинутый уровень
  * [SQL For Web Developers - Complete Database Course](https://youtu.be/KBDSJU3cGkc?si=iK8mVf9sBmgYyvnU)
  * [SQL Tutorial - Full Database Course for Beginners](https://youtu.be/HXV3zeQKqGY?si=SXl0PNhiKRS9l9ZD)
  * [Энтони Молинаро "SQL. Сборник рецептов"](https://www.amazon.com/SQL-Cookbook-Query-Solutions-Techniques/dp/1492077445/ref=sr\_1\_2?dchild=1\&keywords=sQL\&qid=1613292997\&s=books\&sr=1-2)
  * [Алекс Кригель "SQL. Библия пользователя"](https://www.amazon.com/SQL-Bible-Alex-Kriegel/dp/0470229063/ref=sr\_1\_1?dchild=1\&keywords=sQL+bible\&qid=1613293063\&s=books\&sr=1-1)
  * [Джеймс Грофф, Пол Вайнберг, Эндрю Оппель "SQL Полное руководство. Третье издание."](https://www.amazon.com/SQL-Complete-Reference-James-Groff-dp-0071592555/dp/0071592555/ref=mt\_other?\_encoding=UTF8)
* Практика
  * [Бесплатные курсы для изучения SQL в 2024 году](https://habr.com/p/791260/)
  * [SQLAcademy - Онлайн тренажер с упражнениями по SQL](https://sql-academy.org/ru)
  * [SQLBolt - Introduction to SQL](https://sqlbolt.com)
  * [W3C - The Try-SQL Editor](https://www.w3schools.com/sql/trysql.asp?filename=trysql\_op\_in)
  * [HackerRack SQL](https://www.hackerrank.com/domains/sql)
  * [Упражнения по SQL](https://www.sql-ex.ru/?Lang=0)
  * [Тест на знание SQL](https://www.learnqa.ru/sql\_test)
  * [https://www.db-fiddle.com/](https://www.db-fiddle.com)
  * [Видео курс “SQL Практикум”](https://www.youtube.com/playlist?list=PLvItDmb0sZw-WX3dpyJJcuIyy6i2dT7FA)
  * [6 бесплатных ресурсов для практики в SQL](https://robotdreams.cc/blog/178-6-besplatnyh-resursov-dlya-praktiki-v-sql)
* Shit happens
  * [SQL Cheat Sheet](http://www.sqltutorial.org/wp-content/uploads/2016/04/SQL-cheat-sheet.pdf)
  * [Основные команды SQL, которые должен знать каждый программист](https://tproger.ru/translations/sql-recap/)
  * [27 распространенных вопросов по SQL с собеседований и ответы на них](https://tproger.ru/articles/sql-interview-questions/)
* [Ресурсы и инструменты для обучения и практической работы с базами данных - SQL](https://www.youtube.com/watch?v=fiiNGLSIs80)
* [The 10 best sql analytics services for qa teams in 2021](https://theqalead.com/tools/best-sql-analytics/)
* [Что такое базы данных NoSQL?](https://aws.amazon.com/ru/nosql/)
* [Курс Тестирование ПО. Занятие 34. NoSQL база данных. Сравнение SQL и NoSQL](https://www.youtube.com/watch?v=Skl0tWrnqz8)
* [100+ Most Popular SQL Interview Questions And Answers](https://www.softwaretestingmaterial.com/sql-interview-questions/)
* [Курс Тестирования ПО. Занятие 19. Зачем тестировщику нужен SQL. Практические примеры](https://www.youtube.com/watch?v=EdXq2AoRYI8)
* [Лучшие вопросы средней сложности по SQL на собеседовании аналитика данных](https://habr.com/ru/company/dcmiran/blog/500360/)
* [Плейлист "Базы данных"](https://www.youtube.com/playlist?list=PLbuh2pN46AEvM2ZI-rJL2MVguz8Ea9mrJ)
* [Памятка/шпаргалка по SQL](https://habr.com/ru/post/564390/)
* [Тестирование баз данных](https://habr.com/p/804851/)
* [База по базам. SQL для тестировщика](https://testengineer.ru/sql-for-testers/)

**Инструменты тестирования мобильных приложений**:

Инструменты тестирования мобильных приложений помогают тестировщикам выявлять и исправлять ошибки в мобильных приложениях, обеспечивая их высокое качество и стабильность. Эти инструменты позволяют автоматизировать процесс тестирования, проводить функциональные, производительные и пользовательские тесты на различных устройствах и платформах.

Популярные инструменты:

1. [Appium](http://appium.io/): Открытая платформа для автоматизации тестирования мобильных приложений на iOS и Android, поддерживающая различные языки программирования.

2. [Espresso](https://developer.android.com/training/testing/espresso): Инструмент от Google для автоматизированного тестирования Android-приложений, интегрированный с Android Studio.

3. [XCUITest](https://developer.apple.com/documentation/xctest): Фреймворк для тестирования iOS-приложений, интегрированный в Xcode, предоставляемый Apple.

4. [Calabash](https://github.com/calabash/calabash-android): Открытый фреймворк для написания и выполнения автоматизированных тестов для мобильных приложений на iOS и Android, использующий язык Cucumber.

5. [TestComplete](https://smartbear.com/product/testcomplete/): Коммерческий инструмент для автоматизированного тестирования мобильных приложений, поддерживающий iOS и Android, а также предоставляющий возможности для записи и воспроизведения тестов.

* [Android Debug Bridge (adb)](https://developer.android.google.cn/studio/command-line/adb?hl=en), [Minimal ADB](https://rootmydevice.com/download-minimal-adb-and-fastboot/), [Инструменты тестирования Android приложений. Часть 2](https://szadorozhnyi.medium.com/%D0%B8%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F-android-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B9-%D1%87%D0%B0%D1%81%D1%82%D1%8C-2-4107dc748d0f), [Отладка по ADB](https://trofimovdigital.ru/blog/adb)
* [Logcat](https://developer.android.com/studio/debug/am-logcat), [Инструменты тестирования Android приложений. Часть 3](https://szadorozhnyi.medium.com/%D0%B8%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F-android-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B9-%D1%87%D0%B0%D1%81%D1%82%D1%8C-3-e347a621a3bd)
* [Logcat прямо на устройстве](https://play.google.com/store/apps/details?id=com.tananaev.logcat\&hl=ru\&gl=US)
* [ANR-WatchDog](https://github.com/SalomonBrys/ANR-WatchDog), [Инструменты тестирования Android приложений. Часть 5](https://szadorozhnyi.medium.com/%D0%B8%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F-android-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B9-%D1%87%D0%B0%D1%81%D1%82%D1%8C-5-caddda14f175)
* [Performance tracing](https://developer.android.com/topic/performance/tracing)
* [Xcode profiler](https://www.avanderlee.com/debugging/xcode-instruments-time-profiler/)
* [On-device developer options](https://developer.android.com/studio/debug/dev-options)
* [apkanalyzer](https://developer.android.com/studio/command-line/apkanalyzer)
* [Top 10 Mobile Performance Testing Tools in 2020](https://dzone.com/articles/top-10-mobile-performance-testing-tools-in-2020)
* [UI/Application Monkey Tester](https://developer.android.com/studio/test/monkey), [Monkey Testing - Как тестировать мобильные приложения](https://www.youtube.com/watch?v=sXtXy5kWVw8)
* [Mobile App Beta Testing Services (IOS And Android Beta Testing Tools)](https://www.softwaretestinghelp.com/mobile-app-beta-testing-services/)
* Инструменты скорее разработчика, чем тестировщика, но наверняка когда-то придется столкнуться:
  * Google Firebase: некоторые из самых популярных функций платформы включают в себя базы данных, аутентификацию, push-уведомления, аналитику (в т.ч. по крешам), хостинг и многое другое: [документация](https://firebase.google.com/docs/crashlytics), [youtube](https://www.youtube.com/c/firebase/videos?app=desktop), [обзор](https://blog.back4app.com/ru/%D1%87%D1%82%D0%BE-%D1%82%D0%B0%D0%BA%D0%BE%D0%B5-firebase/), [мастеркласс](https://www.youtube.com/watch?v=1\_2R6yIg3SY)
  * OneSignal: Лидер на рынке взаимодействия с клиентами, мобильных и веб пушей, электронной почты, SMS и in-app сообщений.

**Эмуляторы, симуляторы, фермы устройств**:

Эмуляторы, симуляторы и фермы устройств — это инструменты, которые позволяют тестировщикам проверять работу приложений на различных устройствах и операционных системах без необходимости иметь физический доступ ко всем этим устройствам. Эти инструменты значительно упрощают процесс тестирования, обеспечивая доступ к широкому спектру конфигураций и сценариев использования.

_Эмуляторы_: программные приложения, которые воспроизводят поведение реальных устройств, позволяя тестировать программное обеспечение на различных платформах.

_Симуляторы_: похожи на эмуляторы, но не воспроизводят аппаратную часть устройства, а имитируют его программное окружение.

_Фермы устройств_: облачные или локальные сервисы, предоставляющие доступ к множеству реальных устройств для удаленного тестирования.

* [Android studio emulator](https://developer.android.google.cn/studio/run/emulator)
* [Genymotion - Android Virtual Devices for all your development & testing needs](https://www.genymotion.com)
* [BrowserStack - Test instantly on a wide range of real iOS and Android devices on the cloud](https://www.browserstack.com/app-live)
* [10 лучших альтернатив BrowserStack (бесплатные и платные) 2021](https://rigorousthemes.com/blog/best-browserstack-alternatives-free-paid/)
* [Xcode simulator](https://developer.apple.com/library/archive/documentation/ToolsLanguages/Conceptual/Xcode\_Overview/RunningintheSimulator.html)
* [Центр приложений Visual Studio](https://visualstudio.microsoft.com/ru/app-center/)
* [Samsung Remote Test Lab](https://developer.samsung.com/remotetestlab/rtlDeviceList.action)
* [AWS Device Farm](https://aws.amazon.com/ru/device-farm/)
* [Huawei cloud debugging](https://developer.huawei.com/consumer/en/doc/development/Tools-Guides/remote-debugging-0000001073142313)
* [Device Farmer is a web application for debugging smartphones, smartwatches and other gadgets remotely](https://github.com/DeviceFarmer)
* [Appetize.io - Run native mobile apps in your browser](https://appetize.io)
* [Genymobile/scrcpy - обеспечивает отображение и управление устройствами Android через USB или TCP/IP](https://github.com/Genymobile/scrcpy)
* [Как тестировщики написали свою мобильную ферму для IOS](https://habr.com/ru/post/572668/)
* [Облачные платформы для мобильного тестирования](https://habr.com/ru/post/464433/)
* [Как мы сделали мобильные устройства круглосуточно доступными для распределенной QA-команды и не только](https://habr.com/ru/company/kaspersky/blog/663282/)
* [Docker Emulator for Android | VK](https://github.com/VKCOM/docker-emulator-android)

**Работа с логами**:

Работа с логами является важной частью процесса тестирования и отладки приложений. Логи содержат записи о событиях, происходящих в системе, и помогают тестировщикам выявлять ошибки, отслеживать выполнение процессов и анализировать поведение приложений.

* [Логи для тестировщика / Работа с логами в тестировании](https://www.youtube.com/watch?v=pAF1a\_2a\_6s)
* [О чём могут рассказать логи: важный инструмент в работе тестировщика](https://habr.com/ru/companies/yandex_praktikum/articles/739058/)
* [Tools for Log Analysis](https://medium.com/tensult/tools-for-log-analysis-461eb07c2d6b)
* [https://developer.apple.com/documentation/os/logging](https://developer.apple.com/documentation/os/logging)
* [Просмотр системных логов iOS](https://bulkin-me.turbopages.org/turbo/bulkin.me/s/notes/2884) и [еще](https://stackoverflow.com/questions/7277804/ios-iphone-ipad-ipodtouch-view-real-time-console-log-terminal)
* [Доклад: "Мониторинг приложения в проде" / Семён Мацепура (СберМаркет)](https://www.youtube.com/watch?v=lSS9eTlrNf8)
* [Как тестировщику работать с логами](https://testgrow.ru/article12)

**Тестирование производительности**:

Тестирование производительности – это процесс оценки скорости, масштабируемости и стабильности приложения или системы под нагрузкой. Оно позволяет определить, как система будет работать в реальных условиях использования и выявить ее проблемы с производительностью до выпуска в продакшен.

Основные популярные инструменты:

  1. [Apache JMeter](https://jmeter.apache.org/): Мощный инструмент с открытым исходным кодом для тестирования производительности веб-приложений.
  2. [LoadRunner](https://www.microfocus.com/en-us/products/loadrunner-professional/overview): Коммерческое решение от Micro Focus для проведения нагрузочного тестирования и анализа производительности.
  3. [Gatling](https://gatling.io/): Инструмент с открытым исходным кодом, написанный на Scala, для тестирования производительности и нагрузочного тестирования.
  4. [BlazeMeter](https://www.blazemeter.com/): Облачная платформа для проведения нагрузочного тестирования, интегрируемая с Apache JMeter и другими инструментами.
  5. [artillery.io](https://artillery.io): Позволяет создавать гибкие сценарии нагрузки с использованием простого синтаксиса YAML и запускать их с помощью командной строки. Artillery предоставляет широкие возможности для мониторинга и анализа результатов тестирования.
  6. [Яндекс.Танк](https://yandex.ru/dev/tank/): это инструмент для проведения нагрузочного тестирования веб-приложений и сервисов. Он обладает мощными возможностями по настройке сценариев нагрузки и поддерживает различные протоколы, включая HTTP, HTTPS, WebSocket и многие другие. Яндекс.Танк предоставляет удобный веб-интерфейс для настройки тестов и анализа результатов.
  7. [Google Lighthouse](https://developers.google.com/web/tools/lighthouse/): это автоматизированный инструмент для оценки качества веб-приложений и анализа их производительности. Он позволяет проводить аудит веб-страниц на предмет оптимизации производительности, доступности, SEO и других аспектов. Lighthouse доступен как в браузере Chrome, так и в виде командной строки для автоматизации тестирования.

Доп. материал:

* Apache JMeter + JMeter Result Analysis: [The Ultimate Guide](https://octoperf.com/blog/2017/10/19/how-to-analyze-jmeter-results/#understanding-jmeter-metrics)
* [Top 10 лучших инструментов для нагрузочного тестирования](https://www.performance-lab.ru/blog/luchshie-instrumenty-dlya-nagruzochnogo-testirovaniya)
* [10 инструментов тестирования производительности мобильных приложений](https://proglib.io/p/10-instrumentov-testirovaniya-proizvoditelnosti-mobilnyh-prilozheniy-2020-09-20)
* [Топ-15 бесплатных инструментов для нагрузочного тестирования](https://testengineer.ru/besplatnye-instrumenty-dlya-nagruzochnogo-testirovaniya/)
* [Использование Gatling. Разбираемся в тестировании HTTP](https://habr.com/ru/company/tinkoff/blog/658479/)
* [Тестирование производительности API с помощью K6](https://testengineer.ru/testirovanie-proizvoditelnosti-api-s-pomoshchyu-k6/)

**Mind maps**:

* [12 программ и сервисов для создания майндкарт](https://presium.pro/blog/software\_for\_maindmapping)
* [Как нарисовать карту приложения (mind map)](http://okiseleva.blogspot.com/2020/01/mind-map.html)
* [Mind map вместо тест-кейса, или Как визуализация позволяет тестировать приложение быстрее](https://habr.com/ru/company/badoo/blog/418353/)
* [Mind Map в помощь тестировщику](https://habr.com/ru/post/539756/)
* [Mind Map в тестировании - или легкий способ тестировать сложные приложения](https://habr.com/ru/post/515990/)
* [Mind Map для QA - Интеллектуальные карты](https://www.youtube.com/watch?v=N5B-3bi6\_88)

**TMS**:

* [Test IT](https://testit.software)
* [Allure TestOps](https://qameta.io)
* [Топ-12 лучших систем управления тестированием 2020](https://habr.com/ru/post/522474/)
* [Инструмент на века - гугл таблицы](https://docs.google.com/spreadsheets/u/0/)
* [Пришла пора отправить в отставку инструменты управления кейсами](https://software-testing.ru/library/testing/testing-tools/3588-its-time-to-retire-our-test-case-management-tools)
* [Системы управления тест кейсами. Какую выбрать для немедленной работы?](https://habr.com/ru/post/582608/)
* [Топ-10 лучших систем управления тестированием 2021](https://habr.com/ru/post/580526/)
* [QA-митап Redmadrobot 19/11, Google Sheet - универсальное подспорье для QA, Саша Строкин](https://www.youtube.com/watch?v=9aXGHFuivck)
* [10 Best free test management tools for 2022](https://theqalead.com/tools/free-test-management-tools/)
* [10 Best test management tools for JIRA in 2022](https://theqalead.com/tools/test-management-tools-for-jira/)
* [Successfully Managing Test Cases: Finding the Right Test Case Tool](https://blog.gurock.com/right-test-case-tool/)
* [Allure. В поисках почти идеальной TMS](https://habr.com/ru/post/571476/)
* [FAQ по баг-трекингу JIRA](https://www.youtube.com/watch?v=rxyc1OXTijc)
* Руководство по лучшему программному обеспечению для отслеживания проблем: [часть 1](https://habr.com/ru/company/otus/blog/660821/), [часть 2](https://habr.com/ru/company/otus/blog/666360/)
* [Баг-трекинговые системы: Jira и альтернативные варианты](https://testengineer.ru/bag-trekingovye-sistemy-jira-i-alternativnye-varianty/)
* [Рациональный выбор системы управления тестированием](https://habr.com/ru/company/domrf/blog/672780/)

**Полезные расширения для браузера**:

* [Vimbox Переводчик от Skyeng](https://chrome.google.com/webstore/detail/vimbox-%D0%BF%D0%B5%D1%80%D0%B5%D0%B2%D0%BE%D0%B4%D1%87%D0%B8%D0%BA-%D0%BE%D1%82-skye/heeikiohkfkolhmdodhcjdklofmhmmhn?hl=ru)
* [Violentmonkey](https://chrome.google.com/webstore/detail/violentmonkey/jinjaccalgkegednnccohejagnlnfdag), [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo?hl=ru) + [script](https://4pda.to/pages/go/?u=https%3A%2F%2Fraw.githubusercontent.com%2Fsodapng%2Fvoice-over-translation%2Fmaster%2Fvot.user.js)
* [Talend API Tester - Free Edition](https://chrome.google.com/webstore/detail/talend-api-tester-free-ed/aejoelaoggembcahagimdiliamlcdmfm)
* [Dimensions](https://chrome.google.com/webstore/detail/dimensions/baocaagndhipibgklemoalmkljaimfdj) - A tool for designers to measure screen dimensions
* [Page Ruler Redux](https://chrome.google.com/webstore/detail/page-ruler-redux/giejhjebcalaheckengmchjekofhhmal) - A Web Developer\Designer ruler to get pixel dimensions and positioning to measure elements on any web page
* [Tape](https://chrome.google.com/webstore/detail/tape/jmfleijdbicilompnnombcbkcgidbefb) - Measurement tools, rulers and grids
* [PerfectPixel](https://chrome.google.com/webstore/detail/perfectpixel-by-welldonec/dkaagdgjmgdmbnecmcefdhjekcoceebi?hl=ru)
* [GoFullPage - Full Page Screen Capture](https://chrome.google.com/webstore/detail/gofullpage-full-page-scre/fdpohaocaechififmbbbbbknoalclacl)
* [WhatFont](https://chrome.google.com/webstore/detail/whatfont/jabopobgcpjmedljpbcaablpmlmfcogm?hl=ru) - The easiest way to identify fonts on web pages
* [Spectrum](https://chrome.google.com/webstore/detail/spectrum/ofclemegkcmilinpcimpjkfhjfgmhieb) for color blindness checks
* [Check My Links](https://chrome.google.com/webstore/detail/check-my-links/ojkcdipcgfaekbeaelaapakgnjflfglf) for link checking
* [Selenium IDE](https://www.selenium.dev/selenium-ide/) for test data setup and debugging
* [Ranorex Selocity](https://www.ranorex.com/selocity/browser-extension/) for generating selectors
* [Bug Magnet](https://bugmagnet.org) for test data
* [Fake Filler](https://chrome.google.com/webstore/detail/fake-filler/bnjjngeaknajbdcgpfkgnonkmififhfo/related) for test data
* [Mokku](https://github.com/mukuljainx/Mokku): Mock API calls seamlessly
* [EditThisCookie](https://chrome.google.com/webstore/detail/editthiscookie/fngmhnnpilhplaeedifhccceomclgfbg) - менеджер cookie
* [Гуру Очистки](https://chrome.google.com/webstore/detail/clean-all-history-cache-c/elidgjfpciimeeeoeneeiifkmhadhkeh?hl=ru&) - удаление кеша & истории браузера
* [Responsive Viewer](https://chrome.google.com/webstore/detail/responsive-viewer/inmopeiepgfljkpkidclfgbgbmfcennb) - Show multiple screens once, Responsive design tester
* [Window Resizer](https://chrome.google.com/webstore/detail/window-resizer/kkelicaakdanhinjdeammmilcgefonfh?hl=ru&) - Resize the browser window to emulate various screen resolutions
* [Resolution Test](https://chrome.google.com/webstore/detail/resolution-test/idhfcdbheobinplaamokffboaccidbal) - An extension for developers to test web pages in different screen resolutions
* [Exploratory Testing Chrome Extension](https://chrome.google.com/webstore/detail/exploratory-testing-chrom/khigmghadjljgjpamimgjjmpmlbgmekj)
* [Web Developer Form Filler](https://chrome.google.com/webstore/detail/web-developer-form-filler/gbagmkohmhcjgbepncmehejaljoclpil/related?hl=en)
* [Web Developer](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm) - Adds a toolbar button with various web developer tools
* [Web Developer Checklist](https://chrome.google.com/webstore/detail/web-developer-checklist/iahamcpedabephpcgkeikbclmaljebjp) - Analyses any web page for violations of best practices
* [Docsumo Free OCR Software](https://chrome.google.com/webstore/detail/docsumo-free-ocr-software/ihmmlfacoffajllfpdfkdikgmoogbnph?ref=producthunt) - Screenshot any webpage or a portion of a webpage and immediately convert it into editable text
* [ColorZilla](https://chrome.google.com/webstore/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp) - Advanced Eyedropper, Color Picker, Gradient Generator and other colorful goodies
* [d3coder](https://chrome.google.com/webstore/detail/d3coder/gncnbkghencmkfgeepfaonmegemakcol) - Encoding/Decoding Plugin for various types of encoding like base64, rot13 or unix timestamp conversion
* [IE Tab](https://chrome.google.com/webstore/detail/ie-tab/hehijbfgiekmjfkfjpbkbammjbdenadd) - Display web pages using IE within Chrome. Use Java, Silverlight, ActiveX, Sharepoint, and more
* [Screencastify](https://chrome.google.com/webstore/detail/screencastify-screen-vide/mmeijimgabbpbgpdklnllpncmdofkcpn?hl=ru&) - The #1 screen recorder for Chrome. Capture, edit and share videos in seconds
* [Siteimprove](https://chrome.google.com/webstore/detail/siteimprove-accessibility/efcfolpjihicnikpmhnmphjhhpiclljc?hl=en-US) for accessibility
* [axe DevTools](https://chrome.google.com/webstore/detail/axe-devtools-web-accessib/lhdoppojpmngadmnindnejefpokejbdd?hl=ru&) - Web Accessibility Testing
* [WAVE](https://chrome.google.com/webstore/detail/wave-evaluation-tool/jbbplnpkjmmeebjpijfedlgcdilocofh) is a web accessibility evaluation tool
* [Proxy SwitchySharp](https://chrome.google.com/webstore/detail/proxy-switchysharp/dpplabbmogkhghncfbfdeeokoefdjegm?hl=ru&) - Manage and switch between multiple proxies quickly & easily
* [Browsec VPN](https://chrome.google.com/webstore/detail/browsec-vpn-free-vpn-for/omghfjlpggmjjaagoclmmobgdodcjboh?hl=ru&) - Free VPN for Chrome
* [Otsledit](https://chrome.google.com/webstore/detail/price-tracker-otsledit/ibamclpibpnhmkaphhemfbljmenlpbch?hl=ru&) - Отслеживайте изменения контента на веб-страницах, просматривайте историю мониторинга
* [Ruto](https://chrome.google.com/webstore/detail/ruto-xpath-finder/ilcoelkkcokgeeijnopjnolmmighnppp?hl=ru&) - XPath Finder

**Программы для снятия скриншотов и записи видео**:

* Windows: скриншот всего экрана Prtsc+Fn, выделяемой части Win+Shift+S, запись видео Win+G
* [Screenpic - больше чем программа для скриншотов](https://screenpic.net/ru/)
* [ScreenRec](https://screenrec.com)
* [Делайте снимки экрана в один клик со Скриншотером Mail.ru](https://screenshoter.mail.ru)
* [ShareX - Screen capture, file sharing and productivity tool](https://getsharex.com)
* [Greenshot is a light-weight screenshot software tool for Windows](https://getgreenshot.org)
* [Flameshot - powerful yet simple to use screenshot software](https://flameshot.org)
* [Bandicam - это лучшая программа для записи экрана, игр и видеоустройств](https://www.bandicam.com/ru/)
* [Recordit - fast screencasts](https://recordit.co)
* [ScreenToGif - screen, webcam and sketchboard recorder with an integrated editor](https://www.screentogif.com)
* [OBS Studio - бесплатная программа с открытым исходным кодом для записи видео и потокового вещания](https://obsproject.com/ru)
* [Snagit lets you quickly capture your screen](https://www.snagit.com)
* [Joxi - бесплатная программа для снятия скриншотов](http://joxi.ru)
* [Movavi Screen Recorder - захват экрана в один клик](https://www.movavi.ru/screen-capture/)
* [PicPick - захват экрана, редактор изображений, выбор цвета, цветовая палитра, пиксельная линейка, угломер, перекрестие, грифельная доска и многое другое](https://picpick.app/ru/)
* [Apowersoft Screen Capture Pro - multi-functional Screenshot Program](https://www.apowersoft.com/screen-capture-pro)
* [Screencast-o-matic - Free Screen Recorder](https://screencast-o-matic.com/screen-recorder)
* [Loom](https://www.loom.com) - Record quick videos of your screen and cam
* [ImageOptim](https://imageoptim.com/mac) makes images load faster
* [Monosnap](https://monosnap.com) - take screenshots in one click
* [BugCatcher](https://bugcatcher.pro) - Создает скриншот или видео, Копирует контекст (OS, browser, hardware e.t.c ), Копирует errorlog, Отправляет в багтрекинг систему

**Linux**

* [Обсуждение зачем вообще уметь в Linux](https://software-testing.ru/forum/index.php?/topic/23210-linuxnix-znanija-dlja-testirovshika/)
* [Введение в UNIX/LINUX для тестировщиков](https://www.youtube.com/watch?v=fpujpnsPiuA)
* Command Line с нуля (Bash, Unix): [часть 1](https://www.youtube.com/watch?v=jRYggi1pNkM), [2](https://www.youtube.com/watch?v=ULhRW6mFzYI), [3](https://www.youtube.com/watch?v=38E3pE-jh38), [4](https://www.youtube.com/watch?v=ekM8q2SL5qM), [5](https://www.youtube.com/watch?v=\_nme7F-luJ0)
* [Linux Command Line Cheat Sheet by DaveChild](https://cheatography.com/davechild/cheat-sheets/linux-command-line/)
* [Базовые команды Linux для тестировщиков и не только](https://habr.com/ru/post/481398/) + [картинка](https://wizardzines.com/networking-tools-poster.pdf)
* [Бесплатный курс “Основы командной строки”](https://ru.hexlet.io/courses/cli-basics)
* [How To Run / Execute Command Using SSH](https://www.cyberciti.biz/faq/unix-linux-execute-command-using-ssh/)
* [TOP 70+ Best UNIX Interview Questions With Answers](https://www.softwaretestinghelp.com/unix-interview-questions/)
* [Автоматизация рутины. Скачиваем файлы через bash](http://okiseleva.blogspot.com/2021/11/bash.html)

**RegExp**:

* [Регулярные выражения (regexp) - основы](https://habr.com/ru/post/545150/)
* [Мягкое введение в Regex](https://telegra.ph/Myagkoe-vvedenie-v-Regex-03-19)
* [https://regex101.com/](https://regex101.com)
* [http://myregexp.com/](http://myregexp.com)
* [https://regexr.com/](https://regexr.com)

**Разное**:

* [HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML)/[CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)/[JavaScript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
* [Подборка шпаргалок](https://overapi.com)
* [Курс Тестирование ПО. Занятие 20. Инструменты для сбора тестовых доказательств (Test Evidences)](https://www.youtube.com/watch?v=4CBBWV6ldcs)
* [AnyDesk](https://anydesk.com/ru) - подключение к удаленному рабочему столу любой платформы
* [LetsView](https://letsview.com) - Free Wireless Screen Mirroring
* [clumsy](https://github.com/jagt/clumsy) makes your network condition on Windows significantly worse, but in a managed and interactive manner
* [netem](https://wiki.linuxfoundation.org/networking/netem) provides Network Emulation functionality for testing protocols by emulating the properties of wide area networks
* [Полезные ресурсы для тестировщика. Генераторы данных, изображений, текста. Сравнение текста, файлов.](https://www.youtube.com/watch?v=-oWstXJFI2Y)
* [Десять классных генераторов тестовых данных](https://testengineer.ru/klassnye-generatory-testovyh-dannyh/)
* [Dynamic Dummy Image Generator](https://dummyimage.com)
* [Just add your desired image size (width & height) after our URL, and you'll get a random image](https://picsum.photos)
* [SortSite](https://www.powermapper.com/products/sortsite/) checks any website for broken links, spelling errors, browser compatibility, accessibility, web standards validation and search engine issues.
* [PowerMapper](https://www.powermapper.com/products/mapper/) - One click site mapping
* [File generator](https://file.generator.teremokgames.com)
* [Screen Dimensions for Devices + my device](https://yesviz.com)
* [Супер простой сервис для генерации разных HTTP-кодов](https://httpstat.us)
* [Бесплатные одноразовые e-mail](https://www.mailinator.com)
* [Tools for Software Testing](http://qala.io/blog/test-tools.html)
* [Get Credit Card Numbers](https://www.getcreditcardnumbers.com)
* [Тестовые банковские карты](https://securepayments.sberbank.ru/wiki/doku.php/test\_cards)
* [Stripe test card numbers](https://stripe.com/docs/testing#cards)
* ["Can I use"](https://caniuse.com) provides up-to-date browser support tables for support of front-end web technologies on desktop and mobile web browsers.
* [Chrome Remote Desktop - теперь подключаемся к ПК и со смартфона на Android](https://habr.com/ru/post/219783/)
* [Пингуем из Excel](https://pikabu.ru/story/pinguem\_iz\_excel\_8165074)
* [Тулзы ручного тестировщика приложений на базе Windows](https://habr.com/ru/post/554300/)
* [One click website testing tool](https://www.powermapper.com)
* [Инструменты для тестирования - Что должен знать тестировщик без опыта.](https://www.youtube.com/watch?v=RPllElm0QQI)
* [Генератор номеров банковских счетов](https://infostart.ru/public/1075832/)
* [Программа для генерации банковских счетов и генерации ключа проверки](https://github.com/fleytman/generator\_bank\_accounts)
* [mChat is a real-time messaging app written in Swift for iOS devices](https://github.com/vitaliy-paliy/Messenger)
* [Telegram iOS Source Code Compilation Guide](https://github.com/TelegramMessenger/Telegram-iOS)
* [Как установить, настроить и использовать подсистему Linux в Windows 10. Обновленный Windows Terminal](https://www.youtube.com/watch?v=UJ-Sncozy58)
* [Багред - ставите задачу в баг-трекер? Проверьте название на стоп-слова!](http://bugred.ru)
* [Top Cross-Browser Testing Tools to Test from Different Geo-Locations](https://hackernoon.com/top-cross-browser-testing-tools-to-test-from-different-geo-locations-nx2837uk)
* [10 best data engineering tools and technologies in 2021](https://theqalead.com/tools/best-data-engineering-tools/)
* [Кракозябры](https://disk.yandex.ru/d/ShyvfnM15MXacA)
* [Прорисовка и визуализация сервисов, систем, архитектуры и всего остального](https://t.me/pmdaily/824)
* RF SCreater - Генератор паспортов РФ
* [Генератор личностей EN](https://vk.com/away.php?to=http%3A%2F%2Frandomprofile.com%2Fusa-random-names\&cc\_key=)
* [Генератор личностей RUS](https://vk.com/away.php?to=http%3A%2F%2Frandus.ru%2F\&cc\_key=)
* [Почтовый сервис для создания временного ящика](https://temp-mail.org)
* [Одноразовые и Бесплатные адреса электронной почты](https://yopmail.com/ru/)
* [Большой тред о полезных сервисах для разработчиков](https://twitter.com/bespoyasov/status/1430537219241123845?s=21)
* [Install any command on any operating system](https://command-not-found.com)
* [ngrok](https://ngrok.com) - One command for an instant, secure URL to your localhost server through any NAT or firewall
* [projector-docker](https://github.com/JetBrains/projector-docker) - is a technology to run and access Swing GUI applications remotely
* [Code With Me](https://www.jetbrains.com/ru-ru/code-with-me/) - Сервис JetBrains для совместной работы над кодом
* [Calendly](https://calendly.com) is your hub for scheduling meetings
* [Воркшоп: Инструменты для дебага сети / Евгений Рядовой (СберМаркет)](https://www.youtube.com/watch?v=Bf9WDqwHWAc)
* [Как установить два независимых Chrome браузера на один ПК](https://www.youtube.com/watch?v=tyg15uz2F1M)
* [Инструменты коммуникации для QA, и не только](https://www.youtube.com/watch?v=W2N9ALAqHSE)
* [Application monitoring and error tracking software](https://sentry.io/welcome/)
* [Katacoda - Learn new technologies using real environments right in your browser](https://www.katacoda.com)
* [TestRail и дополнительные инструменты для тестировщика](https://www.youtube.com/watch?v=XQ7MoUT7rEk)
* [Как тестируют документацию в Test IT](https://habr.com/ru/company/testit-tms/blog/564666/)
* [Как правильно оформить баг-репорт](https://testit.software/blog/post/kak-pravilno-oformit-bag-report)
