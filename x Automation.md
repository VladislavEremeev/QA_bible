ВНИМАНИЕ!!! Attention! Achtung! Attenzione! Увага!
Это даже не черновик, а франкенштейн из обрывков. Выкладываю его сюда просто чтобы обозначить, что когда-нибудь я начну работу над этим разделом (не ближайший год точно), а также для того, чтобы желающие могли это начать уже сейчас. Может быть кто-то просто найдет в этом хаосе что-то полезное.

<h2><i>Автоматизированное тестирование</i> программного обеспечения — основные понятия</h2>
<img src="https://lh5.googleusercontent.com/kmaGmmkcvQitnryKwKezyN_1AIw_lV9w4QW42oGgAbZD3gKKR1EK8sBMUp2eWyU7_J6tGgd9ea2yOsQHbsgzQWX1p1szTFRCAcl0EfvcJlNCGguIHacGr7p7gdcM3fEWrLpiMcA" align="center">
<h1>Задачи автоматического тестирования</h1>
От более важного к менее:

<ol>
<li><strong>Обнаружение дефектов как можно раньше.</strong> До того как увидит пользователь, до того как выложить на сервер, до того как отдать на тестирование, до того как закоммитить.</li>
<li><strong>Локализация проблемы.</strong> Тест затрагивает лишь часть кода.</li>
<li><strong>Ускорение разработки.</strong> Исполнение теста происходит гораздо быстрее ручной проверки.</li>
<li><strong>Актуальная документация.</strong> Тест представляет из себя простой и гарантированно актуальный пример использования.</li>
</ol>
Самый незамысловатый подход к автоматизации тестирования, который только можно придумать, просто взять тест-кейсы, созданные для ручного тестирования, и автоматизировать их на уровне пользовательского интерфейса (Ge используя инструменты наподобие Selenium. В то же время, это наименее эффективный подход. Автоматические тесты на уровне UI медленны, уязвимы к любым изменениям, их трудно поддерживать.

Пирамида автоматизации Майка Кона отлично иллюстрирует более эффективный подход. Ширина каждого уровня пирамиды показывает, сколько тестов должно быть на каждом уровне по сравнению с другими.

На нижнем уровне пирамиды находятся компонентные, или юнит-тесты. Они должны составлять <i>большинство</i> ваших тестов. Например, чтобы протестировать класс, который вычисляет проценты с суммы, создается юнит-тест, передающий процентную ставку <i>x</i> и баланс <i>y.</i> Ожидаемый результат: корректное вычисление суммы процентов с нужной точностью.

Средний уровень занимают тесты, которые верифицируют бизнес-поведение (но <i>не через GUI</i>!). Такие тесты иногда называют API тестами. Если вы используете методологию «разработки через поведение» (BDD, behavior-driven development), ваши автоматические тесты будут относиться к этому уровню. Вам может понадобиться довольно большое количество тестов этого уровня, но всё равно их должно быть меньше, чем юнит-тестов. Такие тесты могут затрагивать несколько компонентов одновременно и проверять поведение продукта с точки зрения бизнеса. Пример: после вычисления процента по депозиту нужная сумма добавляется к балансу.

Верхний уровень пирамиды — автоматические тесты, которые непосредственно затрагивают пользовательский интерфейс. Их должно быть намного меньше, чем остальных. Пример такого теста: после начисления процента в банковской выписке отображается правильная, новая сумма.

И, «вишенка на тортике» — ручные тесты. Некоторые виды тестирования не могут быть автоматизированы, допустим, исследовательское тестирование или тестирование юзабилити, но в идеале стоит стремиться минимизировать объем мануальных тестов.

Еще несколько важных принципов, связанных с пирамидой автоматизации:

<i><strong>Избегайте дублирования тестов на разных уровнях.</strong></i><i> </i>Нет смысла повторять одни и те же тесты на разных уровнях. Например, если граничные значения были проверены на уровне юнит-тестов, не стоит повторять их на уровне GUI — таким образом мы вряд ли получим новую информацию.

В целом, там, где это возможно, стоит <i><strong>стремиться к сдвигу тестов на более низкий уровень</strong></i>. Допустим, проверить вычисление процентов с отрицательной суммы наверняка возможно на «среднем уровне» или даже на уровне юнит-тестов, так зачем делать это на уровне пользовательского интерфейса? Автоматизировать тесты на более низком уровне эффективнее, это позволяет раньше обнаруживать дефекты, экономит время и деньги.

<strong>Автоматизированное тестирование программного обеспечения</strong> (<strong>Software Automation Testing</strong>) — это процесс верификации программного обеспечения, при котором основные функции и шаги теста, такие как запуск, инициализация, выполнение, анализ и выдача результата, выполняются автоматически при помощи инструментов для автоматизированного тестирования.

<strong>Специалист по автоматизированному тестированию программного обеспечения</strong> (<strong>Software Automation Tester</strong>) — это технический специалист (тестировщик или разработчик программного обеспечения), обеспечивающий создание, отладку и поддержку работоспособного состояния тест скриптов, тестовых наборов и инструментов для автоматизированного тестирования.

<strong>Инструмент для автоматизированного тестирования</strong> (<strong>Automation Test Tool</strong>) — это программное обеспечение, посредством которого специалист по автоматизированному тестированию осуществляет создание, отладку, выполнение и анализ результатов прогона тест скриптов.

<strong>Тест Скрипт</strong> (<strong>Test Script</strong>) — это набор инструкций, для автоматической проверки определенной части программного обеспечения.

<strong>Тестовый набор</strong> (<strong>Test Suite</strong>) — это комбинация тест скриптов, для проверки определенной части программного обеспечения, объединенной общей функциональностью или целями, преследуемыми запуском данного набора.

<strong>Тесты для запуска</strong> (<strong>Test Run</strong>) — это комбинация тест скриптов или тестовых наборов для последующего совместного запуска (последовательного или параллельного, в зависимости от преследуемых целей и возможностей инструмента для автоматизированного тестирования).

<h1>Что нужно автоматизировать?</h1>
Спрашивая: «<strong>Что автоматизировать?</strong>», необходимо сначала ответить на вопрос: «Целесообразна ли <strong>автоматизация тестирования</strong> в условиях проекта». Если ответ «ДА», то необходимо, исходя из требований к объекту тестирования, создать план, по которому будут разрабатываться <strong>автоматизированные тесты</strong>. Создавая подобный документ, вы должны четко представлять, «<strong>что автоматизировать?</strong>«, «<a href="http://www.protesting.ru/automation/functional/howtoauto.html"><strong>как автоматизировать?</strong></a>« и «<a href="http://www.protesting.ru/automation/functional/testtool.html"><strong>чем автоматизировать?</strong></a>«. Не будем вдаваться в подробности, как и чем тестировать ту или иную функцию, просто перечислим места, <strong>где</strong>, на наш взгляд, <strong>нужно применять автоматизацию</strong>:

<ol>
<li>Труднодоступные места в системе (бэкенд процессы, логирование файлов, запись в БД)</li>
<li>Часто используемая функциональность, риски от ошибок в которой достаточно высоки. Автоматизировав проверку критической функциональности, можно гарантировать быстрое нахождение ошибок, а значит и быстрое их решение.</li>
<li>Рутинные операции, такие как переборы данных (формы с большим количеством вводимых полей. Автоматизировать заполнение полей различными данными и их проверку после сохранения)</li>
<li>Валидационные сообщения (Автоматизировать заполнение полей не корректными данными и проверку на появление той или иной валидации)</li>
<li>Длинные end-to-end сценарии</li>
<li>Проверка данных, требующих точных математических расчетов</li>
<li>Проверка правильности поиска данных</li>
</ol>
А также, многое другое, в зависимости от требований к тестируемой системе и возможностей выбранного инструмента для тестирования.

<strong>Для</strong> более <strong>эффективного использования автоматизации тестирования</strong> лучше разработать отдельные <a href="http://www.protesting.ru/testing/testcase.html"><strong>тест кейсы</strong></a> проверяющие:

<ul>
<li>Базовые операции создания/чтения/изменения/удаления сущностей (так называемые CRUD операции — Create / Read / Update / Delete).</li>
</ul>
<strong>Пример</strong>: создание, удаление, просмотр и изменение данных о пользователе.

<ul>
<li>Типовые сценарии использования приложения, либо отдельные действия.</li>
</ul>
<strong>Пример</strong>: пользователь заходит на почтовый сайт, листает письма, просматривает новые, пишет и отправляет письмо, выходит с сайта. Это так называемый <strong>end-to-end сценарий</strong>, который проверяет совокупность действий. Мы предлагаем вам использовать именно такие сценарии, так как они позволяют вернуть систему в состояние, максимально близкое к исходному, а значит – минимально влияющее на другие тесты.

<ul>
<li>Интерфейсы, работы с файлами и другие моменты, неудобные для тестирования вручную.</li>
</ul>
<strong>Пример</strong>: система создает некоторый xml файл, структуру которого необходимо проверить.

Это и есть та функциональность, от автоматизации тестирования которой, можно получить наибольшую отдачу.

<h1>Выбор инструмента автоматизации тестирования</h1>
Выбор инструмента зачастую <strong>зависит от объекта тестирования и требований к тестовым сценариям</strong>, т.к. инструменты тестирования не могут поддерживать абсолютно все технологии, используемые при разработке приложений. То есть, выбор инструмента сводится к банальному методу проб и ошибок. В итоге, нередко мы выбираем несколько инструментов для тестирования функций приложения. Например, GUI мы проверяем посредством <strong>Mercury WinRunner</strong>, бэкенд процессы — используя <strong>«java based test tools»</strong> или другие инструменты. Основные <strong>аспекты выбора инструмента автоматизации тестирования</strong> рассмотрены в разделе «<a href="http://www.protesting.ru/automation/functional/howtoauto.html"><strong>Как автоматизировать?</strong></a>«.

Рассмотрим <strong>инструменты для автоматизированного функционального тестирования</strong> от разных производителей:

<table>
<tr>
<td><strong>Компания</strong></td>
<td><strong>Инструмент</strong></td>
</tr>
<tr>
<td><strong>Hewlett-Packard (Mercury Interactive)</strong></td>
<td>QuickTest Professional, WinRunner</td>
</tr>
<tr>
<td><strong>IBM Rational</strong></td>
<td>Rational Robot, Rational Functional Tester</td>
</tr>
<tr>
<td><strong>Borland (Segue)</strong></td>
<td>SilkTest</td>
</tr>
<tr>
<td><strong>AutomatedQA Corp</strong></td>
<td>TestComplete</td>
</tr>
<tr>
<td><strong>Microsoft</strong></td>
<td>Microsoft VS 2005</td>
</tr>
<tr>
<td><strong>SeleniumHQ</strong></td>
<td>Selenium</td>
</tr>
</table>
Отдельным пунктом также хочется выделить <strong>Java библиотеки для автоматизированного тестирования</strong> (<i>java based test tools and libraries</i>):

<table>
<tr>
<td><strong>Инструмент</strong></td>
<td><strong>Описание</strong></td>
</tr>
<tr>
<td><a href="http://docs.seleniumhq.org/"><strong>Selenium</strong></a></td>
<td>Selenium is a set of different software tools each with a different approach to supporting test automation of web applications across many platforms.</td>
</tr>
<tr>
<td>Watij</td>
<td>Watij (pronounced wattage) stands for Web Application Testing in Java. Watij is a pure Java API created to allow for the automation of web applications. Based on the simplicity of Watir and enhanced by the power of Java, Watij automates functional testing of web applications through a real browser. Currently Watij supports automating Internet Explorer on Windows only. Future plans are in place to support others like Mozilla.</td>
</tr>
<tr>
<td><a href="http://htmlunit.sourceforge.net/"><strong>HtmlUnit</strong></a></td>
<td>HtmlUnit is a «browser for Java programs». It models HTML documents and provides an API that allows you to invoke pages, fill out forms, click links, etc... just like you do in your «normal» browser. It has fairly good JavaScript support (which is constantly improving) and is able to work even with quite complex AJAX libraries, simulating either Firefox or Internet Explorer depending on the configuration you want to use. It is typically used for testing purposes or to retrieve information from web sites. HtmlUnit is not a generic unit testing framework. It is specifically a way to simulate a browser for testing purposes and is intended to be used within another testing framework such as JUnit or TestNG</td>
</tr>
<tr>
<td><a href="http://httpunit.sourceforge.net/"><strong>HttpUnit</strong></a></td>
<td>Written in Java, HttpUnit emulates the relevant portions of browser behavior, including form submission, JavaScript, basic http authentication, cookies and automatic page redirection, and allows Java test code to examine returned pages either as text, an XML DOM, or containers of forms, tables, and links. When combined with a framework such as JUnit, it is fairly easy to write tests that very quickly verify the functioning of a web site.</td>
</tr>
<tr>
<td><a href="http://jameleon.sourceforge.net/"><strong>Jamaleon</strong></a></td>
<td>Jameleon is an automated testing framework that can be easily used by technical and non-technical users alike. One of the main concepts behind Jameleon is to create a group of keywords or tags that represent different screens of an application. All of the logic required to automate each particular screen can be defined in Java and mapped to these keywords. The keywords can then be organized with different data sets to form test scripts without requiring an in-depth knowledge of how the application works. The test scripts are then used to automate testing and to generate manual test case documentation.</td>
</tr>
<tr>
<td><a href="http://junit.org/"><strong>Junit</strong></a></td>
<td>JUnit is a simple framework to write repeatable tests. It is an instance of the xUnit architecture for unit testing frameworks.</td>
</tr>
<tr>
<td><a href="http://abbot.sourceforge.net/"><strong>Abbot</strong></a></td>
<td>Abbot is a simple framework for unit and functional testing of Java GUIs. Facilitates generating user actions and examining component state. Supports recording and playback on any Java application.</td>
</tr>
<tr>
<td><a href="http://www.marathontesting.com/"><strong>Marathon</strong></a></td>
<td>With Marathon you capture user interactions on the applications and also insert assertions to verify that correct processing is taking place. The generated raw script can be re-factored to modules for efficient reuse and maintainability. Replay the scripts either manually or integrate Marathon into your build process for automatic execution of the test suites.</td>
</tr>
</table>
Так же существует огромное количество фреймворков и инструментов, ориентированных не только на Java, но и на другие языки программирования, такие как: ruby, php, C#, javascript, python, perl и т.д. 

<h1>Инструменты для нагрузочного тестирования</h1>
<strong>Коммерческие инструменты</strong> для автоматизированного нагрузочного тестирования:

<table>
<tr>
<td><strong>Hewlett-Packard (Mercury Interactive)</strong></td>
<td><a href="https://h10078.www1.hp.com/cda/hpms/display/main/hpms_content.jsp?zn=bto&cp=1-11-126-17_4000_100__"><strong>HP Performance Center</strong></a> (включает <a href="http://www8.hp.com/us/en/software-solutions/software.html?compURI=1175451"><strong>HP LoadRunner</strong></a>)</td>
</tr>
<tr>
<td><strong>IBM Rational</strong></td>
<td><a href="http://www-01.ibm.com/software/awdtools/tester/performance/"><strong>Rational Performance Tester</strong></a></td>
</tr>
<tr>
<td><strong>Borland (Segue)</strong></td>
<td><a href="http://www.borland.com/us/products/silk/silkperformer/"><strong>Silk Performer</strong></a></td>
</tr>
<tr>
<td><strong>SmartBear</strong></td>
<td><a href="http://smartbear.com/products/qa-tools/load-testing-tool"><strong>LoadComplete Web Load Testing</strong></a></td>
</tr>
<tr>
<td><strong>Neotys</strong></td>
<td><a href="http://www.neotys.com/product/overview-neoload.html"><strong>NeoLoad</strong></a></td>
</tr>
</table>
Отдельным пунктом выделим <strong>бесплатные инструменты</strong> для автоматизированного нагрузочного тестирования:

<ul>
<li><a href="http://jakarta.apache.org/jmeter/"><strong>Jmeter</strong></a> - an Apache Jakarta project that can be used as a load testing tool for analyzing and measuring the performance of a variety of services</li>
<li><a href="http://grinder.sourceforge.net/"><strong>Grinder</strong></a> - a load testing framework that makes it easy to run a distributed test using many load injector machines. Test scripts are written in Jython, and HTTP scripts can be recorded easily from a browser session.</li>
</ul>
<h1>Как автоматизировать?</h1>
<strong>Во первых</strong>, вы должны обратить внимание <strong>насколько хорошо инструмент для автоматизации распознает элементы управления</strong> в вашем приложении. В случае когда элементы не распознаются стоит поискать плагин, либо соответствующий модуль. Если такового нет – от инструмента лучше отказаться. Чем больше элементов может распознать инструмент – тем больше времени вы сэкономите на написании и поддержке скриптов!

<strong>Во-вторых</strong>, нужно обратить внимание на то <strong>сколько времени требуется на поддержку скриптов</strong> написанных с помощью выбранного инструмента. Для этого запишите простой скрипт который выбирает пункт меню, а потом представьте, что изменился пункт меню который необходимо выбрать. Если для восстановления работоспособности сценария вам придется перезаписать скрипт целиком, то инструмент не оптимален, так как реальные сценарии гораздо сложнее. Лучше всего тот инструмент, который позволяет вам вынести название кнопки в переменную в начале скрипта и быстро заменить ее значение. В идеале – описать меню как класс.

<strong>И последний момент</strong> на который нужно обратить внимание – <strong>насколько удобен инструмент для написания новых скриптов</strong>. Сколько требуется на это времени, насколько можно структурировать код (поддержка ООП), насколько код читаем, насколько удобна среда разработки для рефакторинга (переработки кода) и т.п.

Лучше всего для принятия правильного решения об автоматизации отвечать на вопросы <strong>«Зачем? Что? Как?»</strong> именно в таком порядке. Это поможет избежать впустую потраченных времени нервов и финансов. С другой стороны вы сможете получить <strong>надежность, скорость и качество</strong>!!!

<source>
</source>
Flaky-тесты или «мигающие» авто-тесты, т.е. такие тесты, которые по независящим от нас внешним обстоятельствам или из-за трудновоспроизводимых багов, могут иногда падать, хотя всё остальное время они проходят успешно

<strong>Фикстуры</strong> - это по сути тестовые данные. Они нужны для unit-тестирования. Это могут быть как данные в базе, так и обычные файлы (обычно 2 варианта, до и после обработки так скажем). Каждый раз когда запускаются тесты, эти данные используются для установления начального состояния системы, что бы тесты всегда выполнялись предсказуемо.

<strong>Сеанс-это один вызов pytest, включая все тесты, выполняемые в нескольких каталогах.</strong>

<source>
</source>
Мне нравится разделять функциональные и модульные тесты, потому что функциональные тесты должны ломаться, только если мы намеренно изменяя функциональность системы, в то время как модульные тесты могут сломаться во время рефакторинга или изменения реализации.

Проект содержит два типа файлов __init__.py: найденные в каталоге src/ и те, которые находятся в tests/. Файл src/tasks/__init__.py сообщает Python, что каталог является пакетом. Он также выступает в качестве основного интерфейса для пакета, когда кто-то использует import tasks. Он содержит код для импорта определенных функций из api.py, так что cli.py и наши тестовые файлы могут обращаться к функциям пакета, например tasks.add(), вместо того, чтобы выполнять task.api.add (). Файлы tests/func/__init__.py и tests/unit/__init__.py пусты. Они указывают pytest подняться вверх на один каталог, чтобы найти корень тестового каталога и pytest.ini-файл.

Файл pytest.ini не является обязательным. Он содержит общую конфигурацию pytest для всего проекта. В вашем проекте должно быть не более одного из них. Он может содержать директивы, которые изменяют поведение pytest, например, настрйки списка параметров, которые всегда будут использоваться

Файл conftest.py также является необязательным. Он считается pytest как «local plugin» и может содержать hook functions и fixtures. <i>Hook functions</i> являются способом вставки кода в часть процесса выполнения pytest для изменения работы pytest. Fixtures — это setup и teardown функции, которые выполняются до и после тестовых функций и могут использоваться для представления ресурсов и данных, используемых тестами.

Использование <i>usefixtures</i> почти то же самое, что указание имени фикстуры в списке параметров метода теста. Единственное отличие состоит в том, что тест может использовать возвращаемое значение фикстуры, только если оно указано в списке параметров. Тест, использующий фикстуру из-за использования <i>usefixtures</i>, не может использовать возвращаемое значение фикстуры.

С параметризованными функциями вы можете запускать эту функцию несколько раз. Но с параметризованными фикстурами каждая тестовая функция, использующая эту фикстуру, будет вызываться несколько раз.

<ul>
<li><i>pytest.ini</i>: Это основной файл конфигурации Pytest, который позволяет вам изменить поведение по умолчанию. Поскольку вы можете внести довольно много изменений в конфигурацию, большая часть этой главы посвящена настройкам, которые вы можете сделать в pytest.ini.</li>
<li><i>conftest.py</i>: Это локальный плагин, позволяющий подключать хук-функции и фикстуры для каталога, в котором существует файл conftest.py, и всех его подкаталогов. Файл conftest.py описан в главе 5 «Плагины» на стр. 95.</li>
<li><i>__init__.py</i>: При помещении в каждый test-подкаталог этот файл позволяет вам иметь идентичные имена test-файлов в нескольких каталогах test. Мы рассмотрим пример того, что пойдет не так без файлов __init__.py в тестовых каталогах в статье «Избегание коллизий имен файлов» на стр. 120.</li>
</ul>
Откройте терминал, перейдите в директорию, в которой вы работаете с автотестами, и активируйте виртуальное окружение.

После чего выполните в терминале команду:

pip freeze > requirements.txt

Эта команда сохранит все версии пакетов в специальный файл <strong>requirements.txt.</strong>

Как их оттуда достать? Попробуйте создать новое виртуальное окружение (если нужно, вернитесь в <a href="https://stepik.org/lesson/25969/step/3?unit=196192">модуль 1</a> за инструкциями) и активировать. После чего выполните команду:

pip install -r requirements.txt

В свежем окружении все пакеты установлены одной командой!

СЕЛЕКТОРЫ:

<a href="https://www.youtube.com/watch?v=_TNh2ydpoOw">https://www.youtube.com/watch?v=_TNh2ydpoOw</a>

Точный

Уникальный

Простой+понятный

Устойчивые к изменениям

Используйте комбинации, отрицания, не искать по тексту, чайлдам

<a href="https://github.com/JakUi/stepik-auto-tests-course/blob/master/%D0%A4%D0%B8%D0%BA%D1%81%D1%82%D1%83%D1%80%D1%8B%20%D0%B8%20%D0%BA%D0%BB%D0%B0%D1%81%D1%81%D1%8B.txt">https://github.com/JakUi/stepik-auto-tests-course/blob/master/%D0%A4%D0%B8%D0%BA%D1%81%D1%82%D1%83%D1%80%D1%8B%20%D0%B8%20%D0%BA%D0%BB%D0%B0%D1%81%D1%81%D1%8B.txt</a>

<a href="https://habr.com/ru/company/yandex/blog/242795/">https://habr.com/ru/company/yandex/blog/242795/</a>

<strong>PyTest плагины</strong>

<a href="https://plugincompat.herokuapp.com/">https://plugincompat.herokuapp.com/</a>

<strong>PyTest документация фул</strong>

<a href="https://docs.pytest.org/en/latest/contents.html">https://docs.pytest.org/en/latest/contents.html</a>

Всё про всё выше

<a href="https://stepik.org/lesson/237258/step/1?unit=209646">https://stepik.org/lesson/237258/step/1?unit=209646</a>

Полезные фреймворки

<a href="https://stepik.org/lesson/239062/step/1?unit=211485">https://stepik.org/lesson/239062/step/1?unit=211485</a>

Всё по xpath <a href="https://stepik.org/lesson/102555/step/10?unit=196193">https://stepik.org/lesson/102555/step/10?unit=196193</a>

CSS-селекторы:

<a href="https://developer.mozilla.org/ru/docs/Web/CSS/CSS_%D0%A1%D0%B5%D0%BB%D0%B5%D0%BA%D1%82%D0%BE%D1%80%D1%8B">https://developer.mozilla.org/ru/docs/Web/CSS/CSS_%D0%A1%D0%B5%D0%BB%D0%B5%D0%BA%D1%82%D0%BE%D1%80%D1%8B</a>

<a href="https://www.w3schools.com/cssref/css_selectors.asp">https://www.w3schools.com/cssref/css_selectors.asp</a>

Селениум

<a href="https://habr.com/ru/post/250975/">https://habr.com/ru/post/250975/</a>

<a href="https://selenium-python.readthedocs.io/locating-elements.html#locating-hyperlinks-by-link-text">https://selenium-python.readthedocs.io/locating-elements.html#locating-hyperlinks-by-link-text</a>

html атрибуты

<a href="https://www.w3schools.com/tags/ref_attributes.asp">https://www.w3schools.com/tags/ref_attributes.asp</a>

Чего еще можно ждать, пока не кликнет

<a href="https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.support.expected_conditions">https://selenium-python.readthedocs.io/api.html#module-selenium.webdriver.support.expected_conditions</a>

Общее полезные ресурсы

<a href="https://stepik.org/lesson/171979/step/1?unit=146657">https://stepik.org/lesson/171979/step/1?unit=146657</a>

Всё про QA

<a href="https://dou.ua/lenta/articles/qa-engineer-position/">https://dou.ua/lenta/articles/qa-engineer-position/</a>

<a href="https://dou.ua/lenta/articles/qa-automation-engineer-position/">https://dou.ua/lenta/articles/qa-automation-engineer-position/</a>

Всё про GIT

<a href="https://stepik.org/lesson/187065/step/12?unit=161976">https://stepik.org/lesson/187065/step/12?unit=161976</a>

<img src="https://lh5.googleusercontent.com/BBhA_g9R8_LQHm1XTb53kqTALKBr4WYD6ri9Rm0VgHThuaFpohKpy1mglgkvW_TgKJHPrpJ08lBXLLV8dFAm3UXq3tCEbWJRWuYVCwn_k8wZy5uAROAuHrbhi-s7nQ" align="center">
<ul>
<li>Git и GitHub — системы управления исходным кодом;</li>
<li>Jenkins — сервер автоматизации для создания конвейеров CI/CD;</li>
<li>Docker — ПО для автоматизации деплоя и управления приложениями в средах с поддержкой контейнеризации;</li>
<li>Kubernetes — открытая система оркестрации контейнеров;</li>
<li>Chef, Puppet и Ansible — средства для автоматического конфигурирования и развертывания;</li>
<li>Selenium — решение для автоматизации тестирования;</li>
<li>Prometheus и Nagios — программы для мониторинга серверов;</li>
<li>Grafana — решение для сбора и анализа метрик.</li>
</ul>
Удалёнка:

<img src="https://lh6.googleusercontent.com/5Kh-W8LyQKS9ss9w52mYU2bnK2KO36unCL-Wvc6QzzHWR4qy8yjmiyob-g8pFFuWxuZTlWrdrl5Yhn0fV8oprq8TiFS7hxhNr1qVeikk7WLUFp__k39BVrADsfUJAQ" align="center">
 

<a href="https://habr.com/ru/company/vdsina/blog/494762/">https://habr.com/ru/company/vdsina/blog/494762/</a>    50 инструментов для удаленки

<ul>
<li>Asana — для управления проектами. Настроена интеграция с Jenkins.</li>
<li>Google Meet — для проведения видеовстреч.</li>
<li>Slack — для коммуникаций и различных оповещений, включая нотификации из Jenkins.</li>
<li>Atlassian Confluence — для документирования и групповой работы.</li>
</ul>
Простота – HTMLelements, retrofit, owner.aeonbits.org, google guice

Доверие – короткие атомарные тесты, моки

Контроль – grafana

<img src="https://lh3.googleusercontent.com/wiCcYjAavUI-JoDW1bSJkiNS8Nsc4m30_ib1EpQmsNK2g6xnJ8c63FNn36BSPPxBT6WNaGE4i8M0JNbCL7fAFFr7THbNZZO7zsXL1ZL6BYXiJiStqTTsGw_pD8ebOw" align="center">
Здесь нужно понять из каких уровней будет состоять этот подход к автоматизации. На каждый уровень можно свой инструмент какой-нибудь накрутить.

Первый уровень — это выбрать на чём писать, это Java, .NET, JS? Я больше с Java работала, про неё и буду говорить. Собственно, на чём построить проект — Java. Собрать его можно с помощью Maven или Gradle. Сейчас у Maven прикольные в YAML формате описания pom-ника есть, с ним удобно работать.

Дальше, выбрать чем эти тесты запускать — это JUnit или TestNG какие-нибудь. Я с JUnit 5 в последнее время работаю.

Потом выбрать уровень взаимодействия с элементами. Это Selenium, либо обёртка над ним какая-нибудь, например, Selenide. С ним можно скоратить время на написание тестов.

Дальше нужно проверять результаты тестов. Здесь очень большой выбор инструментов. Можно из JUnit 5 использовать те же самые <a href="https://junit.org/junit5/docs/5.0.1/api/org/junit/jupiter/api/Assertions.html">Assertions</a>, они сейчас в нём довольно удобно сделаны. Либо библиотека <a href="http://hamcrest.org/">Hamcrest</a>, мне она очень нравится. Либо <a href="https://joel-costigliola.github.io/assertj/">AssertJ</a> тоже удобная вещь. Когда для запуска тестов выбираете этот раннер, то нужно подумать о параллельности запуска тестов, как её будет лучше организовать. В JUnit 5 это удобно, там аннотация просто делается.

Потом уже само написание тестов, это может быть какая-нибудь BDD обёртка, тот же Cucumber. Если выбираете JUnit, то к нему ещё дополнительные вещи потребуются.

Плюс инфраструктура. Я в последнее время с Selenoid работала, мне с ним удобнее всего было.

Ещё отчёты.

<strong>— Ну отчёты это, конечно, </strong><a href="http://allure.qatools.ru/"><strong>Allure</strong></a><strong>?</strong>

<strong>Аня</strong>: Ну или <a href="https://reportportal.io/">ReportPortal</a>.
Я могу объяснить, когда лучше Allure, когда лучше ReportPortal. Allure хорошо, когда маленький проект, тогда он идеально вообще заходит. Если это какой-нибудь большой проект, где 100500 тысяч тестов или это энтерпрайзное решение, или есть понимание, что тестов должно быть очень много и они должны все в какой-нибудь отчёт складываться, то тогда хорош ReportPortal, там удобнее обрабатывать результаты именно большого количества тестов. Когда тестов немного, тогда Allure удобнее.

Есть тот самый Selenium обычный старый, Selenium или Selenium Grid, или Selenium Server — это приложение, написанное на Java, которое самое старое и самое простое с точки зрения фич. Года три назад от Selenium стандартного, от Selenium Grid отпочковался проект <a href="https://github.com/zalando/zalenium">Zalenium</a>. Он уже умеет запускать браузеры в Docker-контейнерах. Этот проект реализует полностью весь стандарт, поддерживает возможность видеозаписи, возможность хранения логов, имеет интерфейс лучше, чем у стандартного Selenium.

Мы же сделали с нуля проект под названием <a href="https://aerokube.com/selenoid/latest/">Selenoid</a>. Это тоже совершенно независимая реализация Selenium-протокола. Она написана на Go, не требуется установки Java, ничего не нужно, просто в бинарнике запускается и нужен Docker.

Кроме опенсорса мы делаем реализацию для Kubernetes, это <a href="https://aerokube.com/moon/latest/">Moon</a>. Это тоже совершенно независимая реализация, которая нужна, если у вас есть Kubernetes. Мы делали упор на то, чтобы развернуть инфраструктуру было просто легко с помощью пары команд. Людям это нравится, что ты две команды ввел и у тебя уже всё работает.

Ещё для Selenium есть всякие онлайн-платформы, если не хочется самому Selenium разворачивать. Можно пойти в облачные сервисы Они достаточно дорогие, но тем не менее они есть, пользуются довольно большой популярностью.

<strong>Аня</strong>: У меня был опыт с <a href="https://saucelabs.com/">SauceLabs</a>, там тоже довольно удобно всё. Просто указываешь в каком браузере запустить, они даже мобильное тестирование поддерживают. И запускаешь. Но они дорого стоят.

<strong>— Как, с точки зрения кроссбраузерности и мобилок, работает Selenium, и есть ли какие-то проблемы с инфраструктурой с этим? Я знаю, что некоторые тестируют определенные браузеры на мобилках. К счастью, не тестировал это руками в Selenium, не знаю, насколько это сложно всё настраивать.</strong>

<strong>Ваня</strong>: Это геморно и достаточно дорого. Цель — протестировать, что если мы откроем на каком-то телефоне наше приложение, в каком-нибудь мобильном Chrome, у нас всё работает точно так же. Естественно, мы хотим, как и в случае настольных браузеров, делать это кодом.

Первоначальная простая идея состоит в том, чтобы накупить телефонов разных моделей, положить их на стол. Есть готовые инструменты, например, <a href="http://appium.io/">Appium</a>, которые реализуют стандарт Selenium. Это тоже реализация Selenium-расширения, которая позволяет работать как раз с мобильными. Изначально это делалось как раз под ферму реальных телефонов и планшетов. Проблема в том, что просто опыт эксплуатации таких ферм телефонов показывает, что это очень дорого. Это постоянно ломается, нужно эти телефоны заменять, у них распухают батарейки, это требует довольно специальных систем, которые заряжают эти телефоны, туда нужно ставить обновления, следить, чтобы там ничего не разломалось.

Сейчас всё потихонечку двигается в сторону того, чтобы запускать это всё в эмуляторах. Существуют специальные программы — эмуляторы, которые показывают на экране обычного компьютера или сервера ровно то же самое, что видит пользователь на своём телефоне или планшете. Существуют эмуляторы для Android и для iOS. Проблема заключается в том, что, с точки зрения Android, это виртуалки, такие эмуляторы нельзя запустить на абы каком железе. Если вы хотите Android эмуляторы, вам нужно брать железные сервера, это дорого.

Если вы хотите тестировать на эмуляторах под iOS, вам нужно брать эппловское железо, то есть MacMini, MacPro, MacBook или что-то подобное, это тоже дорого. Это связано с лицензионными ограничениями компании Apple. Поэтому тестирования на мобильных в принципе возможно, понятно как делать инфраструктуру. Даже в Docker можно запускать Android, но это достаточно дорого. Если люди хотят такое делать, им нужно сильно подумать.
Основная задача тестирования на мобильных — найти баги, которые воспроизводятся только на мобильных. Существуют разные способы сделать это дешевле. Есть возможность запускать настольные браузеры вроде Chrome, в котором подсовывается юзер-агент, подсовывается нужное разрешение экрана. Решение о том, нужно ли тестировать на настоящих эмуляторах, на телефонах, нужно принимать исходя из того, можете ли вы отловить баги только на эмуляторе или на телефоне.
<strong>— Кстати, есть разные инструменты вроде Puppeteer, Playwright, которые позволяют достаточно точно эмулировать и делать кроссбраузерное тестирование в т.ч. в мобильных браузерах. Может на них уже давно все пересели или пересаживаются?</strong>

<strong>Ваня</strong>: Фронтендеры, больше никто не пересел.

<strong>Аня</strong>: Это клёвые штуки, но у них есть ограничения в плане кроссбраузерности. У Cypress для Firefox вроде выйдет обновление скоро. Ты можешь очень круто быстро писать тесты, всё удобно, но ты ограничен только Chromium-ом.

<strong>Ваня</strong>: Начнем с <a href="https://www.cypress.io/">Cypress</a>. В 2004-2005 году Selenium работал следующим образом.

Запускался браузер, в него загружалось специальное расширение, в которое запихивались команды по автоматизации браузера. Через 15 лет появились ребята, которые посмотрели на это. От этого подхода в Selenium отказались, потому что не всё можно делать при помощи расширения. Поскольку Javascript, то выполнять можно не всё в браузере, нельзя обращаться к файлам на файловой системе. В Selenium перешли на нативный подход, стали писать отдельные бинари, отдельно стоящие от браузера. Прошло 15 лет. Ребята на JavaScript сделали похожим образом инструмент.

Puppeteer ровно то же самое. Puppeteer это Google Chrome, Chromium, в котором реализован специальный протокол для работы с этой отладочной панели. В Chrome есть отладочная панель, чтобы там можно было сообщения в консоли смотреть, сетевые запросы и так далее.

<strong>— Developer tools очень крутая, конечно.</strong>

<strong>Ваня</strong>: Да-да, для разработчика удобная. Как выяснилось, эта штука взаимодействует с браузером по специальному протоколу. Основная идея заключается в том, чтобы в этот протокол не руками мышкой кликать, а чтобы можно было точно так же, как в Selenium, команды слать кодом. Ребята просто написали Javascript-библиотеку, которая реализует протокол.

<strong>Аня</strong>: Эти инструменты, мне кажется, могут хорошо подходить для компонентного тестирования, которое бы сами фронтендеры и покрывали. Я знаю такие кейсы применения, они прямо очень хорошо заходили.

<i><strong>Популярные системы управления тестированием</strong></i>

<strong>Зачем она нужна?</strong>
Решить задачу создания единой системы для работы со всей документацией проекта можно несколькими способами:

<ul>
<li>Самый дешёвый способ — не заморачиваться и выбрать Google Docs для матрицы трассируемости, а дефекты вести в open-source баг-трекере.</li>
<li>Другой способ — использовать одну из популярных TMS'ок, интегрированную с баг-трекером компании.</li>
<li>Next-level способ — выбрать Test Management System, исходя из специфики проектов, объемов задач, типов документации и используемых видов тестирования.</li>
</ul>
Очень важно подойти к вопросу выбора TMS ответственно, ведь для компании, цена ошибки может оказаться высокой.

<ul>
<li>Test Link</li>
<li>Test IT</li>
<li>Zephyr</li>
<li>qTest</li>
<li>PractiTest</li>
<li>TestLodge</li>
<li>TestRail</li>
<li>Qase</li>
<li>Tematoo</li>
<li>Test Collab</li>
<li>HP ALM</li>
<li>Testuff</li>
<li>XQual</li>
<li>Xray</li>
</ul>
<i></i><i><strong>1. TestLink</strong></i>
Один из немногих open-source инструментов управления тестированием, который доступен на рынке. Это веб-инструмент с типичными функциями, такими как управление требованиями, создание и сопровождение тест сьютов, прогон тестов, отслеживание ошибок, интеграция с известными баг-трекинговыми системами.

Для отслеживания прогресса проекта доступны отчёты и диаграммы, а дополнительные функции включают тэгирование ключевыми словами, указание требований и журнал событий.
Код проекта часто обновляется и дополняется.

<strong>Возможности:</strong>

<ul>
<li>Управление требованиями</li>
<li>Спецификация — определение тест кейсов путём группировки в разные наборы тестов</li>
<li>Назначение выполнения тест сьютов на уровне сборки</li>
<li>Централизованное управление пользователями и ролями</li>
<li>Кастомизация настраиваемых пользователем полей</li>
</ul>
<a href="https://github.com/TestLinkOpenSourceTRMS">Ссылка на код (GitHub)
</a><a href="https://sourceforge.net/projects/testlink/">Ссылка на скачивание

</a>
<img src="https://lh6.googleusercontent.com/rX8wP3WAAgOmZNLjicNInLWe5c3XqkastkL2Gba0LoKmjALu4IqN8r0L6qO3E5rh4RzBlgBWxOdwR8yfIcIFG6wzHJF8g30YL2NOwMYSb0RjJkhSsqx1rDQmtFXsQg" align="center">
<i><strong></strong></i>

<i><strong>2. Test IT</strong></i>

Test IT — TMS, которую создают тестировщики для тестировщиков. Этот инструмент отличает продуманный и понятный интерфейс. Внутри системы можно создавать проекты и вести для каждого структурированную библиотеку тестовых случаев и чек-листов, часто повторяющиеся операции выделяются в общие шаги. Инструмент гибкий — в каждом проекте создаются дополнительные пользовательские атрибуты, распределяются роли и права, что упрощает настройку TMS под процессы вашей компании. Test IT помогает руководителям групп тестирования равномерно распределять нагрузку между тестировщиками и контролировать исполнение работ с помощью пользовательских запросов и отчётов.

Разработчики приложения уделяют большое внимание автоматизированному тестированию, каждый тестовый случай в библиотеке тестов можно интегрировать с автотестами по API. Правильно настроенная интеграция с автотестами позволяет следить за прогонами и их результатами прямо из TMS в режиме реального времени. Вы сможете видеть какие автоматические тесты в процессе выполнения, анализировать их результаты и просматривать исходный код прямо из Test IT.

Приложение активно развивается, в ближайшем будущем заявлено много полезных фич.

<strong>Возможности:</strong>

<ul>
<li>Управление тест-планами, тест-кейсами и чек-листами</li>
<li>Общие шаги для повторяющихся действий</li>
<li>Автоматическое распределение тестов на QA инженеров</li>
<li>Интеграция автоматических тестов с помощью API</li>
<li>Аналитика как по автоматическим, так и по ручным тестам</li>
<li>Ролевая модель и персонализация</li>
<li>Геймификация</li>
<li>Двусторонняя интеграция с JIRA</li>
<li>Импорт из других систем управления тестированием</li>
</ul>
<strong>Бесплатная пробная версия:</strong> Открытая демо-версия на сайте
<a href="https://testit.software/downloads">Ссылка на скачивание

</a>
<img src="https://lh3.googleusercontent.com/-ogAEAjp5RyzFiyuW26JM5P5cCX09bDrKv0dHbM9NaRZFydtKS2us3SDFnCK4-aGVRO0Mz0opFA8_RZmsiXehQYvyydikZfLhqkOLQN_YOOb6ypPl4EIZbYQdprzxg" align="center">
<i><strong>3. Zephyr</strong></i>

Zephyr — это плагин для всем известной JIRA, который интегрирует тестирование в проектный цикл, позволяя вам отслеживать качество программного обеспечения и принимать решения в стиле go / no-go. Тест кейсы могут создаваться, выполняться и трекаться так же, как и любые другие задачи в JIRA. Для более оптимальной фиксации процесса тестирования есть интеграция с инструментами управления качеством, автоматизации, непрерывной интеграции и аналитики.
Кроме того, у продукта быстро отвечающая тех поддержка.

<strong>Возможности:</strong>

<ul>
<li>Ссылка на user stories, задачи, требования, дефекты</li>
<li>Конфигурации деплоя: в облаке, на сервере, в дата-центре</li>
<li>Расширенная информация на дашбордах аналитики и DevOps</li>
<li>Интеграция с JIRA, Confluence, Selenium, Jenkins и Bamboo</li>
</ul>
<strong>Бесплатная пробная версия:</strong> 30 дней
<a href="https://www.getzephyr.com/products">Ссылка на скачивание

</a>
<img src="https://lh6.googleusercontent.com/WpdVdeYlIsEyBx6-ImtDhXi3wilWgKGHZ9lTHs9-uKNbmS2XkppkiSVO5HJpMMUJalB8mkkLM73i9a0ca0fUuSJpaXh5JEBg-pvSib67URSROBHAtFIB6jxTe-jIQg" align="center">
<i><strong></strong></i>

<i><strong>4. qTest</strong></i>

Инструмент полезный не только тестировщикам, но и всей команде. Интерфейс qTest нативно понятен, мануалы просты в освоении. Это позволяет быстро и эффективно создавать, организовывать и управлять тест кейсами.

Разработчики нескромно заявляют, что их инструмент управления тестами №1
Согласно анализу рынка, qTest является одним из самых быстрорастущих решений для управления тестированием среди команд Agile Development.

<strong>Возможности:</strong>

<ul>
<li>Планирование тестов</li>
<li>Создание и управление требованиями</li>
<li>Интуитивный drag-n-drop интерфейс</li>
<li>Комплексная матрица трассируемости</li>
<li>Наглядные отчёты с подробными графиками</li>
<li>Интеграция со сторонними инструментами баг-трекинга</li>
<li>Детальный контроль доступа пользователей</li>
<li>Облачный инструмент интеграции с JIRA</li>
</ul>
<strong>Бесплатная пробная версия:</strong> 30 дней
<a href="https://www.qasymphony.com/software-testing-tools/qtest-manager/test-case-management/">Ссылка на скачивание

</a>
<img src="https://lh5.googleusercontent.com/x3GmUqfpfVRCgNTgBvuRNvcfDtvRlsH1vm8qHPJTgv3SxgnXdGpH-KDTVDpK6ieRzg7PIOyzF_y5dfQDkmfoWkqcEWiqPNrcILeXY_tp0LuPY6ZJnrxX73k70EZTwQ" align="center">
<i><strong></strong></i>

<i><strong>5. PractiTest</strong></i>

PractiTest — это комплексное средство управления тестами. Оно обеспечивает полную наглядность процесса тестирования и более глубокое понимание результатов тестирования. Этот инструмент поможет организовать тест сьюты в соответствии с вашими циклами и спринтами. Тестовые наборы можно формировать по различным критериям, таким как компоненты, версии или типы. Тул заточен на Agile тестирование, регрессионное тестирование, тестирование микросервисов и DevOps.

А в тех поддержке работают обученные QA сотрудники, которые могут быстро понять вашу проблему.

<strong>Возможности:</strong>

<ul>
<li>Лёгкое добавление тестов новых фич в регрессионное тестирование</li>
<li>Группировка тестов на основе микросервисов, которые они охватывают, даже кросс-сервисные</li>
<li>Различное отображение информации для разных групп пользователей</li>
<li>Дашборды в реальном времени показывают состояние тестов, прогонов на этапах разработки и при деплое на продакшн</li>
<li>Интеграция с JIRA, Redmine, Jenkins, GitLab и Slack</li>
</ul>
<strong>Бесплатная пробная версия:</strong> 14 дней
<a href="https://landing.practitest.com/free-trial/">Ссылка на скачивание

</a>
<img src="https://lh3.googleusercontent.com/1j1EooZOR9cUPDDWO7V88KTSy74J2W1o6fQPOwXGl2TG6PRNifKjIWKrGRR581aSO9k2dGsiOHM55JOMSxcyA6DFgS0pBhO0ZhIsTSAgH83ph_VfU7TSMsqXcS47sQ" align="center">
<i><strong></strong></i>

<i><strong>6. TestLodge</strong></i>
В нём есть самый необходимый минимум, который требуется для управления тестированием: тест планы, требования, тест кейсы и сьюты, и тестовые прогоны. Тул можно интегрировать с существующими баг-трекерами, что позволяет автоматически создавать отчёты о дефектах и заводить задачи.

<strong>Возможности:</strong>

<ul>
<li>Базовый набор создания, редактирования тест плана и тест сьютов</li>
<li>Нативный интерфейс</li>
<li>Интеграция с JIRA, Redmine, Trello, Asana, GitHub и YouTrack</li>
</ul>
<strong>Бесплатная пробная версия:</strong> 30 дней
<a href="https://www.testlodge.com/signup?plan_name=plus">Ссылка на скачивание

</a>
<img src="https://lh6.googleusercontent.com/uIduFg98gWLDqQuObUOqETD32VwXxFE2j8b7iei5becZlRCzl1G8uQsdZlTFbhGGmbYJXvd0w4uouqvb8IapNd5VekD0rUFAS2HbTFZPJJV5S9Z4Lb9nZIzLJNd-FA" align="center">
<i><strong></strong></i>

<i><strong>7. TestRail</strong></i>

Это программное обеспечение удобно как для команд QA, так и для разработки. План тестирования можно выстроить как по сценарию гибкой методологии, так и для более традиционного подхода. Инструмент позволяет получить представление о ходе тестирования в реальном времени.

<strong>Возможности:</strong>

<ul>
<li>Отслеживание состояния и результатов отдельного теста</li>
<li>Сравнение результатов нескольких тестов, конфигураций и этапов</li>
<li>Отслеживание рабочей нагрузки команды для корректировки задач и ресурсов</li>
<li>Развёрнутые отчёты и метрики</li>
<li>Широкие возможности настройки, облачные или локальные варианты установки</li>
<li>Интеграция с JIRA, Redmine, YouTrack, GitHub, Jenkins, Selenium и Visual Studio</li>
<li>Удобный REST API</li>
</ul>
<strong>Бесплатная пробная версия:</strong> 30 дней
<a href="https://secure.gurock.com/customers/testrail/trial/">Ссылка на скачивание

</a>
<img src="https://lh4.googleusercontent.com/bMLpd90j68qmFHm56we8jkM498BnchgYrVmhgCdCiqT9uc0ZitnhKp7NxPUw-JgDryKS4pmUaymIuAPgOg00ZuOl-CzbfY0fU6h6IhB0ytQov6SfhnJn1EPPVMY1Yg" align="center">
<i><strong></strong></i>

<i><strong>8. Qase</strong></i>

Qase это недавно появившийся продукт, который можно нормально использовать в работе. Облачная TMS, которая поможет вашей команде повысить производительность и организовать удобный флоу тестирования программного обеспечения.

<strong>Возможности:</strong>

<ul>
<li>Тестовый репозиторий: выстраивание тестов в логические группы</li>
<li>Составление шагов для кейсов, установка приоритета и серьёзности</li>
<li>Запуск тестовых прогоны с трекингом времени по каждому тест кейсу</li>
<li>Хранение документации по проекту</li>
<li>Автоматическое заведение дефектов в интегрированные трекеры</li>
<li>Интеграция с JIRA, Redmine, YouTrack и Slack</li>
<li>Объединение результатов автотестов с REST API</li>
</ul>
<strong>Бесплатно для небольших компаний</strong>
<a href="https://app.qase.io/signup">Ссылка на скачивание

</a>
<img src="https://lh5.googleusercontent.com/vZdEyDAWGmJboj7jfSc-IWfGIVyRxPX7xr7wt2iNvaLoi7eoq9YxFZJGXYsY2rBgO1Y9uvi224PN35waSZ8TymwCfzHMa_uCNwiFjVJTJpUBxa6t4oG9-mM0j2pVbA" align="center">
<i><strong></strong></i>

<i><strong>9. Tematoo</strong></i>

Эта облачная TMS от TestLink не так разрекламирована, но не уступает по своей функциональности более дорогим аналогам. Инструмент предоставляет лаконичную инфраструктуру, позволяя быстро приступить к тестированию продукта. А бесплатный план поддержки небольших команд позволяет проводить пилотные реализации проекта бесплатно. Tematoo может быть интегрирован со многими баг-трекерами, даже облачными.

<strong>Возможности:</strong>

<ul>
<li>Формирование тест сьютов по билдам и типам</li>
<li>Описание тест кейса по шагам, с возможностью прикрепить скриншот</li>
<li>Статус отдельных тестов, наборов и общий статус сборки</li>
<li>Аналитические отчёты и общий метрики по тест плану</li>
<li>Для платного плана: свой баг-трекер</li>
</ul>
<strong>Бесплатно:</strong> для команды из 1-5 человек
<a href="http://tematoo.com/buynow/?package=starter">Ссылка на скачивание

</a>
<img src="https://lh4.googleusercontent.com/SGUcFFQLJ94Gi2CNjTe-ffcw90AVVlvEQzQ0ucpII7LAiqErn1rasUw_AeJLELV4YcpZJ0SWTQ7V2tDLx5mP-EatDQGZIWd_4OlqwzTAHNDepCuio4oK4no_dg4z5A" align="center">
<i><strong></strong></i>

<i><strong>10. Test Collab</strong></i>

Это сервис с полезным набором функций, который необходим для быстрого старта использования инструмента. Плюс, немного приятных бонусов: удобный интерфейс, кастомизация фильтров и полей, time-трекер для каждого члена команды, и внутрисистемное общение.

Test Collab можно настроить в облаке или в вашей инфраструктуре, тут всё достаточно гибко.

<strong>Возможности:</strong>

<ul>
<li>Группировка тест кейсов по этапам или билдам</li>
<li>Управление требованиями</li>
<li>Переиспользование тестов</li>
<li>Настройка спринтов</li>
<li>Отчёты по результатам тестов</li>
<li>Комментирование тест кейсов</li>
<li>Интеграция с JIRA, Redmine, Bugzilla, Asana, Trello, YouTrack, GitHub

</li>
</ul>
<strong>Бесплатно:</strong> 200 тест кейсов, 400 выполненных прогонов
<strong>Бесплатная пробная версия:</strong> 14 дней
<a href="https://testcollab.com/trial/">Ссылка на скачивание

</a>
<img src="https://lh4.googleusercontent.com/A_sfI65mbonUNRqVTHvjilTz7ix2weYQHow_noGschdTjztmIk98rxnJ3t5bJBzp3G9dyG2DTx5FKjrr5hIVouLE5v4ErsxPvtF3rT8n0w5aR5gcikwxiUnPLCl2rA" align="center">
<i><strong></strong></i>

<i><strong>11. HP ALM</strong></i>

HP ALM — долгожитель среди систем управления жизненным циклом продукта, и его тестировании в том числе. Инструмент позволяет осуществлять планирование, создание, тестирование и контроль на всех этапах разработки. Сложен в первоначальном освоении, но незаменим для компании крупной руки, где особое внимание уделяется деталям производства.
Именно потому что продукт уже обкатан, в интернете есть большое множество мануалов и видеогайдов по настройке и использованию.

<strong>Возможности:</strong>

<ul>
<li>Общий доступ к библиотекам требований и ресурсов</li>
<li>Подробные сведения о коде, тестировании, управлении рисками и их оценке, а также о соответствии требованиям</li>
<li>Быстрый доступ к показателям, например к данным о неустранённых дефектах</li>
<li>Быстрая настройка лабораторной среды для устранения ошибок конфигурации в средах Agile</li>
<li>Создание требований и отслеживание их выполнения на всех этапах жизненного цикла приложения</li>
<li>Аналитика на любой вкус и цвет: гибко настраиваемые отчёты</li>
<li>Интеграция с 50+ инструментами</li>
</ul>
<strong>Бесплатная пробная версия:</strong> 60 дней
<a href="https://ssl.www8.hp.com/ru/ru/ssl/dlc/secure_software.html?prodNumber=TC096EVE&siebelid=23810&lang=ru&cc=ru&resouce_type=Trial%2520Software&cpt_resource_type=hp.resource_type.software_trial.label&sectionid=software&subbu=TSG.Software&simpletitle=try%2520now%252Fhp%2520ALM%2520product%2520page&parentUrl=https%253A%252F%252Fwww.google.com%252F">Ссылка на скачивание

</a>
<img src="https://lh5.googleusercontent.com/dsN4TOcFLBGahRKzksQW4ek0GCHXaUt6Aar2T7n5mNW-ZRN1J35b8YcJJHj98z59WkhY2-Knw8ZhXYmH8w1Vz8_1HefNjRUugUn1euVng0Eev2LcWX2QPoGihmAMHg" align="center">
<i><strong></strong></i>

<i><strong>12. Testuff</strong></i>

Testuff — это мощная веб-платформа управления тестированием, которая позволяет легко проектировать, выполнять и управлять неограниченным количеством тестов. Тул можно настроить под любой формат тестирования: от популярной гибкой методологии и TDD, до White-Box или Black-Box; Top-Down или Bottom-Up.

Здесь есть и оптимизированная очередь управления задачами для каждого тестировщика с применением тайм-менеджмента. И организация тестов по проектам, веткам кода и типичным тестовым наборам. Помимо бонуса экспорта в HTML/Excel, есть маленькие плюшки в виде встроенного тула создания скриншотов и видео с отображением указателя и нажимаемых клавиш.

<strong>Возможности:</strong>

<ul>
<li>Два доступных клиента — Web и Desktop</li>
<li>Планирование цикла тестирования с использованием нескольких тестовых окружений</li>
<li>Разграничение по ролям пользователей</li>
<li>Встроенный захват экрана в виде скриншота или видео</li>
<li>Подключение результатов автоматизированных тестов по API</li>
<li>Интеграция с JIRA, Trello, Redmine, Bugzilla, YouTrack, Selenium, GitHub, Visual Studio

</li>
</ul>
<strong>Бесплатная пробная версия:</strong> 30 дней
<a href="https://app.testuff.com/%23">Ссылка на скачивание

</a>
<img src="https://lh5.googleusercontent.com/A8rAW88nv6tiK7ZXYPPvMgcDThL-EKdY3dofjgKpKs9myPXwIh2OlFHXquz4jlo74UDwf4aGPGsDV2wTQE9xzPfAvDuLOczCIbsz1eoHQshNTsRsiVGIruTP1uMRqA" align="center">
<i><strong></strong></i>

<i><strong>13. XQual</strong></i>

XStudio от XQual осчастливит продвинутого тестировщика, который хочет подвергнуть свой продукт максимальному количеству испытаний. С помощью этого инструмента можно управлять не только своими релизами, требованиями, рисками, спецификациями, тестами, кампаниями и багами. Он может быть интегрирован со всеми платформами непрерывной интеграции и может выполнять любой вид тестирования.

<strong>Возможности:</strong>

<ul>
<li>Расширенная настройка шагов тест кейса</li>
<li>Переиспользование тестов</li>
<li>Матрица трассируемости</li>
<li>Настройка тестовой лаборатории: hardware, software, тестовое окружение</li>
<li>Продвинутое логирование действий (даже удалённых тестов)</li>
<li>Настраиваемая аналитика</li>
<li>Встроенный захват экрана</li>
<li>Интеграция с JIRA, Redmine, MySQL, Oracle, Apache, Skype</li>
<li>Интеграция с 5 различными интерфейсами для ручного тестирования</li>
<li>Интеграция с почти 70 тулами автоматизации: Selenium, QTP / UFT, JMeter, Ranorex, TestComplete, JUnit, NUnit, TestPartner, Sahi, NeoLoad, QF-Test, RobotFramework, Sikuli, SoapUi, Squish, TestNg, TestOptimal и многие другие

</li>
</ul>
<strong>Бесплатно:</strong> для команды из 4-10 человек, 200 тестов
<a href="https://www.xqual.com/support/download.html">Ссылка на скачивание
</a>
<img src="https://lh5.googleusercontent.com/kWyxl7mAugoAaqj4H0zGK4VyHiYQxW3x9IOlYS2k1O6eqJOgoRCtPU_qdLFlCO3_nbBdPFOfXtEa-MXbr8JBzujNUFnjVF0nYgQqoYGnrq53gzp7KXBZ60Jr2Q9zQA" align="center">
<i><strong></strong></i>

<i><strong>14. Xray</strong></i>

Xray — еще один плагин для тест менеджмента внутри Jira. В нем присутствует все, что нужно, чтобы дополнить существующий фунционал Jira на этапах написания, организации, планирования и запуска тестов. Тест кейсы, тест планы, сэты, прогоны и прекондишны являются нативными задачами Jira, тем самым давая пользователям возможность использовать продукты его деятельности с другими аддонами прямо с коробки. Прекондишны — выделены в отдельный тип задач, который позволяет указать предварительные условия для ваших тестов и переиспользовать их позже, присоединяя к тесткейсам — это очень полезно во многих случаях, когда вам нужно начать с того же самого списка действий. Вместе с тем, в плагине присутствует возмножность множественного запуска тестов, что существенно упрощает процесс дальнейшего анализа состояния тестовых объектов по версии, тест плану и среде выполнения; а продвинутая система репортинга позволяет просматривать тестовое покрытие требований с помощью интерактивных диаграмм. У Xray детальная <a href="https://docs.getxray.app/site/xray">документация</a>, быстро отвечающая служба поддержки, частые апдейты (с интервалом в 2-3 месяца) и собственная <a href="https://academy.getxray.app/">платформа для обучения</a>.

Помимо основного продукта, еще доступны мобильные приложения XRay для <a href="https://apps.apple.com/pt/app/xray-test-management-app/id1455875584#?platform=iphone">iOS</a> и <a href="https://play.google.com/store/apps/details?id=com.xpandit.xrayapp">Android</a>, которые позволяют запускать тесты, проверять ход тестирования и визуализировать отчеты. Также доступно десктопное приложение Xray Exploratory App, которое существенно упрощает репортинг. В конце сессии приложение автоматически прикрепляет PDF-файл к вашему тесту, включая все дефекты.

<strong>Возможности:</strong>

<ul>
<li>Использование нативных типов задач Jira и интеграция с другими аддонами прямо с коробки</li>
<li>Конфигурации деплоя: в облаке, на сервере/дата-центре</li>
<li>Продвинутая система репортинга</li>
<li>Импорт тестов из других систем управления тестированием</li>
<li>Встроеный REST API</li>
<li>Интеграция с CI & DevOps тулами</li>
<li>Поддержка написания BDD сценариев внутри Jira</li>
<li>Поддержка фреймворков на основе Gherkin</li>
<li>Встроенная интеграция с фреймворками автоматизации тестирования</li>
</ul>
<strong>Бесплатная пробная версия:</strong>
<a href="https://marketplace.atlassian.com/apps/1211769/xray-test-management-for-jira?hosting=server&tab=overview">Ссылка на скачивание</a>
<img src="https://marketplace-cdn.atlassian.com/files/images/677a478e-6a2c-44e8-8885-34820032473f.png" align="center">
Линтеры изучают код, помогают найти ошибки и сделать его стилистически согласованным со стандартами и кодом, который пишут разработчики в вашей команде. Самые распространенные из них — Pylint и Flake8

<i><strong>Charles</strong></i> — инструмент для мониторинга HTTP/HTTPS трафика. Программа работает как прокси-сервер между мобильным приложением (в нашем случае) и сервером этого приложения. Charles записывает и сохраняет все запросы, которые проходят через подключенный к нему телефон и позволяет их редактировать.

<img src="https://lh4.googleusercontent.com/uxmwB2d6ezkE2I3olFEUU-M9zHd_7iHRRt9PKia0zysiLPfYYrT6X-G0QH4aAjxL48R5E3Ywoydoa5fA3pSphE1ipWbWkB0c1PJS-v7XyZ10Rb1qNzIRlRgyDcGCKw" align="center">
Для тестирования мобильных приложений, работающих с удаленными серверами, QA-инженеру приходится держать под рукой множество разных тестовых аккаунтов, логов, запросов и ответов. Реальность такова, что не всегда удается договориться о предоставлении нужных тестовых данных в срок. Чаще всего серверные разработчики будут незнакомыми вам людьми по ту сторону Скайпа. В таких ситуациях приходится своими руками подменять ответ сервера перед его передачей в приложение.

Чтобы редактировать выдачу сервера и воспроизводить сложные тестовые сценарии в QA Redmadrobot, мы используем <a href="http://www.charlesproxy.com/"><strong>Charles</strong></a>.

Charles является незаменимым инструментом в арсенале QA-инженеров Redmadrobot. С его помощью можно создавать любые необходимые тестовые данные, как реальные, так и невозможные (если верить API-спецификациям). Такие возможности расширяют границы тестирования черного ящика и позволяют наблюдать все основные взаимодействия вашего МП и его серверов. Тестирование на таком уровне позволяет находить более сложные дефекты и значительно повышает общее качество приложения.

<a href="https://habr.com/ru/company/redmadrobot/blog/269109/">https://habr.com/ru/company/redmadrobot/blog/269109/</a>

Софт такого рода — отличная вещь для дебага веб-запросов. Но Charles — не мой выбор. Мне больше понравился бесплатный аналог <a href="http://www.telerik.com/fiddler">Fiddler</a>.

Работал с ним хоть и не очень долго, но в нем есть все что нужно — есть те же фильтры, можно подменять ответы, поддерживает HTTPS, может перехватить запрос и ответить на него, не обращаясь к реальному серверу. На Linux работает <a href="http://fiddler.wikidot.com/mono">под Mono</a>, но с периодическими вылетами и мелкими глюками.

<strong>Redis</strong> (от <a href="https://ru.wikipedia.org/wiki/%D0%90%D0%BD%D0%B3%D0%BB%D0%B8%D0%B9%D1%81%D0%BA%D0%B8%D0%B9_%D1%8F%D0%B7%D1%8B%D0%BA">англ.</a> <i>remote dictionary server</i>) — <a href="https://ru.wikipedia.org/wiki/%D0%A0%D0%B5%D0%B7%D0%B8%D0%B4%D0%B5%D0%BD%D1%82%D0%BD%D0%B0%D1%8F_%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0_%D1%83%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D1%8F_%D0%B1%D0%B0%D0%B7%D0%B0%D0%BC%D0%B8_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85">резидентная система управления базами данных</a> класса <a href="https://ru.wikipedia.org/wiki/NoSQL">NoSQL</a> с <a href="https://ru.wikipedia.org/wiki/%D0%9E%D1%82%D0%BA%D1%80%D1%8B%D1%82%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D0%B5">открытым исходным кодом</a>, работающая со структурами данных типа «<a href="https://ru.wikipedia.org/wiki/%D0%9A%D0%BB%D1%8E%D1%87_%E2%80%94_%D0%B7%D0%BD%D0%B0%D1%87%D0%B5%D0%BD%D0%B8%D0%B5">ключ — значение</a>». Используется как для <a href="https://ru.wikipedia.org/wiki/%D0%91%D0%B0%D0%B7%D0%B0_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85">баз данных</a>, так и для реализации <a href="https://ru.wikipedia.org/wiki/%D0%9A%D1%8D%D1%88">кэшей</a>, <a href="https://ru.wikipedia.org/w/index.php?title=%D0%91%D1%80%D0%BE%D0%BA%D0%B5%D1%80_%D1%81%D0%BE%D0%BE%D0%B1%D1%89%D0%B5%D0%BD%D0%B8%D0%B9&action=edit&redlink=1">брокеров сообщений</a><a href="https://en.wikipedia.org/wiki/message_broker"><sup>[en]</sup></a>.

Ориентирована на достижение максимальной производительности на <a href="https://ru.wikipedia.org/wiki/%D0%90%D1%82%D0%BE%D0%BC%D0%B0%D1%80%D0%BD%D0%B0%D1%8F_%D0%BE%D0%BF%D0%B5%D1%80%D0%B0%D1%86%D0%B8%D1%8F">атомарных</a> операциях (заявляется о приблизительно 100 тыс. SET- и GET-запросов в секунду на Linux-сервере начального уровня<a href="https://ru.wikipedia.org/wiki/Redis#cite_note-5"><sup>[5]</sup></a>). Написана на <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B8_(%D1%8F%D0%B7%D1%8B%D0%BA_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F)">Си</a>, интерфейсы доступа созданы для большинства основных языков программирования.

RabbitMQ — диспетчер обмена сообщениями между приложениями

<strong>Zabbix</strong> — <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B2%D0%BE%D0%B1%D0%BE%D0%B4%D0%BD%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D0%B5">свободная</a> система <a href="https://ru.wikipedia.org/wiki/%D0%9C%D0%BE%D0%BD%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D0%BD%D0%B3">мониторинга</a> и отслеживания статусов разнообразных сервисов <a href="https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BC%D0%BF%D1%8C%D1%8E%D1%82%D0%B5%D1%80%D0%BD%D0%B0%D1%8F_%D1%81%D0%B5%D1%82%D1%8C">компьютерной сети</a>, <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D1%80%D0%B2%D0%B5%D1%80_(%D0%B0%D0%BF%D0%BF%D0%B0%D1%80%D0%B0%D1%82%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D0%B5)">серверов</a> и <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D1%82%D0%B5%D0%B2%D0%BE%D0%B5_%D0%BE%D0%B1%D0%BE%D1%80%D1%83%D0%B4%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5">сетевого оборудования</a>, написанная <a href="https://www.linkedin.com/in/vadim-zubovich-16846b62/">Вадимом Зубовичем (динозавр)</a>.

Для хранения данных используется <a href="https://ru.wikipedia.org/wiki/MySQL">MySQL</a>, <a href="https://ru.wikipedia.org/wiki/PostgreSQL">PostgreSQL</a>, <a href="https://ru.wikipedia.org/wiki/SQLite">SQLite</a> или <a href="https://ru.wikipedia.org/wiki/Oracle_Database">Oracle Database</a>, веб-интерфейс написан на <a href="https://ru.wikipedia.org/wiki/PHP">PHP</a>. Поддерживает несколько видов мониторинга:

<ul>
<li><i>Simple checks</i> — может проверять доступность и реакцию стандартных сервисов, таких как SMTP или HTTP, без установки какого-либо программного обеспечения на наблюдаемом хосте.</li>
<li><i>Zabbix agent</i> — может быть установлен на <a href="https://ru.wikipedia.org/wiki/UNIX">UNIX-подобных</a> или <a href="https://ru.wikipedia.org/wiki/Windows">Windows</a>-хостах для получения данных о нагрузке <a href="https://ru.wikipedia.org/wiki/CPU">процессора</a>, использования сети, дисковом пространстве и так далее.</li>
<li><i>External check</i> — выполнение внешних программ, также поддерживается мониторинг через <a href="https://ru.wikipedia.org/wiki/Simple_Network_Management_Protocol">SNMP</a>.</li>
</ul>
В любой сети, где есть больше, чем один сервер, очень полезно бывает иметь перед глазами полную картину происходящего. В крупных сетях, где количество хостов переваливает за несколько десятков, следить за каждым в отдельности — непосильная задача для администраторов. Для облегчения задачи наблюдения применяются системы мониторинга, и я расскажу об одной из них, которой на Хабре не посвящено ни одной полноценной статьи.

И так, встречайте: <a href="http://www.zabbix.com/">Zabbix</a>. Система состоит из нескольких частей, и при большой нагрузке и наблюдении за очень большим количеством хостов позволяет разнести эти части на несколько раздельных машин.

Zabbix состоит из

<ul>
<li>собственно сервера мониторинга, который выполняет периодическое получение данных, обработку, анализ и запуск скриптов оповещения</li>
<li>базы данных (MySQL, PostgreSQL, SQLite или Oracle)</li>
<li>веб-интерфейса на PHP</li>
<li>агента — демона, который запускается на отслеживаемых объектах и предоставляет данные серверу. Агент опционален, мониторинг можно производить не только с помощью него, но и по SNMP (версий 1, 2, 3), запуском внешних скриптов, выдающих данные, и несколько видов предопределенных встроенных проверок, таких как ping, запрос по http, ssh, ftp и другим протоколам, а так же замер времени ответа этих сервисов.</li>
</ul>
<strong>Bugzilla</strong> (Багзилла) — <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B2%D0%BE%D0%B1%D0%BE%D0%B4%D0%BD%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D0%B5">свободная</a> <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0_%D0%BE%D1%82%D1%81%D0%BB%D0%B5%D0%B6%D0%B8%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F_%D0%BE%D1%88%D0%B8%D0%B1%D0%BE%D0%BA">система отслеживания ошибок</a> (багтрекинга) с <a href="https://ru.wikipedia.org/wiki/%D0%92%D0%B5%D0%B1-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5">веб-интерфейсом</a>.

<strong>Redmine</strong> <a href="https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D0%B6%D0%B4%D1%83%D0%BD%D0%B0%D1%80%D0%BE%D0%B4%D0%BD%D1%8B%D0%B9_%D1%84%D0%BE%D0%BD%D0%B5%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B0%D0%BB%D1%84%D0%B0%D0%B2%D0%B8%D1%82">[ɹɛdˈmɑɪn]</a> — <a href="https://ru.wikipedia.org/wiki/%D0%9E%D1%82%D0%BA%D1%80%D1%8B%D1%82%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D0%B5">открытое</a> серверное <a href="https://ru.wikipedia.org/wiki/%D0%92%D0%B5%D0%B1-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B5">веб-приложение</a> для <a href="https://ru.wikipedia.org/wiki/%D0%A3%D0%BF%D1%80%D0%B0%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5_%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82%D0%B0%D0%BC%D0%B8">управления проектами</a> и задачами (в том числе для <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0_%D0%BE%D1%82%D1%81%D0%BB%D0%B5%D0%B6%D0%B8%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F_%D0%BE%D1%88%D0%B8%D0%B1%D0%BE%D0%BA">отслеживания ошибок</a>). 

<strong>Confluence</strong> — тиражируемая <a href="https://ru.wikipedia.org/wiki/%D0%92%D0%B8%D0%BA%D0%B8">вики</a>-система для внутреннего использования организациями с целью создания единой базы знаний. Написана на <a href="https://ru.wikipedia.org/wiki/Java">Java</a>. Разрабатывается <a href="https://ru.wikipedia.org/wiki/Atlassian">Atlassian</a>.

<a href="https://aerokube.com/selenoid/latest/">Selenoid</a> – это сервер, запускающий изолированные браузеры в Docker контейнерах.

Преимущества использования Selenoid:

<ul>
<li>Единая среда для параллельного запуска автотестов</li>
<li>Изолированное окружение: каждый браузер запускается в отдельном контейнере, что позволяет полностью изолировать окружение нашего браузера</li>
<li>Масштабируемость: окружение никак не влияет на качественное и непрерывное проведение тестов</li>
<li>Потребление и утилизация ресурсов: Selenoid позволяет поддерживать высокую нагрузку без дополнительных ресурсозатрат; кроме того, он утилизирует все неактивные контейнеры после завершения самой его сессии, тем самым постоянно поддерживая нужно количество свободной памяти</li>
<li>Установка: не занимает много времени и осуществляется, по сути, при помощи одной команды</li>
<li>Одновременная поддержка нескольких версий одного браузера: данная опция доступна только у Selenoid, для этого необходимо создать несколько контейнеров с необходимыми браузерами</li>
<li>Фокус: операционная система работает таким образом, что в фокусе может быть только одно окно. При запуске нескольких браузеров на одной машине, окна могут начать конкурировать за фокус. У Selenoid такой проблемы нет, поскольку каждый тест запускается в отдельном контейнере</li>
<li>Пользовательский интерфейс и логи: Selenoid позволяет быстро получить доступ к имеющимся журналам. Помимо этого есть возможность интеграции с <a href="https://www.elastic.co/what-is/elk-stack">ELK</a> стэком для более быстрого сбора и анализа текущих файлов.</li>
</ul>
<strong>Selenoid UI</strong> – графическая оболочка, через которую мы можем посмотреть ход выполнения наших тестов в реальном времени, видеозаписи выполнения сценариев, примеры конфигурационных файлов, собрать какую-то статистику и т.д.

<h4><i>Дополнительные возможности Selenoid</i></h4>
<ul>
<li>Хранение данных в оперативной памяти: в Selenoid все временные памяти хранятся в <i>Tmpfs</i> – временном файловом хранилище, которое позволяет хранить файлы в оперативной памяти. Доступ к ОЗУ, как известно, осуществляется намного быстрее, чем к файловой системе жесткого диска.</li>
<li>Selenoid позволяет использовать различное разрешение экрана: мы самостоятельно можем настраивать подходящее разрешение экрана для запущенного контейнера. Сделать это можно посредством выставления необходимых параметров в настройках компонента <i>Browser Capabilities</i>.</li>
<li>Видеозапись тестов: активация записи в Selenoid на примере браузера Google Chrome происходит за счет выставления параметра <i>true</i> в соответствующую настройку компонента <i>Browser Capabilities</i>:

<i>ChromeOptions options = new ChromeOptions();</i>
<i>options.setCapability(«enableVideo»,true);</i></li>
</ul>
Если кратко, <a href="https://selenide.org/index.html">Selenide</a> – это обёртка вокруг Selenium WebDriver, позволяющая быстро и просто его использовать при написании тестов. По своей сути, Selenide – это инструмент для автоматизации действия пользователя в браузере, ориентированный на удобство и легкость реализации бизнес-логики в автотестах на языке пользователя, не отвлекаясь на технические детали работы с «драйвером браузера». Для примера, нам не нужно акцентировать внимание на работе с ожиданиями элементов в процессе автоматизации тестирования динамических веб-приложений, а также на реализации высокоуровневых действий над элементами.
Ключевые и главные преимущества Selenide:
Лаконичный синтаксис в духе jQuery

<ul>
<li>Автоматическое решение большинства проблем с Ajax, ожиданиями и таймаутами</li>
<li>Управление жизнедеятельностью браузера</li>
<li>Автоматическое создание скриншотов</li>
</ul>
Цель Selenide – сосредоточиться на бизнес-логике тестов и не «растрачивать» ментальную энергию на технические детали.

Selenide — достаточно популярный инструмент, для которого есть много готовых решений. Часть возможностей Selenide доступна и у аналогов — Atlas, Selenium, HTMLElements и т.п. Но каждый из них по-своему нам не подходил.

Selenium лежит в основе Selenide. Но для наших целей он слишком низкоуровневый. Нет смысла изобретать велосипед, когда есть готовое решение.

Atlas появился совсем недавно. Он достаточно сырой и не имеет поддержки Groovy.
HtmlElements всем хорош, но устарел и не поддерживается. Есть еще JDI, но в нем возникли проблемы с многопоточностью.

Serenity, ранее использовавшийся на проекте, был слишком громоздким. В нем все настолько взаимосвязано, что для добавления какого-то нового обработчика или перехватчика событий приходилось переписывать десяток классов (и это не каждый раз приводило к успеху). Плюс к Serenity не получалось подключить Allure — фактический отраслевой и внутрикорпоративный стандарт для генерации тестовых отчетов. 

В Selenide с точки зрения автоматизатора все гораздо проще. Например, нет необходимости отдельно описывать шаги — привязываться к методам и т.п. Поскольку у него есть поддержка Allure из коробки, в тестовый отчет автоматически попадают все действия по работе с веб-элементами.

Разумеется, у Selenide есть поддержка PageFactory, Page Object и PageElement. Это делает код более читаемым. Плюс предусмотрены внутренние ожидания того момента, когда элемент появится, — нет необходимости явно прописывать, что нужно остановить тест на несколько секунд, прежде чем идти дальше (предельное время ожидания устанавливается в конфигах). Отдельно существуют и явные ожидания — можно на каждом тестовом шаге явно переопределить таймаут для нужных элементов.

Удобно, что у Selenide есть целый набор всевозможных готовых методов.

<source>
</source>

<img src="https://lh3.googleusercontent.com/xaQdrVZwu-be3t616MW29ZvL7NykdBHTHNVfCTUMgupHVDKrVB34Rzs2Yz7jQ9SUS8d4LF78CMaw9rp6xVOU8_yaeH0-VQMrtZCt7NdPhgMfDD6FI8WhdXPspnvRdQ" align="center">
Selenium Grid – кластер, состоящий из нескольких Selenium-серверов, который позволяет создавать распределенную сеть для одновременного запуска тестов в нескольких браузерах. Выделяют центральный сервер (хаб) и узлы (ноды), которые к нему подключены. (если отваливается хаб напр по сети или питанию, то соотв всё ломается) + (т.к. связь двусторонняя и хаб периодич опрашивает ноды, то быстро проявляется деградация производительности, уже на неск. Десятках нод)

Чем можно заменить Selenium Grid? Достойным вариантом является Selenoid – инструмент, с помощью которого можно быстрее и проще запускать браузеры в Docker-контейнерах. Процесс отличается от аналогичного в Selenium.

Для каждого запроса нового браузера Selenoid запускает новый контейнер и останавливает его после закрытия сессии.

В каждом контейнере находится определенная версия браузера, нужная версия веб-драйвера или Selenium-сервера и все необходимые зависимости (например, графические библиотеки). При этом благодаря изоляции процессов, можно запускать любое количество разных версий браузеров одновременно.

<source>
</source>
<h2>SELENOID VS. SELENIUM GRID</h2>
Цель использования данных решений одна – создание единой среды для параллельного запуска автотестов. При этом между решениями существует ряд важных отличий. В чем же преимущества Selenoid?

<ul>
<li><i>Изолированное окружение</i></li>
</ul>
В Selenoid каждый браузер запускается в отдельном контейнере, что позволяет полностью изолировать окружение браузера.

При использовании Selenium Grid существует вероятность, что настройки браузера могут быть изменены.

<ul>
<li><i>Масштабируемость</i></li>
</ul>
В процессе работы с Selenium Grid после создания большого количества нод тесты могут перестать выполняться.

В Selenoid окружение никак не влияет на качественное и непрерывное проведение тестов.

<ul>
<li><i>Потребление и утилизация ресурсов</i></li>
</ul>
Поскольку Selenium Server написан на Java, расход ресурсов при большой нагрузке значительно возрастает.

Selenoid позволяет поддерживать высокую нагрузку без дополнительных ресурсозатрат.

В среднем при десяти запущенных сессиях Selenium Server на Java потребляет 500 МБ оперативной памяти, в то время как Selenoid – всего 50–60 МБ.

Кроме того, Selenoid утилизирует все неактивные контейнеры после завершения сессии, тем самым постоянно поддерживая нужное количество свободной памяти.

<ul>
<li>Selenoid гораздо проще и быстрее устанавливается, чем Selenium Server.</li>
<li>С ним удобнее управлять браузерами.</li>
<li>На порядок более легкое масштабирование количества параллельных автотестов.</li>
<li>Имеет очень удобный UI и логирование.</li>
<li>Имеет дополнительные фишки, например, очереди. Если у вас на хост пришло слишком много автотестов одновременно, и хост не может их переработать, то Selenoid ставит их в очередь. И будет их пропускать по очереди, как только какие-то тесты уже завершатся.</li>
</ul>
<source>
</source>
Но это еще не все. Есть еще дополнительные преимущества.

<ul>
<li>Мы можем изменять конфигурации Selenoid на «горячую». Нам не нужно для этого останавливать хосты с Selenoid, мы просто правим JSON и там специальной командой Selenoid перезапускается, и не прерывая активных сессий он уже готов поставлять по запросу новые необходимые браузеры.</li>
<li>По умолчанию используются образы разработчиков Selenoid, но вы можете использовать готовые образы. Есть официальные образы от Selenium с браузерами. Или вы можете создать свой образ, если по политике безопасности вам не разрешают лезть в общедоступные репозитории. Внутри образа у вас должен быть браузер с WebDriver. Должен быть установлен X-сервер, чтобы браузер при запуске думал, что он запущен на реальном экране.</li>
<li>Поддержка централизованного логирования. Selenoid позволяет не просто смотреть отдельные логи браузера. У него есть специальный адрес в строке. Если туда обращаться, то он возвращает JSON с подобной статистикой того, что сейчас происходит на хосте. Это очень удобно применять для живого анализа того, что происходит. Можно подключить graphite, Grafana. И очень легко получать статистику, и выводить на больших экранах, и показывать текущую ситуацию. Например, отслеживать перезагрузку какого-нибудь хоста или какие-то аномалии.</li>
<li>И очень удобная штука – это задание разрешения экрана прямо через код автотестов, т. е. не разрешение самого браузера, с каким он отроется, а именно экрана, чтобы тестировать в том числе мобильные устройства. А именно, когда вы делаете узкий экран, эмулируете экран мобильника, тоже можно запускать и дополнительно проверять тесты.</li>
<li>И новая фича появилась недавно, буквально неделю назад. Это встроенная видеозапись тестов, т. е. подгружается специальный контейнер по умолчанию, который по VNC, если вы включили capability специальный, он в одно место складывает видеозапись прохождения автотестов. Но нужно понимать, что это очень грузит хост и нужно использовать только в режимах отладки, потому что по умолчанию Selenoid запускается без поддержки VNC и поддержки видеозаписи, чтобы максимально утилизировать доступные ресурсы для более стабильного запуска автотестов и прохождения.</li>
</ul>
В production, чтобы увеличить интенсивность прохождения тестов, Selenoid и Selenoid-UI разносят на разные хосты, чтобы они друг другу не мешали при больших нагрузках.

<ul>
<li>Я пришел к тому, что если у вас больше 5 автоматизаторов, то надо внедрять Selenoid. Это реально вам поможет, тем более, что порог входа очень маленький. И ничего не мешает это сделать. И даже если вы один работаете, то большое количество запусков параллельных тестов позволяет вам в тестировании внедрить параметризацию. Например, раньше вы не могли себе позволить использовать случайные значения для автотестов или граничные значения проверять. А теперь, если у вас большое количество одновременных сессий, вы можете очень легко параметризацию проверять.</li>
<li>Очень просто мигрировать. Он виден как обычный Selenium Hub. И ничего не нужно менять в коде. Если вам нужны дополнительные возможности, то вы просто capabilities добавляете.</li>
<li>Экономит время, ресурсы и нервы. Это очень важно. У нас работа вредная, а молоко не дают.</li>
<li>Бесплатный + низкая стоимость владения. Т. е. он требует мало ресурсов на обслуживание. А почему бесплатный? Потому что ребята его сделали сначала для Яндекса, но потом поняли, что инструмент получился хороший и в то же время им ресурсов не хватает для его тестирования, потому что появляются новые браузеры, новые веб-драйверы. И на этом стыке появляются какие-то баги, которые даже в масштабах Яндекса трудно заметить.</li>
<li>Они выложили все это в открытый доступ, чтобы увеличить аудиторию, которая растет с каждым днем. Например, Саймон рассказывал про <a href="https://github.com/zalando/zalenium">zalenium</a> вчера, т. е. это Selenium в Docker. У него в репозитории в Docker 150 000 скачиваний. А у Selenoid уже 300 000 скачиваний. Можно сказать, что реальных внедрений уже где-то 1 000. И это действительно так, у них есть Telegram-канал свой. И я заметил, что в последние несколько месяцев там все больше коллег из Индии появляется, которые очень активно используют Selenoid в реальном применении. И ребята уже столкнулись с тем, что появляются не совсем адекватные запросы. Но они стараются продукт делать простым и мощным. Неадекватные запросы не реализуются, чтобы стабильность была в первую очередь.</li>
</ul>
PICT инструмент для pairwise тестирования (когда есть например 10х10 разных параметров смартфонов, выбираются по одной паре параметров чтоб было достаточно. Пикт комбинирует и выдаёт минимальный набор пар для полного охвата тестов). Либо ACTS тоже самое только с интерфейсом, а не в ком строке. Там еще куча на сайте <a href="http://www.pairwise.org/">http://www.pairwise.org/</a>

<img src="https://lh4.googleusercontent.com/vEPnESvNm9-TLHmC_elhmyxSKrBiBMe-rHZ5pgBrJm0_yJ_ZRTy4NVpUWrOCDw7KGV26pL5aacrUlxs7FDzBMlXyqGFKoAFXyqU_fAOqxmLmTXWyaMA4geBWZebj1A" align="center">
POSTMAN

<a href="https://www.youtube.com/watch?v=vaEHDkDcPTo&list=LLlZaXx9Cfc-at7iDWEn8_RQ&index=83&t=0s">https://www.youtube.com/watch?v=vaEHDkDcPTo&list=LLlZaXx9Cfc-at7iDWEn8_RQ&index=83&t=0s</a>

<a href="https://www.youtube.com/watch?v=hGmJMeE_ok0&list=LLlZaXx9Cfc-at7iDWEn8_RQ&index=89&t=0s">https://www.youtube.com/watch?v=hGmJMeE_ok0&list=LLlZaXx9Cfc-at7iDWEn8_RQ&index=89&t=0s</a>

<img src="https://lh4.googleusercontent.com/22yJkO93Ghkr-yrCUQueFlzEtPjcvH_NBzopk4QNBPKqz9SGmwZEgXjhS8an7AYlPF2WV0_QWptKCGZrxFGAINs5PBnRLJCjd0MzL48RBsMvuWtyQpIJUB4feE2t5w" align="center">
<img src="https://lh4.googleusercontent.com/TaxLIBZuZ3EIkwPzYLrgD9mtPPVr-5Y7n2SMtZBCeuiSBfQ46F6fsw83JmICgaYPwVkiArDWAPOrvITcWj5MnM45T126Nt35khgRzMWd8QuX8joCq1vRUiSaoII2VQ" align="center">
По сути Swagger – это фреймворк для спецификации RESTful API. Его прелесть заключается в том, что он дает возможность не только интерактивно просматривать спецификацию, но и отправлять запросы – так называемый Swagger UI, вот так это выглядит: 
<img src="https://lh4.googleusercontent.com/OApONMrQiNGIN_lirErbmwqdYikQ6RMIGzID9hbE6wKJRKh6YvgiJ2Y4VZwpJOAE0j9SOMMZgTGANoV0OE11gxewnxVkCnrlOZfpX7ZKp015c7qoYfGHdWBNrnBRYg" align="center">
<strong>Swagger</strong> is an <a href="https://en.wikipedia.org/wiki/Open-source_software">open-source software</a> framework backed by a large ecosystem of tools that helps developers design, build, document, and consume <a href="https://en.wikipedia.org/wiki/Representational_state_transfer">RESTful</a> <a href="https://en.wikipedia.org/wiki/Web_API">web services</a>. While most users identify Swagger by the Swagger UI tool, the Swagger toolset includes support for automated documentation, code generation, and test-case generation. Swagger — это программная среда с открытым исходным кодом, опирающаяся на обширную экосистему инструментов, которая помогает разработчикам проектировать, создавать, документировать и использовать веб-сервисы RESTful. В то время как большинство пользователей идентифицируют Swagger с помощью инструмента пользовательского интерфейса Swagger, набор инструментов Swagger включает поддержку автоматической документации, генерации кода и генерации тестовых примеров.

Simplify API development for users, teams, and enterprises with the Swagger open source and professional toolset. Find out how Swagger can help you design and document your APIs at scale. Swagger UI — один из самых популярных инструментов для создания интерактивной документации. Swagger UI создает интерактивную консоль API для экспериментов с запросами в реальном времени. 

Newman is a command-line collection runner for Postman. It allows you to effortlessly run and test a Postman collection directly from the command-line. It is built with extensibility in mind so that you can easily integrate it with your continuous integration servers and build systems. Newman — это сборщик команд в командной строке для Postman. Это позволяет вам легко запускать и тестировать коллекцию Postman непосредственно из командной строки. Он построен с учетом расширяемости, поэтому вы можете легко интегрировать его с вашими серверами непрерывной интеграции и системами сборки.

Стэк ELK (Elasticsearch+Logstash+Kibana)

<img src="https://lh5.googleusercontent.com/GagGd1ihrFY4uflQzr85zvQYW4qrHFOZc3Qsr9m2r2ygLRo2H03H90j15G74VWkQv3agylss_GOmzb7pwS08ZwLjl9zmArs5Z7ogVKBGsYDN_693gw2_0b9mzxsfdw" align="center">
<strong>Kibana</strong> – тиражируемая <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B2%D0%BE%D0%B1%D0%BE%D0%B4%D0%BD%D0%BE%D0%B5_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D0%B5">свободная</a> програмная панель <a href="https://ru.wikipedia.org/wiki/%D0%92%D0%B8%D0%B7%D1%83%D0%B0%D0%BB%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8F_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85">визуализации данных</a>. В процессе использования программы информация, проиндексированная в кластере <a href="https://ru.wikipedia.org/wiki/Elasticsearch">Elasticsearch</a>, представляется в виде <a href="https://ru.wikipedia.org/wiki/%D0%94%D0%B8%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0">диаграмм</a> различных видов

Как правило Kibana используется для мониторинга и анализа ИТ-инфраструктуры в составе <strong>Elastic Stack</strong> (ранее <strong>ELK Stack</strong>), в который помимо нее входят <a href="https://ru.wikipedia.org/wiki/Elasticsearch">Elasticsearch</a> и <a href="https://ru.wikipedia.org/w/index.php?title=Logstash&action=edit&redlink=1">Logstash</a>. <strong>Logstash</strong> отвечает за логирование и поставляет входящий поток данных в <strong>Elasticsearch</strong> для хранения, классификации и поиска. <strong>Kibana</strong>, в свою очередь, получает доступ к данным <strong>Elasticsearch</strong> для их визуализации в различных визуальных форматах, например – в виде информационных панелей (dashboards) с различными видами диаграмм.

Clumsy целенаправленно ухудшает условия, в которых работает Ваше сетевое соединение в Windows

JHipster is a development platform to quickly generate, develop, & deploy modern web applications & microservice architectures.

Burp Suite – это платформа для проведения <a href="https://www.pentestit.ru/site-security-audit/">аудита безопасности веб-приложений</a>. Содержит инструменты для составления карты веб-приложения, поиска файлов и папок, модификации запросов, фаззинга, подбора паролей и многое другое. Также существует магазин дополнений BApp store, содержащий дополнительные расширения, увеличивающие функционал приложения.

Burp Suite — это интегрированная платформа, предназначенная для проведения аудита веб-приложения, как в ручном, так и в автоматических режимах. Содержит интуитивно понятный интерфейс со специально спроектированными табами, позволяющими улучшить и ускорить процесс атаки. Сам инструмент представляет из себя проксирующий механизм, перехватывающий и обрабатывающий все поступающие от браузера запросы. Имеется возможность установки сертификата burp для анализа https соединений.

Если посмотреть статистику и репорты bug-bounty программ — практически везде на скриншотах можно встретить использование этого инструмента. На ряду с OWASP ZAP это самый популярный набор утилит для тестирования веб-приложений.
 

<img src="https://lh6.googleusercontent.com/p90b16n_HO2r-Sm14e8MOeQwus9Ik6XkFeVeBPbfRya-curTbwVMncam_uXeW9cxQipkfHUgilYVJfVqrgNzXBubURPbML40Pa50xoHqpWSarosDQz20OdVmC1VfMg" align="center">
sqlmap is an open source penetration testing tool that automates the process of detecting and exploiting SQL injection flaws and taking over of database servers. It comes with a powerful detection engine, many niche features for the ultimate penetration tester and a broad range of switches lasting from database fingerprinting, over data fetching from the database, to accessing the underlying file system and executing commands on the operating system via out-of-band connections.

<img src="https://lh4.googleusercontent.com/nNd80oxbLK2oiFOsrjF_ba7g9dn1NU4sQTVs9tO2LAfOsZ7bTdFuNj-Yb2W0IVweo44JN2V-IKRvOuWR56SFYLdJco2PdAIu98VU8h52KzMzxf6z0XJ0jG5n0XZ_pQ" align="center">
<h1>Features</h1>
<ul>
<li>Full support for <strong>MySQL, Oracle, PostgreSQL, Microsoft SQL Server, Microsoft Access, IBM DB2, SQLite, Firebird, Sybase, SAP MaxDB, Informix, MariaDB, MemSQL, TiDB, CockroachDB, HSQLDB, H2, MonetDB, Apache Derby, Amazon Redshift, Vertica, Mckoi, Presto, Altibase, MimerSQL, CrateDB, Greenplum, Drizzle, Apache Ignite, Cubrid, InterSystems Cache, IRIS, eXtremeDB and FrontBase</strong> database management systems.</li>
<li>Full support for six SQL injection techniques: <strong>boolean-based blind, time-based blind, error-based, UNION query-based, stacked queries and out-of-band</strong>.</li>
<li>Support to <strong>directly connect to the database</strong> without passing via a SQL injection, by providing DBMS credentials, IP address, port and database name.</li>
<li>Support to enumerate <strong>users, password hashes, privileges, roles, databases, tables and columns</strong>.</li>
<li>Automatic recognition of password hash formats and support for <strong>cracking them using a dictionary-based attack</strong>.</li>
<li>Support to <strong>dump database tables</strong> entirely, a range of entries or specific columns as per user's choice. The user can also choose to dump only a range of characters from each column's entry.</li>
<li>Support to <strong>search for specific database names, specific tables across all databases or specific columns across all databases' tables</strong>. This is useful, for instance, to identify tables containing custom application credentials where relevant columns' names contain string like name and pass.</li>
<li>Support to <strong>download and upload any file</strong> from the database server underlying file system when the database software is MySQL, PostgreSQL or Microsoft SQL Server.</li>
<li>Support to <strong>execute arbitrary commands and retrieve their standard output</strong> on the database server underlying operating system when the database software is MySQL, PostgreSQL or Microsoft SQL Server.</li>
<li>Support to <strong>establish an out-of-band stateful TCP connection between the attacker machine and the database server</strong> underlying operating system. This channel can be an interactive command prompt, a Meterpreter session or a graphical user interface (VNC) session as per user's choice.</li>
<li>Support for <strong>database process' user privilege escalation</strong> via Metasploit's Meterpreter getsystem command.</li>
</ul>
Основные возможности OWASP ZAP:

<ul>
<li>Man-in-the-middle Proxy</li>
<li>Traditional and AJAX spiders</li>
<li>Automated scanner</li>
<li>Passive scanner</li>
<li>Forced browsing</li>
<li>Fuzzer</li>
</ul>
<source>
</source>
<strong>Какие модули и места следует подвергать автоматизации?</strong>

<ul>
<li>Участки кода, исполнение которых трудно визуализировать и получить осязаемую информацию о протекающих процессах (back-end процессы, занесение в базу данных, занесение логов в файл).</li>
<li>Функциональность продукта, которая будет использоваться наиболее часто и возникновение ошибок которой связано с достаточно высоким риском. Автоматизированное тестирование узловых моментов функциональности потребует меньше времени для поиска ошибок. И соответственно, сократит время на их устранение.</li>
<li>Типовые часто выполняемые операции, которые обычно связаны с обработкой данных. Например – формы, в которых количество заполняемых граф и полей довольно значительное. Цель – автоматизировать занесение требуемых данных в нужное поле и проверить правильность выполнения задачи после сохранения результата.</li>
<li>Сообщения об ошибках. Требуется автоматизация разнесения некорректных данных по соответствующим полям и тестирование корректности проверки правильности данных и сообщений об ошибках.</li>
<li>Комплексная проверка поведения всей системы, как целостного объекта (end-to-end testing).</li>
<li>Проверка числовых массивов, нужных для достоверных математических операций.</li>
<li>Тестирование корректности отображаемых результатов поиска в ответ на запрос по нужным данным.</li>
<li>Предложенный список только ориентировочный. Всё зависит от предъявляемых к проверяемой системе требований, возможностей, которые позволяет реализовать выбранный для автоматического тестирования инструмент.</li>
</ul>
<strong>Тест кейсы для автоматизации</strong>

<ul>
<li>Create/Read/Update/Delete операции. Простейший пример – работа с пользователем. Ввод, просмотр и коррекция данных о нём, удаление введённой информации.</li>
<li>Типовые последовательности при эксплуатации приложения. В качестве примера может выступить работа с почтовым менеджером: авторизация, просмотр писем, пролистывание имеющихся, создание новых и их отправка, выход. Это и есть end-to-end последовательность, тестирующая полный объём выполняемых действий и манипуляций. Достоинство таких сценариев в том, что по окончании теста, система возвращается в исходное состояние (или где-то около него), значит, уменьшается влияние на результаты иных тестов.</li>
<li>Другие случаи, когда ручное тестирование не подходить по ряду причин. Примером может служить проверка структуры создаваемых системой файлов.</li>
</ul>