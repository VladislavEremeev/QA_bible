# Manual part 1
<br>
<h1>----- Введение (F.A.Q.) -----</h1>

<h2>Хочу войти в айти (в разработку) через тестирование, хороший план?</h2>
Это имело смысл (и то спорно) несколько лет назад, но после эпидемии и агрессивной рекламы работы в IT со стороны обучающих компаний появились тысячи выпускников курсов по тестированию, так что этого "легкого пути вкатиться в айтишечку" уже нет и не будет. Конкурс на одно место на удаленку может доходить до нескольких сотен человек. Конечно, в разработке тоже конкуренции поприбавилось, но если вы нацелены стать программистом, то никакие вхождения через другие специальности не имеют ни малейшего смысла - тестирование и разработка - разные профессии и опыт работы джуниор тестировщиком вам практически ничем не пригодится, вы лишь потратите время на подготовку к собеседованиям (а требования теперь весьма высокие), а потом еще на обучение непосредственно той специальности, куда хотели изначально, т.к. опыт по сути не релевантен и спрашивать будут с нуля.

Доп. материал:
<a href="https://www.youtube.com/watch?v=qiCjqqtWP7I&t=31s">Мифы о тестировании #2 / О чем не говорят на курсах по тестированию / Правда о работе в IT</a>
<h2>Хочу зарабатывать много денег, мне сюда?</h2>
Первые зарплаты будут мизерными (особенно учитывая конкурс на места), а подняться выше по карьерной лестнице без искреннего интереса и запала не получится, тестирование - слишком обширная область знаний. Без внутренней мотивации к ежедневному самообучению не получится зарабатывать больше чем в любой другой профессии на старте. Так что сферу деятельности стоит менять только если вы всю жизнь чувствовали, что занимаетесь не тем, а тут прям вот екнуло и хочется взахлеб осваивать именно тестирование. Но даже в этих случаях нужно понимать, что далеко не всем компаниям требуются профессиональные тестировщики, разработчикам в этом смысле найти применение своим навыкам куда проще. Именно по этой причине существует отток уже проработавших какое-то время в тестировании специалистов в другие направления: менеджмент, чистая автоматизация, разработка. Фактически они просто не смогли найти дальнейшие пути развития своих навыков. Соответственно и зарплаты здесь в среднем ниже, чем на многих специальностях в IT. 
Статистика зарплат: <a href="https://career.habr.com/salaries">Россия</a>, <a href="https://jobs.dou.ua/salaries/">Украина</a>, <a href="https://salaries.dev.by/">Беларусь</a>
<h2>Хочу работать удаленно джуном, это возможно?</h2>
К сожалению, шансы устроиться на удаленку специалисту без опыта довольно низкие - высокая конкуренция, к тому же компании охотнее берут начинающих в офис (так эффективнее обучать). Поэтому попробовать, конечно, стоит, но рассчитывать на это особо не нужно. Да и начинающему действительно продуктивнее находиться в офисе вместе со всей командой, в гуще событий.
<h2>Что реально должен знать junior? А что спросят на собеседовании?</h2>
Вот пара ссылок на карты знаний для тестировщиков, но можете на просторах найти и другие.
<a href="https://github.com/anas-qa/Quality-Assurance-Road-Map">https://github.com/anas-qa/Quality-Assurance-Road-Map</a> <a href="https://www.mindmeister.com/ru/1324282825/junior-qa?fullscreen=1">https://www.mindmeister.com/ru/1324282825/junior-qa?fullscreen=1</a> <a href="https://www.mindmeister.com/ru/1558647509?t=973hdS2AKb">https://www.mindmeister.com/ru/1558647509?t=973hdS2AKb</a>
Некоторые компании подробно расписывают на своих порталах ожидания от каждой стадии развития сотрудника, тоже не проблема найти, по этой же теме много видео на Youtube (<a href="https://www.youtube.com/watch?v=l9ezImoh5ac&feature=emb_logo&ab_channel=LearnQA%3A%D0%9E%D0%BD%D0%BB%D0%B0%D0%B9%D0%BD%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D1%89%D0%B8%D0%BA%D0%BE%D0%B2">раз</a>, <a href="https://www.youtube.com/watch?v=wDHZsoZIxcY&ab_channel=LearnQA%3A%D0%9E%D0%BD%D0%BB%D0%B0%D0%B9%D0%BD%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D1%89%D0%B8%D0%BA%D0%BE%D0%B2">два</a>, <a href="https://www.youtube.com/watch?v=tzOhRHVX6ko&ab_channel=QAQC">три</a>, <a href="https://www.youtube.com/watch?v=5DGuDT98EC0&ab_channel=AzatZakuanov">четыре</a>, …). Еще один ориентир – просто открыть и почитать вакансии в своем городе, что в среднем у вас требуется от новичка.
Если же попытаться выделить самые частые вопросы на собеседованиях, то получится примерно следующее:
<ul>
<li>Что такое тестирование?
</li>
<li>Зачем оно нужно?
</li>
<li>QA/QC/Тестирование - разница?
</li>
<li>Что такое качество ПО?
</li>
<li>Верификация и валидация?
</li>
<li>Severity priority?
</li>
<li>Виды, типы, уровни тестирования?
</li>
<li>Виды документации? Тест-план, тест-кейс, чек-лист?
</li>
<li>Что такое баг? Его жизненный цикл?
</li>
<li>Техники тест-дизайна?
</li>
<li>SDLC, STLC; Методологии разработки ПО?
</li>
<li>Мобильное тестирование: его особенности (и в частности жизненный цикл Android и iOS приложения)?
</li>
<li>Клиент-серверная архитектура?
</li>
<li>API?
</li>
<li>Базовое знание сетей: HTTP(S), его методы, коды ответов, Query-параметры, REST/SOAP, JSON/XML
</li>
<li>Базы данных: что такое SQL, СУБД, основные команды (особенно любят джойны).
</li>
<li>Инструменты: Chrome DevTools, Postman, Charles/Fiddler, GIT, TMS
</li>
<li>Практика: тестирование форм или какого либо сайта, приложения  (в частности  составление тест-кейсов и баг-репортов), придумать хороший summary для репорта, определение severity/priority; SQL запросы; что-нибудь на "подумать".
</li>
</ul>

В случае gamedev могут еще спросить про последнее во что играл, что понравилось/не понравилось и т.п.

Помимо вышеперечисленного нужно помнить об английском языке и его важности в работе. Конечно, есть небольшое количество компаний, которые не станут уделять этому внимания, но если в вакансии указан необходимый уровень владения языком, то будьте готовы к тому, что как минимум попросят ответить на какой-нибудь простенький житейский или из списка HR-вопросов на английском. В отдельных случаях, где явно указана необходимость разговорного уровня, все собеседование вполне может пройти на английском.

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/company/funcorp/blog/426759/">Образ современного тестировщика. Что нужно знать и уметь</a>
</li>
<li><a href="https://habr.com/ru/company/funcorp/blog/491188/">Что должен знать тестировщик бэкенда</a>
</li>
<li><a href="https://www.youtube.com/watch?v=Yd0Z-35GbK4&feature=youtu.be&ab_channel=%D0%9B%D1%91%D1%88%D0%B0%D0%9C%D0%B0%D1%80%D1%88%D0%B0%D0%BB">Тестировщик ПО / что делает QA Engineer / интервью с Artsiom Rusau QA</a>
</li>
<li><a href="http://mymonday.by/qa-market-research-august-2019">Исследование рынка труда в QA</a>
</li>
<li><a href="https://ru.hexlet.io/blog/posts/gid-po-professii-testirovschik-chem-zanimaetsya-skolko-zarabatyvaet-chto-nado-znat-i-gde-uchitsya">Гид по профессии тестировщик: чем занимается специалист в сфере QA, сколько зарабатывает, что надо знать и где учиться</a>
</li>
<li><a href="https://habr.com/ru/company/otus/blog/530290/">Качественное тестирование ПО</a>
</li>
</ul>
<h2>С чего начать обучение?</h2>
Начать нужно с ознакомления с тестированием и я считаю, что лучший выбор для этого - книга Романа Савина "Тестирование дот ком". После ознакомления я бы посоветовал выбрать по отзывам в коммьюнити хороший базовый онлайн-курс и пройти его, либо по возможности пойти на офлайн-курсы местной компании с возможностью последующего трудоустройства - это вообще лучший вариант. Если нет желания или возможности, то после Савина стоит начать с книги Святослава Куликова "Тестирование программного обеспечения. Базовый курс" и далее уже имея общее представление и понимая азы равномерно восполнять пробелы, подготавливаясь к собеседованиям.
Тестирование – самая широкая область в IT. Т.к. теория хоть и не сильно сложная, но ее настолько много, что невозможно изучить все, нужно пытаться как можно быстрее найти применение своим навыкам. Начать стоит с классики типа тестирования форм, тренировочных сайтов с дефектами специально для тестировщиков и т.п. Не стоит забывать и о софт скилах и базовой грамотности. Бич многих современных тестировщиков даже высокого уровня – безграмотность, поэтому смолоду тренируйтесь в составлении тестовых артефактов.
По мере роста компетенций как можно раньше стоит начать проходить собеседования и пытаться устроиться на любую стажировку, вообще любой вариант, где вы сможете применять знания и указать этот опыт в резюме, т.к. без опыта сейчас найти работу очень трудно. Если нет никаких оффлайн вариантов, как было у меня, можете регистрироваться на краудтестинговых платформах (но зачастую это гиблое дело + многие работодатели игнорируют такой опыт), искать в тг-каналах возможности протестировать какие-то проекты за бесплатно (иногда там ищут волонтеров за опыт) либо придумать такой тестовый проект себе самому - взяться тестировать любимый( или какой-либо популярный) сервис, но делать это близко к тому, будто это ваша реальная работа. То есть чтобы было что потом рассказать и показать результаты (тест-кейсы, баг-репорты и т.п.). Именно поэтому эффективнее обучаться когда есть опытный наставник, который дает приближенные к реальным задания и дает обратную связь по выполненной работе.
Когда вы устроитесь на свою первую работу, спустя некоторые время сможете начать готовиться к дальнейшему развитию и выбору направления, ведь никто не заставляет всю жизнь быть ручным тестировщиком. Вы можете сосредоточиться на mobile/web/desktop платформе, профессионально развиваться в менеджеры или автоматизацию, готовиться к узкой специализации — безопасности или performance и т. д., а также сфокусироваться на подготовке по перспективным направлениям:
<ul>
<li>ML&AI в QA
</li>
<li>QAOps
</li>
<li>Тестирование IoT
</li>
<li>Тестирование больших данных
</li>
</ul>
Помимо прочего, специалисту, планирующему развиваться профессионально, желательно как можно раньше начать сначала посещать релевантные митапы и конференции, а когда-нибудь и начать выступать в роли докладчика. Также не лишними будут различные сертификации (хотя бы тот же ISTQB разных уровней). 

Дополнительные ссылки:
<a href="https://habr.com/ru/company/jugru/blog/541334/">Тестирование в эпоху ИИ</a>
<a href="https://sarahelson81.medium.com/12-important-software-testing-trends-for-2021-you-need-to-know-b23e8f7d6cb7">12 Important Software Testing Trends for 2021 You Need to Know</a>
<a href="https://dou.ua/lenta/columns/how-to-learn/">Как учиться, чтобы научиться</a>

<h2>Какие есть полезные ресурсы кроме этого?</h2>

Telegram:
Must have! Каналы это: знакомство с коммьюнити, живое общение, уникальный опыт тысяч коллег; богатая история сообщений, где поиском по истории сообщений можно найти все что угодно; в шапке каждого канала закреплено сообщение со своим набором полезностей. Кроме того, некоторые каналы специализируются на мониторинге нового полезного материала с основных порталов, так что можно даже не погружаться с головой в хабр, доу, медиум и т.п., вам отберут все самое полезное. В конце концов, в этих каналах публикуются анонсы грядущих онлайн-мероприятий, чтобы ничего не упустить.
<ul>
<li>Всем новичкам сюда! Тренировочные собеседования, интересные обсуждения https://t.me/qa_interviews
</li>
<li>Огромный чат, ориентированный на джуниоров https://t.me/qajuniors
</li>
<li>Огромный чат, ориентированный на уже работающих в сфере тестирования <a href="https://t.me/qa_ru">https://t.me/qa_ru</a>
</li>
<li>Чат по геймдеву https://t.me/qa_gamedev
</li>
<li>Обсуждение курсов, отзывы о них https://t.me/qa_courses
</li>
<li>Тут можно размещать свое резюме <a href="https://t.me/qa_resumes">https://t.me/qa_resumes</a>
</li>
<li>Тут отзывы о компаниях https://t.me/qa_bad_company
</li>
<li>Обсуждение финансов https://t.me/qa_fin
</li>
<li>Публикация книг <a href="https://t.me/booksqa">https://t.me/booksqa</a>
</li>
<li>Авторский бложик https://t.me/shooandendlessagony
</li>
<li>Репосты новых статей и полезных ссылок с разных сайтов: 
</li>
<ul>
<li><a href="https://t.me/qa_wiki">https://t.me/qa_wiki</a>
</li>
<li><a href="https://t.me/serious_tester">https://t.me/serious_tester</a>
</li>
<li><a href="https://t.me/qa_pro">https://t.me/qa_pro</a>
</li>
<li><a href="https://t.me/qa_chillout">https://t.me/qa_chillout</a>
</li>
<li><a href="https://t.me/yetanotherqa">https://t.me/yetanotherqa</a>
</li>
</ul>
</ul>

Youtube-каналы:
<ul>
<li>Вадим Ксендзов (тренировочные собеседования!) https://www.youtube.com/channel/UC6hNNlCXv1ZgdGpziNf83RA
</li>
<li>Mikhail Portnov: <a href="https://www.youtube.com/channel/UCDbzkNMBNZJBKP4C-9qGw4Q">https://www.youtube.com/channel/UCDbzkNMBNZJBKP4C-9qGw4Q</a>
</li>
<li>Podlodka Podcast <a href="https://www.youtube.com/channel/UCOei1E1Vqq10S913OEqTWGw">https://www.youtube.com/channel/UCOei1E1Vqq10S913OEqTWGw</a>
</li>
<li>QA START UP: <a href="https://www.youtube.com/channel/UCAlCZby7zJHzyhOmS8issDQ">https://www.youtube.com/channel/UCAlCZby7zJHzyhOmS8issDQ</a>
</li>
<li>Компания DINS: <a href="https://www.youtube.com/channel/UCmJYB3hvbF3AlVh9HFeXX3A">https://www.youtube.com/channel/UCmJYB3hvbF3AlVh9HFeXX3A</a>
</li>
<li>Artsiom Rusau QA Life <a href="https://www.youtube.com/c/ArtsiomRusauQALife">https://www.youtube.com/c/ArtsiomRusauQALife</a>
</li>
<li>Леша Маршал <a href="https://www.youtube.com/channel/UCTVciJQp8eYwKLLQIl-iSJw">https://www.youtube.com/channel/UCTVciJQp8eYwKLLQIl-iSJw</a>
</li>
<li>Тестирование: <a href="https://www.youtube.com/channel/UC9VeXtf7fcCJUfmZ_cyweXA">https://www.youtube.com/channel/UC9VeXtf7fcCJUfmZ_cyweXA</a>
</li>
<li>Fest Group: <a href="https://www.youtube.com/channel/UClTnsvgTiW2YcfP1tcI2oKA">https://www.youtube.com/channel/UClTnsvgTiW2YcfP1tcI2oKA</a>
</li>
<li>QAGuild: <a href="https://www.youtube.com/channel/UCHtyBZ2XbtsRmNiAxh48RGg">https://www.youtube.com/channel/UCHtyBZ2XbtsRmNiAxh48RGg</a>
</li>
</ul>

Web:
<ul>
<li><a href="https://blog.noveogroup.ru/2020/01/testovye-ploschadki-dlya-trenirovok/">Большой список тестовых площадок для тренировок</a>
</li>
<li>https://cantunsee.space/
</li>
<li>https://software-testing.ru/ (+форум)
</li>
<li>http://www.mobileappstesting.com/
</li>
<li><a href="https://www.guru99.com/">https://www.guru99.com</a>
</li>
<li><a href="https://www.softwaretestingmaterial.com/">https://www.softwaretestingmaterial.com/</a>
</li>
<li><a href="https://www.ministryoftesting.com/">https://www.ministryoftesting.com/</a>
</li>
<li><a href="http://www.testingeducation.org/BBST/foundations/">http://www.testingeducation.org/BBST/foundations/</a>
</li>
<li>https://www.learnqa.ru/ 
</li>
</ul>

Книги:
Очень хвалят вот эту подборку <a href="http://okiseleva.blogspot.com/2014/02/blog-post_6.html?m=1">http://okiseleva.blogspot.com/2014/02/blog-post_6.html?m=1</a>
<br>
Подборка книг по ИБ <a href="https://habr.com/ru/company/mailru/blog/282700/">https://habr.com/ru/company/mailru/blog/282700/</a>
<br>
<a href="https://drive.google.com/file/d/173NvdE4dnKxxbo0mdoPwcDMcdjCWaUTM/view">Перевод книги Ли Копланда "A Practitioner's Guide to Software Test Design"</a>

Еще встречал вот такой список:
<ul>
<li>Роман Савин «Тестирование Дот Ком, или Пособие по жестокому обращению с багами в интернет-стартапах» (можно сказать худ.лит, «для чайников»)
</li>
<li>Святослав Куликов «Тестирование программного обеспечения. Базовый курс.»
</li>
<li>Арбон Джейсон, Каролло Джефф, Уиттакер Джеймс «Как тестируют в Google»
</li>
<li>Борис Бейзер «Тестирование черного ящика. Технологии функционального тестирования программного обеспечения и систем»
</li>
<li>Рекс Блэк «Ключевые процессы тестирования»
</li>
<li>Гленфорд Майерс, Том Баджетт, Кори Сандлер «Искусство тестирования программ.»
</li>
<li><a href="https://www.amazon.com/s/ref=dp_byline_sr_book_1?ie=UTF8&field-author=Microsoft+Corporation&text=Microsoft+Corporation&sort=relevancerank&search-alias=books">Microsoft Corporation</a> - Performance testing Guidance for Web Applications
</li>
</ul>

Мобильные приложения:
<ul>
<li><a href="https://play.google.com/store/apps/details?id=com.strimqa.android.app.strimqa&hl=ru&gl=US">StrimQa — ваш карьерный навигатор! </a>
</li>
</ul>
Другие сборники материала и ответов на вопросы:
<ul>
<li><a href="https://drive.google.com/file/d/1x9oeWuPiVqytNYTKunJgLLarq4IBdeTY/view?usp=sharing">https://drive.google.com/file/d/1x9oeWuPiVqytNYTKunJgLLarq4IBdeTY/view?usp=sharing</a>
</li>
<li><a href="https://www.istqb.org/downloads/category/2-foundation-level-documents.html">https://www.istqb.org/downloads/category/2-foundation-level-documents.html</a>
</li>
<li><a href="https://github.com/ultragreatester/how-to-qa">https://github.com/ultragreatester/how-to-qa</a>
</li>
<li><a href="https://habr.com/ru/post/257529/">https://habr.com/ru/post/257529/</a>
</li>
<li><a href="https://docs.google.com/file/d/18yJqziwhxz5khP1mtrme1mNJW95mwrgc/edit?filetype=msword">https://docs.google.com/file/d/18yJqziwhxz5khP1mtrme1mNJW95mwrgc/edit?filetype=msword</a>
</li>
</ul>

Словари терминов (в т.ч. элементов интерфейса):
<ul>
<li><a href="https://habr.com/ru/company/wrike/blog/475558/">Словарик айтишника или Что? Где? Куда? Часть 1</a>
</li>
<li><a href="https://habr.com/ru/company/jugru/blog/538698/">IT-словарик для не-айтишников</a>
</li>
<li><a href="https://docs.google.com/spreadsheets/d/1LgytNrl7ep9wlr3A_3u0NitQsrZzKhEQwC-OTQfbLAM/edit?usp=sharing">https://docs.google.com/spreadsheets/d/1LgytNrl7ep9wlr3A_3u0NitQsrZzKhEQwC-OTQfbLAM/edit?usp=sharing</a>
</li>
<li><a href="https://docs.google.com/spreadsheets/d/1r5Ek83V4IHkOsW52DyVT8iJepR20oZu_Jy5vAkq7SrI/edit?usp=sharing">https://docs.google.com/spreadsheets/d/1r5Ek83V4IHkOsW52DyVT8iJepR20oZu_Jy5vAkq7SrI/edit?usp=sharing</a>
</li>
<li><a href="https://borodaboroda.com/blog/elementy-interfejsa-sajta/">Элементы интерфейса сайта</a>
</li>
<li><a href="https://habr.com/ru/company/youla/blog/540768/">UI-элементы и жесты в мобильных приложениях</a>
</li>
<li><a href="https://vk.com/@zapiskisedogotestera-slovar-testirovschika">Словарь тестировщика</a>
</li>
</ul>

Чек-листы и идеи для тестов:
<ul>
<li><a href="https://habr.com/ru/post/524784/">Где брать идеи для тестов (подборка полезных ссылок)</a>
</li>
<li><a href="https://habr.com/ru/post/537510/">37 источников тест-идей</a>
</li>
<li><a href="https://checkvist.com/checklists/476089">Checklists Base :)</a>
</li>
<li><a href="https://habr.com/ru/post/534190/">Чек-лист тестирования мобильных приложений</a>
</li>
<li><a href="https://habr.com/ru/company/funcorp/blog/525538/">Дополняем чек-лист тестирования при обновлении иконки и сплеша в мобильных приложениях</a>
</li>
<li><a href="https://software-testing.ru/images/stories/library/checklist-mobile-app-testen.pdf">Чеклист для тестирования мобильных приложений </a>
</li>
<li><a href="https://habr.com/ru/post/525192/">Чек-лист для тестирования числового поля</a>
</li>
<li><a href="https://habr.com/ru/post/542422/">Чек-лист тестирования WEB приложений</a>
</li>
<li><a href="http://www.mobileappstesting.com/2012/07/05/testing-checklist-for-mobile-applications/">Testing checklist for mobile applications</a>
</li>
<li><a href="https://ontestpad.com/library/200/ios-app-testing-template">iOS App Testing Template</a>
</li>
<li><a href="https://www.flickr.com/photos/softwaretestingclub/7159412943/sizes/o/in/photostream/">Getting started with mobile testing</a>
</li>
<li><a href="http://apps.testinsane.com/mindmaps/Mobile-Testing-In-a-Nutshell">Mobile testing in a nutshell</a>
</li>
<li><a href="https://www.koreyhinton.com/blog/ios/am-i-really-done-testing.html">Am I Really Done Testing?</a>
</li>
<li><a href="http://www.testingdiaries.com/mobile-testing-checklist/">Mobile Testing Checklist</a>
</li>
<li><a href="https://www.appqualityalliance.org/files/AQuA_testing_criteria_for_Android_v1.3_oct_2_2012.pdf">Testing Criteria for Android Applications</a>
</li>
<li><a href="https://i.imgur.com/DDWnzbS.png">A mnemonic for mobile app testing</a>
</li>
<li><a href="http://www.kohl.ca/articles/ISLICEDUPFUN.pdf">Test Mobile Applications with I SLICED UP FUN!</a>
</li>
<li><a href="https://testingideas.wordpress.com/2014/08/17/mobile-app-test-coverage-model-long-fun-cup/">Mobile App Test Coverage Model : LONG FUN CUP</a>
</li>
<li><a href="https://hsto.org/getpro/habr/upload_files/079/663/f2f/079663f2fc528456afb1367b4096d266.png">Тестирование новой фичи</a>
</li>
</ul>
<h2>Основные инструменты тестировщика?</h2>
<ul>
<li>Мультитул: DevTools;
</li>
<li>Снифферы: Charles Proxy, Fiddler;
</li>
<li>Тестирование API: Postman, SoapUI;
</li>
<li>Тестирование производительности: JMeter;
</li>
<li>Тестирование безопасности: Kali linux,  Santoku Linux + drozer, OWASP ZAP, …;
</li>
<li>Тестирование UI/UX: Figma, Zeplin, любой mindmap-like продукт;
</li>
<li>Фермы устройств для тестирования мобильных приложений: BrowserStack, Xamarin, AWS;
</li>
<li><a href="https://szadorozhnyi.medium.com/%D0%B8%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F-android-%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D0%B9-%D1%87%D0%B0%D1%81%D1%82%D1%8C-1-87a6d6a9e817">Инструменты тестирования Android приложений</a>
</li>
<li>Системы контроля версий: GIT;
</li>
<li>Взаимодействие с базами данных: язык SQL, системы СУБД;
</li>
<li>Системы CI/CD: Jenkins/TeamCity;
</li>
<li>Прочее: мессенджеры, баг-трекинговые системы и TMS, генераторы тестовых данных и т.п.
</li>
</ul>

DevTools:
В каждый современный браузер встроены инструменты разработчика — они позволяют быстро отловить и исправить ошибки в разметке или в коде. С их помощью можно узнать, как построилось DOM-дерево, какие теги и атрибуты есть на странице, почему не подгрузились шрифты и многое другое:
<ul>
<li><a href="https://siteclinic.ru/blog/seo-instrumenty/seo-chrome-devtools/#2">Проверка ответа сервера</a>
</li>
<li><a href="https://siteclinic.ru/blog/seo-instrumenty/seo-chrome-devtools/#3">Проверка мобильной адаптивности</a>
</li>
<li><a href="https://siteclinic.ru/blog/seo-instrumenty/seo-chrome-devtools/#4">Проверка мобильной выдачи</a>
</li>
<li><a href="https://siteclinic.ru/blog/seo-instrumenty/seo-chrome-devtools/#5">Региональная поисковая выдача</a>
</li>
<li><a href="https://siteclinic.ru/blog/seo-instrumenty/seo-chrome-devtools/#6">Изменение дизайна</a>
</li>
<li><a href="https://siteclinic.ru/blog/seo-instrumenty/seo-chrome-devtools/#7">Анализ протокола безопасности</a>
</li>
<li><a href="https://siteclinic.ru/blog/seo-instrumenty/seo-chrome-devtools/#8">Анализ скорости загрузки страницы</a>
</li>
</ul>
<a href="https://habr.com/ru/company/ruvds/blog/486692/">Средства консоли Chrome, которыми вы, возможно, никогда не пользовались</a>
<br>
Postman:
Постман представляет собой мультитул для тестирования API. В нем можно создавать коллекции запросов, проектировать дизайн API и создавать для него моки (заглушки-имитации ответов реального сервера), настраивать мониторинг (периодическая отправка запросов с журналированием), для запросов возможно написание тестов на JS, есть собственный Runner и т.д. Однако постман сложно назвать подходящим инструментом для серьезной автоматизации ввиду сложности поддержки тестов, но при этом он хорошо подойдет в простых случаях или как инструмент поддержки а анализа: проверка работоспособности endpoint, дебаг тестов, простая передача информации о дефектах (можно сохранить запрос в curl, ответ в json и т.п.). Postman также может работать без графического интерфейса (newman).
<ul>
<li>Аналог: <a href="https://hoppscotch.io/">https://hoppscotch.io/</a>
</li>
<li><a href="https://www.youtube.com/watch?v=55l6XIEK9l0&ab_channel=QASTARTUP-ITTrainingCenter">Курс Тестирование ПО. Занятие 30. POSTMAN. Ручное тестирование API | QA START UP</a>
</li>
<li><a href="https://robertgorter.medium.com/api-testing-using-postman-87cf1c40b82c">API testing using Postman</a>
</li>
</ul>

Proxy (снифферы трафика):
Charles — инструмент для мониторинга HTTP/HTTPS трафика. Программа работает как прокси-сервер между приложением и сервером этого приложения. Charles записывает и сохраняет все запросы, которые проходят через него и позволяет их редактировать.
<ul>
<li><a href="https://habr.com/ru/company/redmadrobot/blog/269109/">Charles: незаменимый тул в арсенале QA-инженера</a>
</li>
<li><a href="https://www.youtube.com/watch?v=74v5lpOug8c&feature=youtu.be&ab_channel=BogdanOvsiyuk">Breakpoints charles proxy Подмена данных</a> 
</li>
<li><a href="https://habr.com/ru/company/youla/blog/527648/">Как приручить Charles Proxy?</a>
</li>
<li><a href="https://www.apriorit.com/dev-blog/591-proxies-for-application-testing">Using Web Debugging Proxies for Application Testing</a>
</li>
<li><a href="https://telegra.ph/Perehvat-SSL-trafika-s-Android-prilozheniya-01-26">Перехват SSL трафика с Android-приложения</a>
</li>
<li><a href="https://trykov.ru/certificate-and-public-key-pinning/">Certificate and Public Key Pinning</a>
</li>
</ul>

Тестирование безопасности:
<ul>
<li><a href="https://habr.com/ru/company/tomhunter/blog/456892/">Чем искать уязвимости веб-приложений: сравниваем восемь популярных сканеров</a>
</li>
<li><a href="https://itfb.com.ua/instrumenty-testirovaniya-bezopasnosti/">20 мощных инструментов тестирования на проникновение в 2019 году</a>
</li>
<li><a href="https://itsecforu.ru/2019/08/06/%F0%9F%92%A3-10-%D0%BB%D1%83%D1%87%D1%88%D0%B8%D1%85-%D0%B8%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D0%B2-%D1%81%D0%BA%D0%B0%D0%BD%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F/">10 лучших инструментов сканирования уязвимостей для тестирования на проникновение – 2020</a>
</li>
<li><a href="https://habr.com/ru/company/alexhost/blog/530110/">Пентест веб сайта с помощью Owasp Zap</a>
</li>
<li><a href="https://habr.com/ru/company/alexhost/blog/535396/">Проверяем безопасность приложений с помощью Drozer</a>
</li>
</ul>

GIT:
Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов. Например, для картинок - полезно для дизайнеров.
С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.
Репозиторием называют хранилище вашего кода и историю его изменений. Git работает локально и все ваши репозитории хранятся в определенных папках на жестком диске.
Так же ваши репозитории можно хранить и в интернете. Обычно для этого используют три сервиса: <a href="https://github.com/">GitHub</a>, <a href="https://bitbucket.org/">Bitbucket</a>, <a href="https://gitlab.com/">GitLab</a>
Знать команды нужно для:
"1. Если надо что-то сделать с гитом по SSH.
2. Если надо сравнить диффы огромных файлов. Vimdiff вытянет, многие тулы сдохнут или будут сильно тормозить.
3. Тулы часто тупят и работают неправильно.
4. Хорошие тулы платные)"  (с) @anton_smolianin
<br>
В любом случае, даже нажимая кнопки, требуется понимать, как это работает под капотом хотя бы на элементарном уровне.

<a href="https://t.me/qa_pro/480">Все что нужно для работы с GIT</a>
<ul>
<li><a href="https://habr.com/ru/post/541258/">Git для новичков (часть 1)</a>
</li>
<li><a href="https://habr.com/ru/company/oleg-bunin/blog/468177/">Git изнутри и на практике</a>
</li>
<li><a href="https://habr.com/ru/company/skillbox/blog/534972/">Git, я хочу все отменить! Команды исправления допущенных ошибок</a>
</li>
</ul>

SQL:
<a href="https://t.me/qa_pro/490">Все что нужно для работы с SQL</a>:
<ul>
<li>Официальные сайты
</li>
<ul>
<li><a href="https://www.sqlite.org/index.html">SQLite</a>
</li>
<li><a href="https://www.mysql.com/">MySQL</a>
</li>
<li><a href="https://www.postgresql.org/">PostgreSQL</a>
</li>
</ul>
<li>GUI клиенты
</li>
<ul>
<li><a href="https://www.mysql.com/products/workbench/">MySQL Workbench</a>
</li>
<li><a href="https://www.heidisql.com/">HeidiSQL</a>
</li>
<li><a href="https://www.navicat.com/en/products/navicat-for-mysql">Navicat for MySQL</a>
</li>
<li><a href="https://www.devart.com/dbforge/mysql/studio/">dbForge Studio for MySQL</a>
</li>
</ul>
<li> Основы SQL 
</li>
<ul>
<li><a href="https://www.amazon.com/Learning-SQL-Generate-Manipulate-Retrieve/dp/1492057614/ref=sr_1_1?dchild=1&keywords=sQL&qid=1613292997&s=books&sr=1-1">Алан Бьюли "Изучаем SQL"</a>
</li>
<li><a href="https://www.amazon.com/Head-First-SQL-Brain-Learners/dp/0596526849/ref=sr_1_10?dchild=1&keywords=sQL&qid=1613292997&s=books&sr=1-10">Линн Бейли "Изучаем SQL"</a>
</li>
<li><a href="https://www.w3schools.com/sql/sql_intro.asp">W3C Introduction to SQL</a>
</li>
<li><a href="https://www.guru99.com/sql.html">guru99 | SQL Tutorial for Beginners: Learn SQL in 7 Days</a>
</li>
</ul>
<li>Продвинутый уровень
</li>
<ul>
<li><a href="https://www.amazon.com/SQL-Cookbook-Query-Solutions-Techniques/dp/1492077445/ref=sr_1_2?dchild=1&keywords=sQL&qid=1613292997&s=books&sr=1-2">Энтони Молинаро "SQL. Сборник рецептов"</a>
</li>
<li><a href="https://www.amazon.com/SQL-Bible-Alex-Kriegel/dp/0470229063/ref=sr_1_1?dchild=1&keywords=sQL+bible&qid=1613293063&s=books&sr=1-1">Алекс Кригель "SQL. Библия пользователя"</a>
</li>
<li><a href="https://www.amazon.com/SQL-Complete-Reference-James-Groff-dp-0071592555/dp/0071592555/ref=mt_other?_encoding=UTF8">Джеймс Грофф, Пол Вайнберг, Эндрю Оппель "SQL Полное руководство. Третье издание." </a>
</li>
</ul>
<li>Практика
</li>
<ul>
<li><a href="https://sql-academy.org/ru">SQLAcademy | Онлайн тренажер с упражнениями по SQL</a>
</li>
<li><a href="https://sqlbolt.com/">SQLBolt | Introduction to SQL</a> 
</li>
<li><a href="https://www.w3schools.com/sql/trysql.asp?filename=trysql_op_in">W3C | The Try-SQL Editor</a>
</li>
<li><a href="https://www.hackerrank.com/domains/sql">HackerRack SQL</a>
</li>
<li><a href="https://www.sql-ex.ru/?Lang=0">Упражнения по SQL</a>
</li>
<li><a href="https://www.learnqa.ru/sql_test">Тест на знание SQL</a>
</li>
<li><a href="https://www.db-fiddle.com/">https://www.db-fiddle.com/</a>
</li>
</ul>
<li>Shit happens
</li>
<ul>
<li><a href="http://www.sqltutorial.org/wp-content/uploads/2016/04/SQL-cheat-sheet.pdf">SQL Cheat Sheet</a>
</li>
<li><a href="https://tproger.ru/translations/sql-recap/">Основные команды SQL, которые должен знать каждый программист</a> 
</li>
<li><a href="https://tproger.ru/articles/sql-interview-questions/">27 распространенных вопросов по SQL с собеседований и ответы на них </a>
</li>
</ul>
</ul>

Mind maps:
<ul>
<li><a href="https://presium.pro/blog/software_for_maindmapping">12 программ и сервисов для создания майндкарт</a>
</li>
<li><a href="http://okiseleva.blogspot.com/2020/01/mind-map.html">Как нарисовать карту приложения (mind map)</a>
</li>
<li><a href="https://habr.com/ru/company/badoo/blog/418353/">Mind map вместо тест-кейса, или Как визуализация позволяет тестировать приложение быстрее</a>
</li>
<li><a href="https://habr.com/ru/post/539756/">Mind Map в помощь тестировщику</a>
</li>
<li><a href="https://habr.com/ru/post/515990/">Mind Map в тестировании — или легкий способ тестировать сложные приложения</a>
</li>
</ul>

TMS:
<a href="https://habr.com/ru/post/522474/">Топ-12 лучших систем управления тестированием 2020</a>

<h2>Как вообще происходит процесс найма?</h2>
Все зависит от компании и в меньшей степени от уровня позиции. В среднем это выглядит так:
<ol>
<li>Отклик на вакансию;
</li>
<li>*Опционально: выполнение тестового задания, п.2 и п.3 могут меняться местами;
</li>
<li>Скрининг по телефону (небольшая беседа с HR);
</li>
<li>Полноценное собеседование с HR;
</li>
<li>Техническое собеседование, п.4 и п.5 иногда делают за раз;
</li>
<li>*Опционально: собеседование с боссом;
</li>
</ol>
<h2>Качества, которыми нужно обладать тестировщику?</h2>
<ul>
<li>Развитые софт-скиллы (например, уметь в коммуникацию, не перебивать собеседника и т.п.);
</li>
<li>Общая грамотность;
</li>
<li>Умение обучаться;
</li>
<li>Пытливый ум и желание выяснить первопричину проблемы;
</li>
<li>Устойчивость к рутине;
</li>
</ul>

Доп. материал: 
<a href="https://telegra.ph/Mif-ob-obraze-myshleniya-v-testirovanii-02-10">Миф об образе мышления в тестировании</a>
<h2>Как составить резюме?</h2>
Кратко о базовых рекомендациях.
Резюме стажера или джуниора – ровно 1 страница (имеется в виду вариант в файле, а не на площадках). Помимо PDF желательно иметь вордовскую копию на google-диске. Язык резюме – русский, если нацелены на компании из РФ с клиентами из РФ. В остальных случаях – английский. Лучший вариант оформления шапки:
<img src="https://lh3.googleusercontent.com/IxmsFBh0Fdl1QXs9nyvBCCmYHFHONqHO_iVQvfHg_ychWksh2QAJoEib1q-oM5GIfbT_nWXHNiMdEXJLpRHXVe-pl55D12BZWQKAk-UAfqX7Ytw76crI4_EV0s9C2c0zvsBaePp8">
Просто нормальное фото, ФИО, на какую позицию претендуете, опционально локация и дата рождения, актуальные контакты.
После чего идет раздел с опытом работы (любые практические навыки), где максимально кратко и емко описывается чем конкретно вы занимались. Это самая важная часть резюме. Общее правило - использовать глаголы совершенного вида (сделал то, там-то; а делал, участвовал - ничего о вас не говорит), а еще лучше в формате «зона ответственности + достижения»
Следом – образование и затем ключевые навыки. Не забудьте упомянуть знание иностранных языков. Сориентироваться поможет, например, бесплатный тест EFSET с сертификатом. Никогда не используйте банальные ключевые навыки «ответственный, целеустремленный, …». Только конкретика. Помните, что HR часто ищут по ключевым словам, а вы не должны раздувать ваше резюме всяким мусором. Технологии, инструменты – хороший выбор. Но будьте готовы, что вас по ним детально будут спрашивать в первую очередь.
Раздел «О себе» можно включить, если есть что важного и интересного написать, опять же, коротко и если есть чем выделиться. 
При отклике на вакансию встает вопрос о сопроводительном письме и мне понравилось это мнение:
[Переслано от Vincent Jozeph Mousekewitz] (@V_J_Mousekewitz)
"Рассматривайте свое резюме как коммерческое предложение, а сопроводительное письмо -- как быстрый и понятный ответ на вопрос "почему я должен рассмотреть детальнее именно Ваше предложение". 
Сопроводительные письма почти всегда читают. Другой вопрос, что они почти всегда написаны плохо, сухо и "не цепляют", что автоматически идет в минус. Если не хотите/не можете/не готовы в эпистолярный жанр -- не пишите. Переформатируйте резюме, чтобы за 30 секунд чтения было понятно, какую боль Вы готовы снять заказчику(работодателю) и какими квалификациями для этого обладаете. 
Сопроводительные -- тоже, в каком-то смысле "инструмент". Не надо их писать "чтобы было", такое отношение видно сразу и не играет на руку кандидату.
Однако, если есть "что сказать" -- не держите в себе. Увидели вакансию, считаете себя идеальным кандидатом и готовы аргументировать -- вперед."

Вообще на тему составления резюме в IT есть миллион статей (<a href="https://hurma.work/rf/blog/idealnoe-rezyume-kandidata-mif-ili-realnost-2/">пример</a>) и видео на youtube, да и не стоит исключать фактор личных пристрастий нанимателя, так что следует просто ознакомиться с базовыми рекомендациями, при желании скинуть итоговый вариант на оценку в коммьюнити и заняться более насущными вопросами.
Насчет самих откликов, тут на мой взгляд уместна аналогия с холодными звонками, т.е. не нужно на начальном этапе выбирать место работы так, будто собираетесь в ней состариться. Вообще слать резюме стоит не только откликаясь на вакансии. Есть мнение, что когда компания уже выкинула вакансию на работные сайты, это уже тупик (т.к. не нашли кандидата по своим каналам). Шлите на почты компаний, HR-ов, расширяйте сеть контактов в linkedin и т.п.. Слышал, что активные джуны рассылали по несколько сотен писем в неделю. Стоит ли говорить, что они быстро нашли свою первую работу?

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/post/470684/">Что писать в резюме, если нет опыта работы</a>
</li>
<li><a href="https://habr.com/ru/post/542952/">Инхаус, фриланс, аутсорс компания: куда приземлиться тестировщику, чтобы не разлюбить профессию и расти как на дрожжах</a>
</li>
</ul>
<h2>Как проходить собеседование?</h2>
Прежде всего, конечно, на него не нужно опаздывать. Стоит прийти немного заранее, оглядеться, привыкнуть к атмосфере и настроиться на нужный лад.
Главное, что нужно сказать о собеседованиях – на них надо ходить. Регулярно. Это отдельный навык, который утрачивается если не практиковать. Не стоит бояться и относиться к ним как к экзамену, вы и сами это поймете на практике. В знаниях это скорее это как калибровка, нахождение ориентира где вы сейчас находитесь и в какую сторону корректировать курс. Прошли – проанализировали – подкачались – повторяете, пока не будет достигнут приемлемый результат. Некоторые советуют даже после устройства на работу периодически ходить на собеседования, чтобы держать этот навык в тонусе и ориентироваться в своей ценности на рынке. 
Если вы ищете первую работу, начать ходить на собеседования нужно как можно раньше еще и потому, что никто не задумывается, как долго в реальности может занять процесс поиска работы. Сначала нужно будет выбить себе возможность пройти интервью. Цифры примерно такие: 10 откликов на подходящие вакансии или 100 рассылкой = 1 собес. 10 не заваленных собесов = 1 оффер. Принятие решения компанией может занимать пару недель. В некоторых компаниях этапов может быть штук до 6. Средне-оптимистичный сценарий предполагает от 2-3 месяцев с нуля до начала работы, но это в случае наличия вокруг выбора и хорошей подготовки у кандидата (а на этот счет тоже многие заблуждаются). В не идеальном случае процесс займет от полугода.
Основное, что хочется сказать про само собеседование:
Узнай о компании, в которую идешь проходить собеседование.
Не скромничай и не занижай свои навыки. Ты, возможно, 50-й кандидат на этой неделе и еще 100 будет после тебя. Если будешь мяться – про тебя забудут, как только ты закроешь за собой дверь. Здоровая гипербола и немного красок еще никому не мешали. Но никогда не переходи в ложь.
Потренируйтесь в самопрезентации, записывая себя на видео и пересматривая. Обычно первое, что вас спросят – «расскажите о себе». Основная задача HR – проверить адекватность кандидата, в некоторых случаях еще соответствие определенному заказу из целевой команды (от возраста до хобби, все что угодно). Помните, что собеседуют в компанию в первую очередь человека, а уже потом специалиста. Кто-то сравнивает собеседование со свиданием, где за час вы должны понять, подходите ли вы друг другу. Вопросы на этом этапе в основном стандартные, ответы на них лучше расписать заранее, но не заучивать. Заученный ответ обычно выглядит нелепо, а вот сформулировать свои мысли заранее и понять себя бывает полезно.
Хороший базовый рассказ о себе определит дальнейший ход собеседования, HR будет копать вглубь от заинтересовавших фактов. Кстати, не на все вопросы вы будете знать ответ и это нормально. Одна из задач рекрутера проверить, как вы себя ведете и как отвечаете, когда не знаете ответ. Или вас попробуют заставить сомневаться в заведомо правильном ответе (в этот момент вы вспомните передачу "кто хочет стать миллионером"). Умение грамотно отстаивать свою точку зрения очень важно для тестировщика. 
Еще хороший совет - всё, что вы скажете, может и будет использовано против вас. В том смысле, что не говорите лишнего или того, в чем плаваете, иначе очень быстро закопаетесь в новых вопросах.
В конце (хотя бывает и в начале) спрашивает собеседуемый! Помните, что это обоюдный процесс? Они выбирают себе кандидата, но и вы выбираете себе компанию. Немного информации для борьбы со стеснением: для компании найм сотрудника очень затратная затея. В крупных компаниях даже есть бонусы сотрудникам за удачную рекомендацию знакомого в размере тысяч 100 и это в контексте затрат на обычный процесс найма просто копейки. Обе стороны заинтересованы закрыть торги прямо здесь и сейчас, так что не бойтесь задавать вопросы и будьте полноценной второй стороной в этих переговорах.
По поводу спросить – вот безжалостный копипаст (есть мнение, что если все это начнет спрашивать начинающий специалист, то на это покрутят у виска. Просто умело и ненавязчиво вплетайте самое важное для вас в беседу и все будет ок):
<ul>
<li>Официальное ли оформление, тип. Белая ли заработная плата? Предусмотрены ли премии?
</li>
<li>Есть ли KPI, что в них входит?
</li>
<li>Какой график работы, как происходят отработки?
</li>
<li>Как часто бывают переработки и оплачиваются ли они?
</li>
<li>Время начала рабочего дня и отношение к опозданиям?
</li>
<li>Схема карьерного роста, матрица компетенций, период и порядок пересмотра з.п.?
</li>
<li>Приветствуется ли инициатива и если нет, насколько она наказуема?
</li>
<li>Есть ли командировки, какие направления и как часто?
</li>
<li>Что входит в социальный пакет и когда он предоставляется?
</li>
<li>Если работа удаленная или частично удаленная — какая техника предоставляется?
</li>
<li>Как организовано рабочее место, что в него входит? Опенспейс или кабинет?
</li>
<li>Есть ли наставничество или менторство в первое время работы в компании?
</li>
<li>Практикуется ли компенсация обучения, заинтересован ли работодатель в сертификации, участии сотрудника в митапах, конференциях и т.п.?
</li>
<li>Как осуществляется контроль за сотрудниками: есть ли тайм-трекеры, камеры и т. д.?
</li>
<li>Наличие спортзала, столовой, душа?
</li>
<li>Наличие библиотеки с актуальной литературой?
</li>
</ul>

Если на собеседовании несколько иерархически подчиненных человек (HR и директор, начальник отдела и директор или топ-менеджер), обратите внимание на модель их общения, на то, слаженно ли они работают, есть ли контакт или же только благоговейное молчание. Команду видно издалека.
<ul>
<li>Как отнеслись к вашему резюме: оно одно из многих и вы здесь «на потоке» или оно лежит одно, и вы в фокусе.
</li>
<li>Как распределено время на собеседование и часто ли отвлекаются его участники, вовремя ли начато общение или вам пришлось ждать больше 15 минут.
</li>
<li>Как вам представили руководителя — с регалиями или нет, по имени-отчеству или имени, формально или неформально. 
</li>
<li>Как отнеслись к ходу решения вами заданий — как к экзамену или как к деловому обсуждению задачи. Это говорит о вашем уровне в глазах собеседующего.
</li>
</ul>

Собеседование на английском языке практическое такое же*, просто из-за языкового барьера могут возникать трудности. Практикуйтесь! И помните, что вашему собеседнику может быть так же трудно, как и вам.
*- при собеседовании в другую страну следует учитывать культурные особенности (да и законодательство), потому что некоторые ценности и взгляды могут совершенно не очевидным образом быть разными и при этом иметь решающее значение. Здесь нужно целенаправленно читать статьи о найме или релокации в интересующую страну, там упоминаются эти нюансы и особенности.
Доп. материал:
<ul>
<li><a href="https://habr.com/ru/post/477354/">Вопросы для собеседования — от кандидата к работодателю</a>
</li>
<li><a href="https://habr.com/ru/post/470227/">Как собеседовать работодателя?</a>
</li>
<li><a href="https://habr.com/ru/post/513524/">О чем поговорить на собеседовании с выпускником онлайн-курсов по тестированию</a>
</li>
<li><a href="https://habr.com/ru/company/headzio/blog/529384/">Как QA найти «ту самую» компанию и стать тимлидом</a>
</li>
<li><a href="https://habr.com/ru/company/gms/blog/527916/">Собеседование для QA: резюме, вопросы на интервью, переговоры о зарплате + полезные ссылки</a>
</li>
<li><a href="https://habr.com/ru/company/mailru/blog/522326/">Сценарий идеального технического собеседования</a>
</li>
<li><a href="https://habr.com/ru/post/431514/">Собеседование для собеседующих</a>
</li>
<li><a href="https://github.com/kix/reverse-interview/blob/master/README.md">Обратное собеседование</a>
</li>
<li><a href="https://www.linkedin.com/pulse/%D1%87%D0%B5%D0%BA-%D0%BB%D0%B8%D1%81%D1%82-%D0%B4%D0%BB%D1%8F-%D0%BF%D0%BE%D0%B4%D0%B3%D0%BE%D1%82%D0%BE%D0%B2%D0%BA%D0%B8-%D0%BA-%D1%81%D0%BE%D0%B1%D0%B5%D1%81%D0%B5%D0%B4%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8E-%D0%BD%D0%B0-%D0%B0%D0%BD%D0%B3%D0%BB%D0%B8%D0%B9%D1%81%D0%BA%D0%BE%D0%BC-mashtalyar/">Чек-лист для подготовки к собеседованию на английском</a> (linkedin, в РФ нужен VPN/proxy)
</li>
</ul>
<h2>Ошибки в работе у начинающих тестировщиков?</h2>
<ul>
<li>Во всем видят дефекты. Как избежать:
</li>
<ul>
<li>Внимательно анализировать требования
</li>
<li>Владеть информацией о том, как должен работать продукт
</li>
<li>Если сомневаешься, что это дефект – спроси БА или ответственного
</li>
<li>Несколько раз перепроверь прежде чем регистрировать дефект
</li>
</ul>
<li>Пытаются сразу все сломать. Как избежать:
</li>
<ul>
<li>Начинать тестирование только с положительных тестов
</li>
<li>Акцентировать внимание на том, что в приоритете для заказчика
</li>
<li>Не проверять редкие сценарии в первую очередь
</li>
</ul>
<li>Боятся задавать вопросы. Как избежать:
</li>
<ul>
<li>Начать понимать, что коммуникация это важная и неотъемлемая часть работы
</li>
</ul>
<li>Не интересуются, кто и за что отвечает, как устроены процессы. Как избежать:
</li>
<ul>
<li>Узнать у ПМ об областях ответственности каждого члена команды
</li>
<li>Узнать у ПМ о всех процессах на проекте
</li>
</ul>
<li>Паникуют при малейшей трудности. Как избежать:
</li>
<ul>
<li>Без паники, п. 3 и 4 помогут разобраться
</li>
</ul>
<li>Пытаются применить сразу все, что изучили. Как избежать:
</li>
<ul>
<li>Помнить, что у каждого вида тестирования своя цель
</li>
<li>Бюджет всегда ограничен, расставлять приоритеты
</li>
</ul>
<li>Задают один и тот же вопрос несколько раз
</li>
<li>Дёргают разработчиков по каждой мелочи (прерывают состояние потока, контекст. Разработка требует держать огромное количество абстракций в голове во время работы над задачей. Это очень легко сбить элементарным вопросом, который находится в первой строчке поисковой выдачи)
</li>
</ul>

Доп. материал:
<ul>
<li><a href="https://red-foks.medium.com/%D0%BA%D0%B0%D0%BA-%D0%B2%D1%8B%D0%B6%D0%B8%D1%82%D1%8C-%D0%BD%D0%B0-%D0%BD%D0%BE%D0%B2%D0%BE%D0%B9-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B5-%D0%B8%D0%BB%D0%B8-%D0%BE%D0%BD%D0%B1%D0%BE%D1%80%D0%B4%D0%B8%D0%BD%D0%B3-%D1%81%D0%BD%D0%B8%D0%B7%D1%83-8e95c7c4ac0c">Как выжить на новой работе или онбординг снизу</a>
</li>
<li><a href="https://telegra.ph/SHest-test-person-s-kotorymi-ne-stoit-imet-dela-01-02">Шесть тест-персон, с которыми не стоит иметь дела</a>
</li>
<li><a href="https://ru.hexlet.io/blog/posts/shest-podskazok-novichku-v-testirovanii">Лучше не знать и спросить, чем притворяться, что знаешь, или Шесть подсказок новичку в тестировании</a>
</li>
<li><a href="https://abilmazhinova.medium.com/%D0%BC%D0%BE%D0%B8-3-%D0%BE%D1%88%D0%B8%D0%B1%D0%BA%D0%B8-%D0%BA%D0%BE%D1%82%D0%BE%D1%80%D1%8B%D0%B5-%D1%8F-%D1%81%D0%BE%D0%B2%D0%B5%D1%80%D1%88%D0%B0%D0%BB%D0%B0-%D0%BA%D0%B0%D0%BA-junior-qa-engineer-10290234e949">Мои 3 ошибки, которые я совершала как junior QA engineer</a>
</li>
</ul>
<h2>Я – единственный тестировщик на проекте. Что делать?</h2>

<img src="https://lh3.googleusercontent.com/YAepXPiV4qhlJogC3O2wL6e39cwsXb4EmTJT-Wg6esjKnh-ImTO4gwtiFIis9EQBonDnMBd3-TmeNvulahKrJIWma63Z38NFoXg0P2p13XtPUTR0RoXxrnitP1i-BjCv2-cLnBo0">
Начинать знакомство с проектом лучше с интервью. Станьте журналистом. Что из себя представляет структура организации, а именно кто над кем стоит и кто за что отвечает? Где больше всего багов, каким видят тестирование сейчас и какие ожидания в будущем? Оцените зрелость процессов по CMM и TMM, зрелость проекта (новый/старый-зрелый/старые-зрелые где будут глобальные изменения) и команды, определите методологию разработки. Проведите вводную лекцию команде: что такое QA, как оно может помочь, с какими проблемами обращаться и зачем вообще оно надо. Далее в зависимости от всего этого ищем и смотрим соответствующий вебинар/статью и т.п., в крайнем случае можно поинтересоваться у коллег в тематических сообществах, например, в tg. Вообще создавать отдел тестирования обычно нанимают QA Lead, а если вы джун, то либо работодатель не понимает что делает, ожидая от джуниора построения процессов, о которых он в лучшем случае где-то читал, либо от вас хотят чего-то вполне конкретного и проводить целое расследование не придется - наверняка все объяснят еще на собеседовании. В нормальной ситуации вы проведете исследовательское тестирование, составите набор кейсов, задокументируете все текущие баги и в дальнейшем будете заниматься тестированием новых сборок, проверкой исправления найденных дефектов и проведением регрессии. 

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/post/439128/">Как организовать работу QA. Один практически примененный способ</a>
</li>
<li><a href="https://habr.com/ru/post/467109/">Как QA организовать автоматизацию тестирования на проекте. Один практически примененный способ</a>
</li>
<li><a href="https://habr.com/ru/post/471576/">Как QA выстроить эффективное взаимодействие с разработчиками. Один возможный путь</a>
</li>
<li><a href="https://www.youtube.com/watch?v=RAC1bjWzIVk&ab_channel=FestGroup">Никогда такого не было и вот опять: Построение отдела тестирования - Андрей Мясников. QA Fest 2018</a>
</li>
<li><a href="https://www.youtube.com/watch?v=54JtRR4GbPQ&ab_channel=FestGroup">Процесс: как наладить, а не нагадить - Андрей Мясников. QA Fest 2015</a>
</li>
<li><a href="https://www.youtube.com/watch?v=4KT_ouolMQs&ab_channel=KatyaKravchenkoUSLife">Как проходит организация тестирования и составление тест планов (в зависимости от проекта)</a>
</li>
<li><a href="https://www.youtube.com/watch?v=UW8sTq8SuFQ&feature=emb_logo&ab_channel=LuxoftTrainingCenter">Концепция построения процесса тестирования в Agile-проектах: 3+1</a>
</li>
<li><a href="https://www.youtube.com/watch?v=POYyrqpbr94&feature=emb_logo&ab_channel=VladislavOrlikov">Построение процессов тестирования на новом проекте</a>
</li>
<li><a href="https://www.youtube.com/watch?v=qiCjqqtWP7I&t=790s">Мифы о тестировании #2 / О чем не говорят на курсах по тестированию / Правда о работе в IT</a>
</li>
<li> <a href="https://dou.ua/lenta/columns/value-driven-testing/">Что нужно знать о Value Driven Testing. Анализируем ценность и экономическую целесообразность тестирования</a>
</li>
</ul>


<h1>----- HR-часть -----</h1>
<h2>Вопросы с реальных собеседований с этапа HR </h2>
Часть из них зададут в любом случае. Список, разумеется, не полный:
<ul>
<li>Расскажи о себе (все что хочешь, что нам нужно знать о тебе)
</li>
<li>Есть ли релевантный опыт?
</li>
<li>Какие курсы проходил и вообще, что изучал?
</li>
<li>Что не устраивало на прошлом месте работы (если было), особенно если решил сменить сферу?
</li>
<li>Почему выбрал именно тестирование?
</li>
<li>Чем заинтересовала именно наша компания?
</li>
<li>Как часто бываешь на собеседованиях?
</li>
<li>Уровень английского? (вопрос могут задать на английском, многие теряются в этот момент)
</li>
<li>(Если требуется и уровень хороший) расскажите на английском: как доехали до собеседования/о себе (только не как в обществе анонимных алкоголиков) /почему считаешь, что можешь стать тестировщиком/ как прошел вчерашний день/о своих хобби/ и т.п.
</li>
<li>Как в целом смотришь на мир, как решаешь возникающие проблемы?
</li>
<li>3 твоих сильных и 3 слабых стороны?
</li>
<li>Как отдыхаешь? Как проводишь свободное время?
</li>
<li>Какие хобби?
</li>
<li>Что последнее прочитал техническое? Не техническое?
</li>
<li>Если бы мог вернуться в начало осознанной жизни, выбрал бы иной карьерный путь?
</li>
<li>3 примера, что тебе положительного дал предыдущий опыт работы (если есть)
</li>
<li>3 плюса и 3 минуса в сфере тестирования лично для тебя
</li>
<li>Как видишь развитие в этой сфере, кем видишь себя через год, три?
</li>
<li>Какая-то одна вещь или ситуация, которой ты гордишься
</li>
<li>Представим, что остальных кандидатов много и они опытнее (обычно так и есть), может у тебя есть какие-то преимущества перед ними? Почему ты думаешь, что лучше других кандидатов?
</li>
<li>Зарплатные ожидания сейчас, после испытательного срока, через год?
</li>
<li>Есть ли какие-то факторы, с которыми ты согласишься на меньшие деньги?
</li>
<li>С чем точно не готов мириться в отношении компании или руководителя?
</li>
<li>Ожидания от работы?
</li>
<li>Отношение к переработкам?
</li>
<li>Представь, что ты работаешь уже полгода. Опиши свой рабочий день.
</li>
<li>Что если при выполнении задачи понимаешь, что не укладываешься в сроки?
</li>
</ul>
<h1>----- Теоретическая часть -----</h1>

<h1>Общие понятия</h1>
<h2>Что означает тестирование ПО?</h2>
Тестирование (testing) программного обеспечения  - с технической точки зрения заключается в выполнении приложения (Application Under Testing (AUT) или Implementation Under Testing (IUT)) на некотором множестве исходных данных и сверке получаемых результатов с заранее известными (эталонными) с целью установить соответствие различных свойств и характеристик приложения заказанным свойствам. Как одна из основных фаз процесса разработки программного продукта (Дизайн приложения - Разработка кода - Тестирование ), тестирование характеризуется достаточно большим вкладом в суммарную трудоемкость разработки продукта. Широко известна оценка распределения трудоемкости между фазами создания программного продукта: 40%-20%-40%, из чего следует, что наибольший эффект в снижении трудоемкости может быть получен прежде всего на фазах Design и Testing. В более широком смысле, тестирование ПО - это техника контроля качества программного продукта, включающая в себя проектирование тестов, выполнение тестирования и анализ полученных результатов.
<h2>Почему требуется тестирование ПО?</h2>
<ul>
<li>Процесс тестирования гарантирует, что ПО будет работать в соответствии с ожиданиями клиентов и на имеющемся у них оборудовании.
</li>
<li>Это уменьшает циклы кодирования, выявляя проблемы на начальном этапе разработки. Обнаружение проблем на более ранних этапах SDLC обеспечивает правильное использование ресурсов и предотвращает повышение стоимости.
</li>
<li>Команда тестирования привносит взгляд клиента в процесс и находит варианты использования, о которых разработчик может не подумать.
</li>
<li>Любой сбой, дефект или ошибка, обнаруженные клиентом в готовом продукте, нарушают доверие к компании.
</li>
</ul>
<h2>Что означает обеспечение качества (Quality Assurance - QA) при тестировании ПО?</h2>
Это совокупность мероприятий, охватывающих все технологические этапы разработки, выпуска и эксплуатации ПО и информационных систем, предпринимаемых на разных стадиях жизненного цикла ПО, для обеспечения требуемого уровня качества выпускаемого продукта.
Доп. материал: <a href="https://habr.com/ru/company/badoo/blog/496452/">QA — специалист по пожарной безопасности вашего проекта</a>
<h2>Что означает контроль качества (Quality Control - QC) при тестировании ПО?</h2>
Это подмножество QA, совокупность действий, проводимых над продуктом в процессе разработки, для получения информации о его актуальном состоянии и соответствии ожидаемым результатам.
<h2>Что означает качество ПО? (Software Quality)</h2>
Качеству очень сложно дать неформальное определение, оно заключается в соответствии требованиям (conformance to requirements) и пригодности к использованию (fitness for use). Качество программного продукта характеризуется набором свойств, определяющих, насколько продукт "хорош" с точки зрения заинтересованных сторон, таких как заказчик продукта, спонсор, конечный пользователь, разработчики и тестировщики продукта, инженеры поддержки, сотрудники отделов маркетинга, обучения и продаж. Каждый из участников может иметь различное представление о продукте и о том, насколько он хорош или плох, то есть о том, насколько высоко качество продукта. То есть, основная последовательность действий при выборе и оценке критериев качества программного продукта включает:
<ul>
<li>Определение всех лиц, так или иначе заинтересованных в исполнении и результатах данного проекта.
</li>
<li>Определение критериев, формирующих представление о качестве для каждого из участников.
</li>
<li>Приоритезацию критериев, с учетом важности конкретного участника для компании, выполняющей проект, и важности каждого из критериев для данного участника.
</li>
<li>Определение набора критериев, которые будут отслежены и выполнены в рамках проекта, исходя из приоритетов и возможностей проектной команды. Постановка целей по каждому из критериев.
</li>
<li>Определение способов и механизмов достижения каждого критерия.
</li>
<li>Определение стратегии тестирования исходя из набора критериев, попадающих под ответственность группы тестирования, выбранных приоритетов и целей.
</li>
</ul>
Доп. материал:
<ul>
<li><a href="https://analytics.infozone.pro/software-quality/">https://analytics.infozone.pro/software-quality/</a>
</li>
<li><a href="https://www.intuit.ru/studies/courses/48/48/lecture/1440?page=1">https://www.intuit.ru/studies/courses/48/48/lecture/1440?page=1</a>
</li>
<li><a href="https://habr.com/ru/company/otus/blog/471080/">Кто несет ответственность за качество тестирования приложения? 10 причин попадания ошибки в продакшен</a>
</li>
<li><a href="https://habr.com/ru/company/otus/blog/537554/">На ком лежит ответственность за качество программного обеспечения?</a>
</li>
<li><a href="https://www.softwaretestinghelp.com/coq-cost-of-quality-tutorial/">What Is Cost Of Quality (COQ): Cost Of Good And Poor Quality</a>
</li>
</ul>
<h2>Объясните отличия в QA, QC и тестировании</h2>
<img src="https://lh6.googleusercontent.com/iuHyNeCGiFo1LRWXSdLStodw1wvg1cJwGEOYpUi8fThHJbIfXsAOMBRx-FaTFbGQJYO23io_U_X5uftxxggNDj5rkl17JVC0-nPk-8PtIBbUoRFx3cuFBgWq7lcoJYBbglENXJ2A">

<h2>Разница между верификацией и валидацией? (Verification и Validation)</h2>
<ul>
<li>Верификация — это процесс включающий в себя проверку Plans, Requirement Specifications, Design Specifications, Code, Test Cases, Check-Lists, etc.
</li>
<li>Верификация всегда проходит без запуска кода.
</li>
<li>Верификация использует методы — reviews, walkthroughs, inspections, etc.
</li>
<li>Верификация отвечает на вопрос "Делаем ли мы продукт правильно?"
</li>
<li>Верификация поможет определить, является ли программное обеспечение высокого качества, но оно не гарантирует, что система полезна. Проверка связана с тем, что система хорошо спроектирована и безошибочна.
</li>
<li>Верификация происходит до Validation.
</li>
</ul>
Она содержит все активности которые позволяют достигнуть высокого качества программного обеспечения:
<ol>
<li>Inspection in software engineering, refers to peer review of any work product by trained individuals who look for defects using a well defined process. (Fagan inspection)
</li>
<li>Walkthroughs In software engineering, a walkthrough or walk-through is a form of software peer review «in which a designer or programmer leads members of the development team and other interested parties go through a software product, and the participants ask questions and make comments about possible errors, violation of development standards, and other problems».
</li>
<li>Reviews In software development, peer review is a type of software review in which a work product (document, code, or other) is examined by its author and one or more colleagues, in order to evaluate its technical content and quality.
</li>
</ol>
Валидация (validation) – это процесс оценки конечного продукта, необходимо проверить, соответствует ли программное обеспечение ожиданиям и требованиям клиента. Это динамический механизм проверки и тестирования фактического продукта.
<ul>
<li>Валидация всегда включает в себя запуск кода программы.
</li>
<li>Валидация использует методы, такие как тестирование Black Box, тестирование White Box и нефункциональное тестирование.
</li>
<li>Валидация отвечает на вопрос "Делаем ли мы правильный продукт?"
</li>
<li>Валидация проверяет, соответствует ли программное обеспечение требованиям и ожиданиям клиента.
</li>
<li>Валидация может найти ошибки, которые процесс Verification не может поймать.
</li>
<li>Валидация происходит после Verification.
</li>
</ul>
На практике, отличия верификации и валидации имеют большое значение: заказчика интересует в большей степени валидация (удовлетворение собственных требований); исполнителя, в свою очередь, волнует не только соблюдение всех норм качества (верификация) при реализации продукта, а и соответствие всех особенностей продукта желаниям заказчика.

<table>
<tr>
<td>Верификация
</td><td>Валидация
</td></tr>
<tr>
<td>По факту отвечает на вопрос, правильно ли создается и тестируется ПО и все ли требования учитываются при этом.
</td><td>Отвечает на вопрос, создается ли продукт правильно с точки зрения ожиданий клиента.
</td></tr>
<tr>
<td>В процессе верификации убеждаемся в том, что весь созданный функционал приложения работает корректно и логически верно.
</td><td>При процессе валидации убеждаемся в том, что продукт полностью соответствует поведению, которое от него ожидается и то, что клиент знает о наличии подобного функционала.
</td></tr>
<tr>
<td>В структуру верификации входят такие компоненты, как сверка завалидированным требованиям, технической документации и корректное выполнения программного кода на любом этапе создания и тестирования ПО.
</td><td>Валидация, по своей сути, в большей степени включает в себя общую оценку ПО и может основываться исключительно на субъективном мнении касательно правильности работы приложения или его компонентов.
</td></tr>
</table>

Источник: <a href="https://qalight.ua/ru/baza-znaniy/verifikatsiya-i-validatsiya/">Верификация и валидация</a>
Доп. материал:
<ul>
<li><a href="https://software-testing.ru/forum/index.php?/topic/979-verification-validation-chto-eto-takoe/">Большое обсуждение: Verification & Validation - что это такое?</a>
</li>
<li><a href="https://testmatick.com/ru/validatsiya-i-verifikatsiya-ponyatiya-shodstva-i-otlichiya/">Чем отличается валидация от верификации</a>
</li>
</ul>
<h2>Принципы тестирования?</h2>
<ul>
<li>Тестирование демонстрирует наличие дефектов
</li>
<li>Исчерпывающее тестирование недостижимо
</li>
<li>Раннее тестирование
</li>
<li>Скопление/кластеризация дефектов
</li>
<li>Парадокс пестицида
</li>
<li>Тестирование зависит от контекста
</li>
<li>Заблуждение об отсутствии ошибок
</li>
<li>Garbage in, garbage out (GIGO)
</li>
</ul>

Принцип 1. Тестирование показывает наличие дефектов
Тестирование может показать, что дефекты присутствуют, но не может доказать, что дефектов нет.
Сколько бы успешных тестов вы не провели, вы не можете утверждать, что нет таких тестов, которые не нашли бы ошибку. Но если мы нашли хотя бы один дефект, мы уже можем утверждать, что в данном ПО присутствуют дефекты.

Принцип 2. Исчерпывающее тестирование невозможно
Вместо попыток «протестировать все» нам нужен некий подход к тестированию (стратегия), который обеспечит правильный объем тестирования для данного проекта, данных заказчиков (и других заинтересованных лиц) и данного продукта. При определении, какой объем тестирования достаточен, необходимо учитывать уровень риска, включая технические риски и риски, связанные с бизнесом, и такие ограничения проекта как время и бюджет. Оценка и управление рисками – одна из наиболее важных активностей в любом проекте. 

Принцип 3. Раннее тестирование
Тестовые активности должны начинаться как можно раньше в цикле разработки и быть сфокусированы на определенных целях.
Этот принцип связан с понятием «цена дефекта» (cost of defect). Цена дефекта существенно растет на протяжении жизненного цикла разработки ПО. Чем раньше обнаружен дефект, тем быстрее, проще и дешевле его исправить. Дефект, найденный в требованиях, обходится дешевле всего. 
Еще одно важное преимущество раннего тестирования – экономия времени. Тестовые активности могут начинаться еще до того, как написана первая строчка кода. По мере того, как готовятся требования и спецификации, тестировщики могут приступать к разработке и ревью тест-кейсов. И когда появится первая тестовая версия, можно будет сразу приступать к выполнению тестов.

Принцип 4. Скопление дефектов
Небольшое количество модулей содержит большинство дефектов, обнаруженных на этапе предрелизного тестирования, или же демонстрируют наибольшее количество отказов на этапе эксплуатации.
Многие тестировщики наблюдали такой эффект – дефекты «кучкуются». Это может происходить потому, что определенная область кода особенно сложна и запутана, или потому, что внесение изменений производит «эффект домино». Это знание часто используется для оценки рисков при планировании тестов – тестировщики фокусируются на известных «проблемных зонах». Также полезно проводить анализ первопричин (root cause analysis), чтобы предотвратить повторное появление дефектов, обнаружить причины возникновения скоплений дефектов и спрогнозировать потенциальные скопления дефектов в будущем.

Принцип 5. Парадокс пестицида
Если повторять те же тесты снова и снова, в какой-то момент этот набор тестов перестанет выявлять новые дефекты. Повторное применение тех же тестов и тех же методик приводит к тому, что в продукте остаются именно те дефекты, против которых эти тесты и эти методики неэффективны.
Чтобы преодолеть «парадокс пестицидов», необходимо регулярно пересматривать существующие тест-кейсы и создавать новые, разнообразные тесты, которые будут выполняться на различных частях системы.
 
Принцип 6. Тестирование зависит от контекста
Тестирование выполняется по-разному, в зависимости от контекста. Например, тестирование систем, критических с точки зрения безопасности, проводится иначе, чем тестирование сайта интернет-магазина.
Этот принцип тесно связан с понятием риска. Что такое риск? Риск – это потенциальная проблема. У риска есть вероятность (likelihood) – она всегда выше 0 и ниже 100% – и есть влияние (impact) – те негативные последствия, которых мы опасаемся. Анализируя риски, мы всегда взвешиваем эти два аспекта: вероятность и влияние.
То же можно сказать и о мире ПО: разные системы связаны с различными уровнями риска, влияние того или иного дефекта также сильно варьируется. Одни проблемы довольно тривиальны, другие могут дорого обойтись и привести к большим потерям денег, времени, деловой репутации, а в некоторых случаях даже привести к травмам и смерти.
Уровень риска влияет на выбор методологий, техник и типов тестирования. <img src="https://lh6.googleusercontent.com/4UYXQ5DHdtgibdzNodKMrNo3CemS1449MPJVgUx9b9KgEJ7y3YDc-VFzZcE1zXn9azLrVtY8IfXLdP6UYh_tYuzpn3pGT6N5SbkVd_x0MPSuRqKUs9ugI-NxJiyCa5_TF_AT7t_-">

Принцип 7. Заблуждение об отсутствии ошибок
Нахождение и исправление дефектов бесполезно, если построенная система неудобна для использования и не соответствует нуждам и ожиданиям пользователей.
Заказчики ПО – люди и организации, которые покупают и используют его, чтобы выполнять свои повседневные задачи – на самом деле совершенно не интересуются дефектами и их количеством, кроме тех случаев, когда они непосредственно сталкиваются с нестабильностью продукта. Им также неинтересно, насколько ПО соответствует формальным требованиям, которые были задокументированы. Пользователи ПО более заинтересованы в том, чтобы оно помогало им эффективно выполнять задачи. ПО должно отвечать их потребностям, и именно с этой точки зрения они его оценивают.
Даже если вы выполнили все тесты и ошибок не обнаружили, это еще не гарантия того, что ПО будет соответствовать нуждам и ожиданиям пользователей.
Иначе говоря, верификация != валидация.

* Принцип 8. GIGO.
В компьютерной науке «garbage in – garbage out» (GIGO) — это концепция, в которой ошибочные или бессмысленные входные данные создают бессмысленный вывод или «мусор», т.е. при неверных входящих данных будут получены неверные результаты, даже если сам по себе алгоритм правилен. В тестировании такие случаи иногда создают намеренно, но я добавил этот принцип в общий список для того, чтобы подчеркнуть важность подготовки качественных тестовых данных, положительные они или отрицательные.

Доп. материал: <a href="https://theqalead.com/topics/zero-defect-software/">The Cold Hard Truth About Zero-Defect Software</a>
<h2>Критерии выбора тестов?</h2>
Требования к идеальному критерию тестирования:
<ul>
<li>Критерий должен быть достаточным, т.е. показывать, когда некоторое конечное множество тестов достаточно для тестирования данной программы.
</li>
<li>Критерий должен быть полным, т.е. в случае ошибки должен существовать тест из множества тестов, удовлетворяющих критерию, который раскрывает ошибку.
</li>
<li>Критерий должен быть надежным, т.е. любые два множества тестов, удовлетворяющих ему, одновременно должны раскрывать или не раскрывать ошибки программы.
</li>
<li>Критерий должен быть легко проверяемым, например вычисляемым на тестах.
</li>
</ul>
Для нетривиальных классов программ в общем случае не существует полного и надежного критерия, зависящего от программ или спецификаций. Поэтому мы стремимся к идеальному общему критерию через реальные частные. Классы критериев:
<ul>
<li>Структурные критерии используют информацию о структуре программы (критерии так называемого "белого ящика").
</li>
<li>Функциональные критерии формулируются в описании требований к программному изделию ( критерии так называемого "черного ящика" ).
</li>
<li>Критерии стохастического тестирования формулируются в терминах проверки наличия заданных свойств у тестируемого приложения, средствами проверки некоторой статистической гипотезы.
</li>
<li>Мутационные критерии ориентированы на проверку свойств программного изделия на основе подхода Монте-Карло.
</li>
</ul>
Структурные критерии используют модель программы в виде "белого ящика", что предполагает знание исходного текста программы или спецификации программы в виде потокового графа управления. Структурная информация понятна и доступна разработчикам подсистем и модулей приложения, поэтому данный класс критериев часто используется на этапах модульного и интеграционного тестирования (Unit testing, Integration testing). Структурные критерии базируются на основных элементах УГП (Управляющий граф программы), операторах, ветвях и путях.
<ul>
<li>Условие критерия тестирования команд (критерий С0) - набор тестов в совокупности должен обеспечить прохождение каждой команды не менее одного раза. Это слабый критерий, он, как правило, используется в больших программных системах, где другие критерии применить невозможно.
</li>
<li>Условие критерия тестирования ветвей (критерий С1) - набор тестов в совокупности должен обеспечить прохождение каждой ветви не менее одного раза. Это достаточно сильный и при этом экономичный критерий, поскольку множество ветвей в тестируемом приложении конечно и не так уж велико. Данный критерий часто используется в системах автоматизации тестирования.
</li>
<li>Условие критерия тестирования путей (критерий С2) - набор тестов в совокупности должен обеспечить прохождение каждого пути не менее 1 раза. Если программа содержит цикл (в особенности с неявно заданным числом итераций), то число итераций ограничивается константой (часто - 2, или числом классов выходных путей).
</li>
</ul>
Структурные критерии не проверяют соответствие спецификации, если оно не отражено в структуре программы. Поэтому при успешном тестировании программы по критерию C2 мы можем не заметить ошибку, связанную с невыполнением некоторых условий спецификации требований.
Функциональный критерий - важнейший для программной индустрии критерий тестирования. Он обеспечивает, прежде всего, контроль степени выполнения требований заказчика в программном продукте. Поскольку требования формулируются к продукту в целом, они отражают взаимодействие тестируемого приложения с окружением. При функциональном тестировании преимущественно используется модель "черного ящика". Проблема функционального тестирования - это, прежде всего, трудоемкость; дело в том, что документы, фиксирующие требования к программному изделию (Software requirement specification, Functional specification и т.п.), как правило, достаточно объемны, тем не менее, соответствующая проверка должна быть всеобъемлющей. Ниже приведены частные виды функциональных критериев:
<ul>
<li>Тестирование пунктов спецификации - набор тестов в совокупности должен обеспечить проверку каждого тестируемого пункта не менее одного раза. Спецификация требований может содержать сотни и тысячи пунктов требований к программному продукту и каждое из этих требований при тестировании должно быть проверено в соответствии с критерием не менее чем одним тестом.
</li>
<li>Тестирование классов входных данных - набор тестов в совокупности должен обеспечить проверку представителя каждого класса входных данных не менее одного раза. При создании тестов классы входных данных сопоставляются с режимами использования тестируемого компонента или подсистемы приложения, что заметно сокращает варианты перебора, учитываемые при разработке тестовых наборов. Следует заметить, что перебирая в соответствии с критерием величины входных переменных (например, различные файлы - источники входных данных), мы вынуждены применять мощные тестовые наборы. Действительно, наряду с ограничениями на величины входных данных, существуют ограничения на величины входных данных во всевозможных комбинациях, в том числе проверка реакций системы на появление ошибок в значениях или структурах входных данных. Учет этого многообразия - процесс трудоемкий, что создает сложности для применения критерия.
</li>
<li>Тестирование правил - набор тестов в совокупности должен обеспечить проверку каждого правила, если входные и выходные значения описываются набором правил некоторой грамматики. Следует заметить, что грамматика должна быть достаточно простой, чтобы трудоемкость разработки соответствующего набора тестов была реальной (вписывалась в сроки и штат специалистов, выделенных для реализации фазы тестирования).
</li>
<li>Тестирование классов выходных данных - набор тестов в совокупности должен обеспечить проверку представителя каждого выходного класса, при условии, что выходные результаты заранее расклассифицированы, причем отдельные классы результатов учитывают, в том числе, ограничения на ресурсы или на время (time out). При создании тестов классы выходных данных сопоставляются с режимами использования тестируемого компонента или подсистемы, что заметно сокращает варианты перебора, учитываемые при разработке тестовых наборов.
</li>
<li>Тестирование функций - набор тестов в совокупности должен обеспечить проверку каждого действия, реализуемого тестируемым модулем, не менее одного раза. Очень популярный на практике критерий, который, однако, не обеспечивает покрытия части функциональности тестируемого компонента, связанной со структурными и поведенческими свойствами, описание которых не сосредоточено в отдельных функциях (т.е. описание рассредоточено по компоненту). Критерий тестирования функций объединяет отчасти особенности структурных и функциональных критериев. Он базируется на модели "полупрозрачного ящика", где явно указаны не только входы и выходы тестируемого компонента, но также состав и структура используемых методов (функций, процедур) и классов.
</li>
<li>Комбинированные критерии для программ и спецификаций - набор тестов в совокупности должен обеспечить проверку всех комбинаций непротиворечивых условий программ и спецификаций не менее одного раза. При этом все комбинации непротиворечивых условий надо подтвердить, а условия противоречий следует обнаружить и ликвидировать.
</li>
</ul>

Стохастическое тестирование применяется при тестировании сложных программных комплексов - когда набор детерминированных тестов (X,Y) имеет громадную мощность.
Мутационный критерий (класс IV). Постулируется, что профессиональные программисты пишут сразу почти правильные программы, отличающиеся от правильных мелкими ошибками или описками типа - перестановка местами максимальных значений индексов в описании массивов, ошибки в знаках арифметических операций, занижение или завышение границы цикла на 1 и т.п. Предлагается подход, позволяющий на основе мелких ошибок оценить общее число ошибок, оставшихся в программе. Подход базируется на следующих понятиях: Мутации - мелкие ошибки в программе. Мутанты - программы, отличающиеся друг от друга мутациями . Метод мутационного тестирования - в разрабатываемую программу P вносят мутации, т.е. искусственно создают программы-мутанты P1, P2... Затем программа P и ее мутанты тестируются на одном и том же наборе тестов (X,Y). Если на наборе (X,Y) подтверждается правильность программы P и, кроме того, выявляются все внесенные в программы-мутанты ошибки, то набор тестов (X,Y) соответствует мутационному критерию, а тестируемая программа объявляется правильной. Если некоторые мутанты не выявили всех мутаций, то надо расширять набор тестов (X,Y) и продолжать тестирование.

Подробнее и с примерами в источнике: <a href="https://www.intuit.ru/studies/courses/48/48/lecture/1428?page=1">https://www.intuit.ru/studies/courses/48/48/lecture/1428?page=1</a>
Доп. материал: <a href="https://www.youtube.com/watch?v=qkUCzvP-5mg&t=20547s">https://www.youtube.com/watch?v=qkUCzvP-5mg&t=20547s</a>
<h2>Что такое импакт анализ (анализ влияния, Impact Analysis)?</h2>
Impact Analysis (импакт анализ) - это исследование, которое позволяет указать затронутые места (affected areas) в проекте при разработке новой или изменении старой функциональности, а также определить, насколько значительно они были затронуты.
Затронутые области требуют большего внимания во время проведения регрессионного тестирования.
Импакт анализ может быть полезным в следующих случаях:
<ul>
<li>есть изменения в требованиях;
</li>
<li>получен запрос на внесение изменений в продукт;
</li>
<li>ожидается внедрение нового модуля или функциональности в существующий продукт;
</li>
<li>каждый раз, когда есть изменения в существующих модулях или функциональностях продукта.
</li>
</ul>
Как мы знаем, в настоящее время продукты становятся все более большими и комплексными, а компоненты все чаще зависят друг от друга. Изменение строчки кода в таком проекте может "сломать" абсолютно все.
Информация о взаимосвязи и взаимном влиянии изменений могут помочь QA:
<ul>
<li>сфокусироваться на тестировании функциональности, где изменения были представлены;
</li>
<li>принять во внимание части проекта, которые были затронуты изменениями и, возможно, пострадали;
</li>
<li>не тратить время на тестирование тех частей проекта, которые не были затронуты изменениями.
</li>
</ul>

Источник:<a href="https://habr.com/ru/post/539208/"> Impact Analysis: 6 шагов, которые облегчат тестирование изменений</a>
<h2>Что подразумевается под тестовым покрытием? (Test Coverage)</h2>
Тестовое Покрытие - это одна из метрик оценки качества тестирования, представляющая из себя плотность покрытия тестами требований либо исполняемого кода. Сложность современного ПО и инфраструктуры сделало невыполнимой задачу проведения тестирования со 100% тестовым покрытием. Поэтому для разработки набора тестов, обеспечивающего более-менее высокий уровень покрытия можно использовать специальные инструменты либо техники тест дизайна.
Существуют следующие подходы к оценке и измерению тестового покрытия:
<ul>
<li><a href="http://www.protesting.ru/testing/testcoverage.html#requirements">Покрытие требований (Requirements Coverage)</a> - оценка покрытия тестами функциональных и нефункциональных требований к продукту путем построения матриц трассировки (traceability matrix).
</li>
<li><a href="http://www.protesting.ru/testing/testcoverage.html#code">Покрытие кода (Code Coverage)</a> - оценка покрытия исполняемого кода тестами, путем отслеживания непроверенных в процессе тестирования частей ПО.
</li>
<li><a href="http://www.protesting.ru/testing/testcoverage.html#flow">Тестовое покрытие на базе анализа потока управления</a> - это одна из техник тестирования белого ящика, основанная на определении путей выполнения кода программного модуля и создания выполняемых тест кейсов для покрытия этих путей. 
</li>
</ul>
Различия:
Метод покрытия требований сосредоточен на проверке соответствия набора проводимых тестов требованиям к продукту, в то время как анализ покрытия кода - на полноте проверки тестами разработанной части продукта (исходного кода), а анализ потока управления - на прохождении путей в графе или модели выполнения тестируемых функций (Control Flow Graph).
Ограничения:
<ul>
<li>Метод оценки покрытия кода не выявит нереализованные требования, так как работает не с конечным продуктом, а с существующим исходным кодом.
</li>
</ul>
<ul>
<li>Метод покрытия требований может оставить непроверенными некоторые участки кода, потому что не учитывает конечную реализацию.
</li>
</ul>

Альтернативное мнение:
Покрытие кода — совершенно бесполезная метрика. Не существует «правильного» показателя. Это вопрос-ловушка. У вас может быть проект со 100% покрытием кода, в котором по-прежнему остаются баги и проблемы. В реальности нужно следить за другими метриками — хорошо известными показателям CTM (Codepipes testing Metrics).
<img src="https://lh5.googleusercontent.com/ycWdGw8XfGW_7xun6DdJ2HLdCP5FaAIht4em7L99M4Pu58zUki4bgk6V0o4VjnGCxPcxyZFsXKep5rwyJP-KVQa9daBeK0XdCUgOkSUvBsPJyLOTxnYOHunUBfvIOrgMuUeH7f61">

PDWT (процент разработчиков, пишущих тесты) — вероятно, самый важный показатель. Нет смысла говорить об антипаттернах тестирования ПО, если у вас вообще нет тестов. Все разработчики в команде должны писать тесты. Любую новую функцию можно объявлять сделанной только если она сопровождается одним или несколькими тестами.

PBCNT (процент багов, приводящих к созданию новых тестов). Каждый баг в продакшне — отличный повод для написания нового теста, проверяющего соответствующее исправление. Любой баг должен появиться в продакшне не более одного раза. Если ваш проект страдает от появления повторных багов даже после их первоначального «исправления», то команда действительно выиграет от использования этой метрики.

PTVB (процент тестов, которые проверяют поведение, а не реализацию). Тесно связанные тесты пожирают массу времени при рефакторинге основного кода.

PTD (процент детерминированных тестов от общего числа). Тесты должны завершаться ошибкой только в том случае, если что-то не так с бизнес-кодом. Если тесты периодически ломаются без видимой причины — это огромная проблема.

Если после прочтения о метриках вы по-прежнему настаиваете на установке жесткого показателя для покрытия кода, я дам вам число 20%. Это число должно использоваться как эмпирическое правило, основанное на законе Парето. 20% вашего кода вызывает 80% ваших ошибок

Доп. материал:
<a href="https://intuit.ru/studies/courses/48/48/lecture/1430">Лекция 4: Оценка оттестированности проекта: метрики и методика интегральной оценки</a>
<h2>Что такое модель зрелости тестирования (TMM - Test Maturity Model)?</h2>
Существует определение Maturity Models, то есть модели зрелости различных процессов в организации, состоящая из 5 уровней. Нас же в рамках этого материала интересует один конкретный подвид моделей MM - модель зрелости тестирования, которая тоже состоит из 5 уровней. TMM в свою очередь основан на модели зрелости возможностей (CMM — Capability Maturity Model). Модель зрелости ПО (CMM или SW-CMM) — это модель для оценки зрелости программных процессов в организации. В ней также перечислены некоторые стандартные практики, которые увеличивают зрелость этих процессов. TMM это подробная модель для улучшения процесса тестирования. Она может быть дополнена любой моделью улучшения процесса или может использоваться как одиночная модель.
Модель ТММ имеет два основных компонента:
<ul>
<li>Набор из 5 уровней, которые определяют возможности тестирования (testing capability)
</li>
<li>Модель оценки (An Assessment Model)
</li>
</ul>
Пять уровней TMM помогают организации определить зрелость своего процесса и определить следующие шаги по улучшению, которые необходимы для достижения более высокого уровня зрелости тестирования. Приведенный далее текст является переводом, но есть и русскоязычные на эту тему. Однако материал везде несколько отличается, поэтому представляю несколько точек зрения: 
<a href="https://devsday.ru/blog/details/5427">https://devsday.ru/blog/details/5427</a> <a href="https://www.software-testing.ru/library/around-testing/processes/3092-test-maturity-model">https://www.software-testing.ru/library/around-testing/processes/3092-test-maturity-model</a> <a href="https://habr.com/ru/company/otus/blog/479368/">https://habr.com/ru/company/otus/blog/479368/</a>
<ul>
<li>Уровень 1. Начальный. ПО должно успешно работать.
</li>
<ul>
<li>На этом уровне области процессов не определены.
</li>
<li>Цель тестирования — убедиться, что ПО работает нормально.
</li>
<li>На этом уровне не хватает ресурсов, инструментов и обученного персонала.
</li>
<li>Нет проверки качества перед поставкой ПО.
</li>
</ul>
<li>Уровень 2. Определенный. Разработка целей и политик тестирования и отладки.
</li>
<ul>
<li>Этот уровень отличает тестирование от отладки, и они считаются различными действиями.
</li>
<li>Этап тестирования наступает после кодирования.
</li>
<li>Основная цель тестирования — показать, что ПО соответствует спецификации.
</li>
<li>Основные методы и методики тестирования.
</li>
</ul>
<li>Уровень 3: Комплексный. Интеграция тестирования в жизненный цикл ПО.
</li>
<ul>
<li>Тестирование интегрируется в весь жизненный цикл.
</li>
<li>На основании требований определяются цели испытаний.
</li>
<li>Структура тестирования существует.
</li>
<li>Тестирование на уровне профессиональной деятельности.
</li>
</ul>
<li>Уровень 4: Управление и измерение. Создание программы тестовых измерений.
</li>
<ul>
<li>Тестирование — это измеренный и количественный процесс.
</li>
<li>Проверка на всех этапах разработки признается как тестирование.
</li>
<li>Для повторного использования и регрессионного тестирования есть Test case и они записаны в базу тестов.
</li>
<li>Дефекты регистрируются и получают уровни серьезности.
</li>
</ul>
<li>Уровень 5: Оптимизированный. Оптимизация процесса тестирования.
</li>
<ul>
<li>Тестирование управляется и определено.
</li>
<li>Эффективность и стоимость тестирования можно отслеживать.
</li>
<li>Тестирование может постоянно настраиваться и улучшаться.
</li>
<li>Практика контроля качества и предотвращения дефектов.
</li>
<li>Практикуется процесс повторного использования (Reuse).
</li>
<li>Метрики, связанные с тестированием, также имеют средства поддержки.
</li>
<li>Инструменты обеспечивают поддержку разработки тестовых наборов и сбора дефектов.
</li>
</ul>
</ul>

Доп. материал:<a href="https://medium.com/@grifer163/7-%D0%BF%D0%BE%D0%B4%D1%85%D0%BE%D0%B4%D0%BE%D0%B2-%D0%BA-%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8E-a78fc69da167"> 7 подходов к тестированию</a>
<h2>Что такое тестирование со сдвигом влево? (Shift left testing) </h2>
В попытке перенести тестирование на более ранний этап жизненного цикла разработки при одновременном улучшении показателей качества, задачи смещаются влево в схеме жизненного цикла разработки ПО. По возможности, тестирование должно проводиться с самого начала фазы проектирования, чтобы построить соответствующую стратегию тестирования. Проще говоря, это подход к тестированию программного обеспечения и тестированию системы, при котором тестирование выполняется на более раннем этапе жизненного цикла. Ключевые преимущества:
<ul>
<li>Сокращение затрат 
</li>
<li>Более высокое качество
</li>
<li>Повышение эффективности 
</li>
<li>Конкурентные преимущества
</li>
</ul>

Доп. материал:
<a href="https://habr.com/ru/post/543318/">Экономим ресурсы и успеваем в срок: зачем подключать QA-инженера в начале работы над фичей</a>
<h2>Что такое независимое тестирование? (Independent testing)</h2>
Можете ли вы доверять вердикту судьи, который является частью внутреннего круга людей, которых он должен судить? Чтобы этот процесс был справедливым, лица, принимающие решения, должны быть беспристрастными. Теперь, когда вы активно участвуете в разработке какого-либо продукта или программного обеспечения, тестировать его с нейтральным мышлением это легче сказать, чем сделать. Как разработчик, вы бы хотели отгружать продукт в кратчайшие сроки и считать его безупречным и в конечном итоге упустите из виду некоторые ошибки. Чтобы избежать такой ситуации, иногда следует нанять независимую организацию по тестированию, которая тщательно проверит ваш продукт на наличие сбоев, готовя его к развертыванию. 
Тестирование по уровням независимости:
<ul>
<li>Программист тестирует свой код 
</li>
<li>Тестирование проводится другим программистом в организации
</li>
<li>Внутренняя команда тестирования 
</li>
<li>Независимая организация тестирования
</li>
</ul>

<ul>
<li>Когда программист проверяет свой код: Вы бы никогда не попросили шеф-повара быть его собственным критиком. И даже если вы это сделаете, вам будет трудно поверить всему, что он говорит. Смысл - создатель никогда не может быть хорошим критиком своей собственной работы. Программист знает свой код от и до. Их цель - создать продукт и отправить его в кратчайшие сроки. Вместо того, чтобы искать ошибки со всех возможных точек зрения, они будут искушены найти способы обойти найденные ошибки. Писатель Гленфорд Майерс в своей книге «Искусство тестирования программного обеспечения» перечислил разницу в мышлении разработчика и тестировщика. Он сказал, что разработчик думает как строитель, сосредоточенный на строительстве, в то время как тестировщик ищет недостатки, которые приведут к разрушению здания, если не будут решены. 
</li>
<li>Тестирование проводится другим программистом в организации: Компромисс - это найти кого-то в организации. Это может быть какой-то другой программист, который участвует в некоторых других проектах. Это дает определенный уровень независимости. Но проблема возникает из-за того же reporting manager. Менеджер может попросить программиста пропустить некоторые тесты, когда есть ограничения по времени. Это приведет к неполному тестированию продукта. Кроме того, если попросить других разработчиков провести тестирование, это приведет к развертыванию различных ресурсов в одном проекте. Это будет вредно для всей работы организации. 
</li>
<li>Внутренняя команда тестирования: Наличие другой внутренней команды - это хорошее решение. Но поскольку они будут в организации, на них будут влиять ограничительные сроки. Кроме того, это будет дорого поддерживать внутреннюю команду. Это приведет к большим бюджетным и ресурсным ограничениям для команды. Команда может иметь доступ к ограниченным инструментам и программному обеспечению, таким образом, не отвечая требованиям всех проектов. Среда тестирования также будет варьироваться в зависимости от количества пользователей и числа выполненных интеграций. Затем тестирование будет проводиться в спешном порядке, что приведет к упущению некоторых ошибок, которые могут появиться после выпуска продукта. Решение, которое позаботится обо всех этих недостатках, - «Независимое тестирование». 
</li>
<li>Почему независимое тестирование? Независимые тестирующие организации изучат все аспекты вашей продукции. Они работают с мышлением поиска недостатков и ошибок. Они не будут использовать ярлыки в процессе тестирования. И поскольку они не были частью процесса разработки, они будут проводить тесты на нейтральной основе, чтобы прежние интересы не мешали процессу тестирования. Мысль о поиске максимальных «точек останова» пойдет на пользу вашему продукту. Почти все сторонние тестирующие организации предоставят вам подробные отчеты об ошибках и предложат корректирующие меры. 
</li>
</ul>
<h2>В чем разница между превентивным и реактивным подходами в тестировании? (Preventative and Reactive approaches)</h2>
<ul>
<li>Превентивный (профилактический) подход: он также известен как Verification Process. Этот подход заключается в предотвращении дефектов. При таком подходе тесты разрабатываются на ранних этапах SDLC, то есть до того, как программное обеспечение было создано. Он подпадает под анализ качества (QA). 
</li>
<li>Реактивный подход: он также известен как Validation Process. Этот подход заключается в выявлении дефектов. При таком подходе тесты предназначены для выполнения после того, как программное обеспечение было произведено. Здесь мы пытаемся найти недостатки. Подпадает под контроль качества (QC).
</li>
</ul>
<h2>Перечислите типичные возможные обязанности инженера по обеспечению качества? </h2>
<ul>
<li>Команда QA отвечает за мониторинг всего процесса разработки. 
</li>
<li>Они несут ответственность за отслеживание результатов каждого этапа SDLC и корректировку их в соответствии с ожиданиями. 
</li>
<li>Они несут ответственность за чтение и понимание необходимых документов. 
</li>
<li>Анализируют требования к тестированию, а также разрабатывают и выполняют тесты. 
</li>
<li>Разрабатывают Test case и расставляют приоритеты в тестировании. 
</li>
<li>Записывают проблемы и инциденты в соответствии с задачами проекта и планами управления инцидентами. 
</li>
<li>Работают с командой приложения и/или клиентом для решения любых проблем, возникающих в процессе тестирования. 
</li>
<li>Проводят регрессионное тестирование каждый раз, когда в код вносятся изменения для исправления дефектов. 
</li>
<li>Должны взаимодействовать с клиентами, чтобы лучше понять требования продукта. 
</li>
<li>Принимают участие в прохождении процедур тестирования.
</li>
</ul>
<h2>Что такое аудит качества? </h2>
Аудит качества - это процесс систематической и независимой проверки программного продукта или процесса для оценки соответствия спецификациям, стандартам, соглашениям и другим соответствующим критериям.
<h2>Почему тестирование делится на отдельные этапы? </h2>
<ul>
<li>Каждый этап испытаний имеет свое назначение 
</li>
<li>Проще управлять поэтапно 
</li>
<li>Мы можем запустить разные тесты в разных средах 
</li>
<li>Производительность и качество тестирования улучшаются с помощью поэтапного тестирования
</li>
</ul>
<h2>Почему невозможно полностью протестировать ПО? </h2>
<ul>
<li>Спецификации ПО могут быть субъективными и приводить к различным интерпретациям. 
</li>
<li>ПО может потребоваться слишком много входов, слишком много выходов и слишком много комбинаций путей для тестирования.
</li>
</ul>
<h2>Как вы тестируете продукт, если требования еще не зафиксированы? </h2>
Если спецификация требований недоступна для продукта, тогда план тестирования может быть создан на основе предположений, сделанных относительно продукта. Но мы должны хорошо документировать все предположения в плане тестирования. 
<h2>Как вы узнаете, было ли создано достаточно тестов для тестирования продукта? </h2>
Прежде всего, мы проверим, охватывает ли каждое требование хотя бы один Test case. Если да, то можно сказать, что тестовых примеров достаточно для тестирования продукта. 
<h2>Как вы понимаете инспекцию? </h2>
Это процесс проверки на уровне группы и улучшения качества документации по продукту. Он фокусируется на следующих двух аспектах: 
<ul>
<li>Улучшение документа продукта 
</li>
<li>Улучшение процесса (как производства документов, так и проверки)
</li>
</ul>
<h2>Какие есть роли/должности в команде?</h2>
<img src="https://lh5.googleusercontent.com/A8vFU_BDXkSdJG3KlSWFvoGcMbwLr1vifKjhwDYYPYyYTOjN8-Cu_EoulIhTHNMzW_0PikTDGgO2FZmNtCJie1rNpjX6z8QHNLcCxJcspISrep5hc0gA1lgBRRF-6VZ_1leCXD3S">
Project manager
Это человек, который берет входящие от заказчика требования (несформулированные хотелки), уточняет все и нормальным языком передает разработчикам, следит за рисками, прогрессом и доводит до финала. На нем вся коммуникация с заказчиком, согласования и т. д. 
Product Owner
Может выполнять немного разные роли в разных компаниях. Человек, который является хранителем информации о продукте. Его роль быть decision maker, он отвечает со стороны бизнеса за приложение, с него будет спрашивать заказчик. Противоположные роли с ПМ, как адвокат с обвинителем. ПМ со стороны команды, пытается извертеться на плюшки, а PO со стороны заказчика выбивает все по максимуму для себя. 
Knowledge manager
Управление знаниями - это о том, как распоряжаться всеми имеющимися в компании знаниями, чтобы позволять всем сотрудникам максимально быстро находить ответы на вопросы, принимать решения, избегать ошибок, придумывать что-то новое, управлять проектами, подбирать и развивать сотрудников. А значит, нужно выстраивать коммуникации между подразделениями, учить их разговаривать друг с другом. Вопросы менеджера по знаниям ведущим специалистам имеют высший приоритет, поэтому тот всегда держит руку на пульсе. Полученные знания после доставки не теряются, а превращаются в обучающие документы, которые изучают все сотрудники.

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/post/538128/">Product Owner vs Product Manager или Product Owner/Product Manager</a>
</li>
<li><a href="https://habr.com/ru/company/habr_career/blog/535032/">Продакт-менеджмент как профессия: востребованность, зарплата и другие нюансы</a>
</li>
<li><a href="https://habr.com/ru/post/535418/">Кто такой продакт-менеджер? Или не все PM’ы — проджект-менеджеры</a>
</li>
<li><a href="https://habr.com/ru/company/plarium/blog/541814/">Knowledge management: как перестать изобретать велосипеды</a>
</li>
<li><a href="https://habr.com/ru/company/exness/blog/505470/">Заметки knowledge manager'a. Как работает управление знаниями в Exness</a>
</li>
<li><a href="https://habr.com/ru/company/ivi/blog/535448/">Профессия СТО</a>
</li>
<li><a href="https://habr.com/ru/company/netologyru/blog/501690/">Кто такой DevOps-инженер, что он делает, сколько зарабатывает и как им стать</a>
</li>
<li><a href="https://habr.com/ru/company/skillfactory/blog/509344/">Гайд по DevOps для начинающих</a>
</li>
</ul>
<h2>Опишите жизненный цикл продукта по этапам - какие участники на каждом этапе, какие у них роли? Какие артефакты на каждом этапе?</h2>
Хотелось бы уточнить, что описанные этапы не являются эталонными и от компании к компании процессы могут радикально отличаться. В данном случае представлены некие «сферические процессы в вакууме» для какого-то начального понимания. Параллельно описывается SDLC и STLC.
<ul>
<li>Анализ. Участники: Product owner, BA(бизнес-аналитик), QA. Артефакты: спецификация требований к ПО (Software Requirement Specification, SRS).
</li>
</ul>
Во время этого этапа BA выясняет у PO все пожелания к продукту и документирует это в процессе обсуждения требований. Необходимо убедиться в том, что все участники правильно поняли поставленные задачи и то, как именно каждое требование будет реализовано на практике. Таким образом, этот этап предполагает сбор требований к разрабатываемому ПО, их систематизацию, документирование, анализ, а также выявление и разрешение противоречий. В компаниях, где налажены процессы обеспечения качества, уже на этом этапе включается в работу QA, т.к. бывают и дефекты требований.
<ul>
<li>Проектирование. Участники: Product owner, разработчики, системные архитекторы, QA. Артефакты: дизайн-спецификация (Design Specification Document, DSD), Тест-план, тест-сценарии, тест-кейсы; вариативно: тестовая стратегия.
</li>
</ul>
На стадии проектирования (называемой также стадией дизайна и архитектуры) программисты и системные архитекторы, руководствуясь требованиями, разрабатывают высокоуровневый дизайн системы. Разнообразные технические вопросы, возникающие в процессе проектирования, обсуждаются со всеми заинтересованными сторонами. Определяются технологии, которые будут использоваться в проекте, загрузка команды, ограничения, временные рамки и бюджет. В соответствии с уточненными требованиями выбираются наиболее подходящие проектные решения. Утвержденный дизайн системы определяет перечень разрабатываемых программных компонентов, взаимодействие с третьими сторонами, функциональные характеристики программы, используемые базы данных и многое другое. QA/test analyst проектируют процесс тестирования в тест плане, руководствуясь также (если есть) политикой и стратегией тестирования. Тестировщики начинают писать сценарии и по ним кейсы для тестирования.
<ul>
<li>Разработка. Участники: разработчики. Артефакты: -.
</li>
</ul>
Системные администраторы настраивают программное окружение, frontend программисты разрабатывают пользовательский интерфейс программы и логику ее взаимодействия с сервером.
Кроме того, программисты пишут Unit-тесты для проверки правильности работы кода каждого компонента системы, проводят ревью написанного кода, создают билды и разворачивают готовое ПО в программной среде. Этот цикл повторяется до тех пор, пока все требования не будут реализованы.
<ul>
<li>Тестирование. Участники: QA. Артефакты: дефект-репорты, сводный отчет о тестировании. 
</li>
</ul>
Тестовый администратор (если есть) настраивает тестовые среды/стенды для проведения тестирования. Тестировщики занимаются поиском дефектов в программном обеспечении и сравнивают описанное в требованиях поведение системы с реальным. В фазе тестирования обнаруживаются пропущенные при разработке баги. При обнаружении дефекта, тестировщик составляет отчет об ошибке, который передается разработчикам. Последние его исправляют, после чего тестирование повторяется – но на этот раз для того, чтобы убедиться, что проблема была исправлена, и само исправление не стало причиной появления новых дефектов в продукте. По итогам проведенного процесса тестирования составляется итоговый отчет.
<ul>
<li>Внедрение и сопровождение. Участники: команда технической поддержки. Артефакты: замечания, запросы на исправление/улучшение.
</li>
</ul>
Когда программа протестирована и в ней больше не осталось серьезных дефектов, приходит время релиза и передачи ее конечным пользователям. После выпуска новой версии программы в работу включается отдел технической поддержки. Его сотрудники обеспечивают обратную связь с пользователями, их консультирование и поддержку. В случае обнаружения пользователями тех или иных пост-релизных багов, информация о них передается в виде отчетов об ошибках команде разработки, которая, в зависимости от серьезности проблемы, либо немедленно выпускает исправление (т.н. hot-fix), либо откладывает его до следующей версии программы. Кроме того, команда технической поддержки помогает собирать и систематизировать различные метрики – показатели работы программы в реальных условиях и т.п.
<h2>Кто такой SDET? </h2>
SDET (Software Development Engineer in Test) инженер по разработке ПО в тестировании - это ИТ-специалист, который может одинаково эффективно работать в сфере разработки и тестирования, и он / она принимает участие в полном процессе разработки ПО. В отличие от Quality Analyst (QA), которым желательны базовые знания в программировании, но нет необходимости писать код, SDET это делает на постоянной основе, совмещая в себе и тестировщика и разработчика.
<table>
<tr>
<td>SDET
</td><td>Manual Tester
</td></tr>
<tr>
<td>Знает всю систему от начала до конца
</td><td>Ограниченные знания о системе
</td></tr>
<tr>
<td>SDET участвует в каждом этапе процесса разработки ПО, как Проектирование, разработка и тестирование.
</td><td>QA участвует только в жизненном цикле тестирования процесса разработки ПО.
</td></tr>
<tr>
<td>Высококвалифицированный специалист со знаниями как в разработке, так и в тестировании
</td><td>Тестировщик ПО участвует только в подготовке и выполнении Test case
</td></tr>
<tr>
<td>SDET может участвовать в разработке средств автоматизации тестирования
</td><td>Не ожидается разработка средств автоматизации тестирования.
</td></tr>
<tr>
<td>SDET должны выполнять такие обязанности, как тестирование производительности, автоматическое создание тестовых данных и т. д. 
</td><td>Только задачи по ручному тестированию
</td></tr>
<tr>
<td>Знает требования и гайдлайны для продуктов
</td><td>От QA таких знаний не ожидается.
</td></tr>
</table>

<h2>Что такое тестирование как сервис? (TaaS – testing as a Service)</h2>
ТЕСТИРОВАНИЕ КАК СЕРВИС (TaaS) - это модель аутсорсинга, при которой деятельность по тестированию передается третьей стороне. Здесь тестирование проводится сторонними подрядчиками, а не сотрудниками организации. TaaS используется, когда Компании не хватает навыков или ресурсов для внутреннего тестирования или чтобы получить свежий взгляд со стороны. Чаще всего на аутсорс отдают тестирование функциональности, производительности и безопасности.
<h2>Что подразумевается под тестовой средой? (Test Environment/Test Bed)</h2>
Вообще существует несколько сред:
<ul>
<li>Среда разработки (Development Env) – в ней разработчики пишут код, проводят отладку, исправляют ошибки, выполняют Unit-тестирование. За эту среду отвечают также разработчики.
</li>
<li>Среда тестирования (Test Env) – в этой среде работают тестировщики. Тут тестируются новые билды. Здесь тестировщики проверяют функционал, проводят регрессионные проверки, воспроизводят ошибки. Эта среда появляется во время начала динамического тестирования;
</li>
<li>Интеграционная среда (Integration Env) – иногда реализована в рамках среды тестирования, а иногда в рамках превью среды. В этой среде собрана необходимая для end-to-end тестирования схема взаимодействующих друг с другом модулей, систем, продуктов. Собственно, необходима она для интеграционного тестирования. Поддержка среды – также, как и в случае со средой тестирования
</li>
<li>Превью среда (Preview, Preprod Env) – в идеале, это среда идентичная или максимально приближенная к продуктивной: те же данные, то же аппаратно-программное окружение, та же производительность. Она используется, чтобы сделать финальную проверку ПО в условиях максимально приближенным к «боевым». Здесь тестировщики проводят заключительное end-to-end тестирование функционала, бизнес и/или пользователи проводят UAT, а команды поддержки L3 и L2 выполняют DryRun (пробную установку релиза). Как правило за эту среду отвечает группа L3 поддержки.
</li>
<li>Продакшн среда (Production Env) – среда, в которой работают пользователи. С этой средой работает команда L2 поддержки устанавливая поставки ПО или патчи с исправлениями, выполняя настройки, отвечая за работоспособность всех систем. Инциденты и проблемы требующие исправления ПО передаются в работу команде на L3

</li>
</ul>
В общем случае среда тестирования - это настройка программного и аппаратного обеспечения для тестирования. 
Испытательный стенд (Test Bed) – более глобальная сущность и включает в себя operating system, configuration management for the products, hardware, network topology и т. д.  Настраиваются в соответствии с требованиями тестируемого приложения. В некоторых случаях испытательный стенд может представлять собой комбинацию тестовой среды и тестовых данных, которые он использует. 
Настройка правильной среды тестирования гарантирует успех тестирования ПО. Любые недостатки в этом процессе могут привести к дополнительным затратам и времени для клиента. Следующие люди участвуют в настройке тестовой среды: Системные администраторы, Разработчики, Тестировщики.

Доп. материал:
<ul>
<li><a href="https://coderlessons.com/tutorials/kachestvo-programmnogo-obespecheniia/ruchnoe-testirovanie/testovaia-sreda-2#:~:text=%D0%A1%D1%80%D0%B5%D0%B4%D0%B0%20%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20%E2%80%94%20%D1%8D%D1%82%D0%BE%20%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D0%BE%D0%B3%D0%BE,%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20%D0%B4%D0%BB%D1%8F%20%D0%B2%D1%8B%D0%BF%D0%BE%D0%BB%D0%BD%D0%B5%D0%BD%D0%B8%D1%8F%20%D1%82%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D1%8B%D1%85%20%D1%81%D0%BB%D1%83%D1%87%D0%B0%D0%B5%D0%B2.&text=%D0%9D%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0%20%D0%BF%D1%80%D0%B0%D0%B2%D0%B8%D0%BB%D1%8C%D0%BD%D0%BE%D0%B9%20%D1%81%D1%80%D0%B5%D0%B4%D1%8B%20%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20%D0%B3%D0%B0%D1%80%D0%B0%D0%BD%D1%82%D0%B8%D1%80%D1%83%D0%B5%D1%82%20%D1%83%D1%81%D0%BF%D0%B5%D1%85%20%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F%20%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BE%D0%B1%D0%B5%D1%81%D0%BF%D0%B5%D1%87%D0%B5%D0%BD%D0%B8%D1%8F.">Тестовая среда</a>
</li>
<li><a href="https://coderlessons.com/tutorials/kachestvo-programmnogo-obespecheniia/uznaite-stlc/stlc-nastroika-testovoi-sredy">STLC — настройка тестовой среды</a>
</li>
</ul>
<h2>Что подразумевается под тестовыми данными?</h2>
Тестовые данные - это набор входных значений, необходимых для выполнения Test case. тестировщики определяют данные в соответствии с требованиями. Они могут сделать это вручную или использовать инструменты генерации. 
<h2>Основные фазы тестирования?</h2>
<ul>
<li>Pre-Alpha: - ПО является прототипом. Пользовательский интерфейс завершен. Но не все функции завершены. На данном этапе ПО не публикуется. 
</li>
<li>Alpha: является ранней версией программного продукта. Цель - вовлечь клиента в процесс разработки. Хороший Альфа-тест должен иметь четко определенный план тестирования с комплексными тестовыми примерами. Это дает лучшее представление о надежности программного обеспечения на ранних стадиях. В некоторых случаях тестирование может быть передано на аутсорс. 
</li>
<li>Beta: ПО стабильно и выпускается для ограниченной пользовательской базы. Цель состоит в том, чтобы получить отзывы клиентов о продукте и внести соответствующие изменения в ПО. 
</li>
<li>Release Candidate (RC): основываясь на отзывах Beta Test, вы вносите изменения в ПО и хотите проверить исправления ошибок. На этом этапе вы не хотите вносить радикальные изменения в функциональность, а просто проверяете наличие ошибок. RC также выпущен для общественности 
</li>
<li>Release: Все работает, ПО выпущено для общественности. 
</li>
</ul>
<h2>Подробнее про бета-тестирование? </h2>
Бета-тестирование происходит на конечных пользователях. Это нужно для обеспечения обратной связи. 
Существуют различные типы бета-тестов в тестировании ПО, и они заключаются в следующем: 
<ul>
<li>Традиционное бета-тестирование: продукт распространяется на целевой рынок, и соответствующие данные собираются по всем аспектам. Эти данные могут быть использованы для улучшения продукта. 
</li>
<li>Публичное бета-тестирование: продукт публикуется во внешнем мире через онлайн-каналы, и данные могут быть получены от любого пользователя. На основе обратной связи могут быть сделаны улучшения продукта. 
</li>
<li>Техническое бета-тестирование: продукт передается во внутреннюю группу организации и собирает отзывы / данные от сотрудников организации. 
</li>
<li>Целевая бета-версия: продукт выпущен на рынок для сбора отзывов об особенностях программы. 
</li>
<li>Бета-версия после выпуска. Продукт выпущен на рынок, и данные собираются для внесения улучшений в будущем выпуске продукта.
</li>
</ul>
<h2>Что означает пилотное тестирование? (Pilot)</h2>
PILOT testing определяется как тип тестирования программного обеспечения, который проверяет компонент системы или всю систему в режиме реального времени. Целью пилотного теста является оценка осуществимости, времени, стоимости, риска и эффективности исследовательского проекта. Это тестирование проводится точно между UAT и Production. В пилотном тестировании выбранная группа конечных пользователей пробует тестируемую систему и предоставляет обратную связь до полного развертывания системы. Другими словами, это означает проведение генеральной репетиции для последующего теста на удобство использования. Пилотное тестирование помогает в раннем обнаружении ошибок в Системе.
Пилотное тестирование связано с установкой системы на площадке заказчика (или в среде, моделируемой пользователем) для тестирования на предмет постоянного и регулярного использования. Выявленные недостатки затем отправляются команде разработчиков в виде отчетов об ошибках, и эти ошибки исправляются в следующей сборке системы. Во время этого процесса иногда приемочное тестирование также включается как часть тестирования на совместимость. Это происходит, когда система разрабатывается для замены старой. 
<h2>В чем отличие build от release?</h2>
Билд это номер, даваемый ПО при передаче от разработчиков тестировщикам. Релиз — это номер, даваемый ПО при передаче конечному пользователю.
<h2>Что такое бизнес – логика (domain)?</h2>
Бизнес – логика (domain) это то, что конкретная программа по задумке должна сделать. Например, в складской программе проверка на возможность отправить товар (вдруг его нет в наличии). Это правила, которые должны соблюдаться в данной конкретной программе, определенные бизнес-клиентом. Слои приложения – слой пользовательского интерфейса, слой бизнес логики, слой сохранения данных.










<h1>----- Виды тестирования -----</h1>
<h2>Какие существуют основные виды тестирования ПО? </h2>
<ul>
<li>Функциональные виды («Что?» - проверяет весь функционал продукта):
</li>
<ul>
<li>Функциональное тестирование (Functional testing)
</li>
<li>Тестирование взаимодействия (Interoperability testing)
</li>
</ul>
<li>Нефункциональное («Как?»):
</li>
<ul>
<li>Производительности (Performance)
</li>
<ul>
<li>Тестирование емкости/способностей (Capacity testing)
</li>
<li>Стрессовое (Stress testing)
</li>
<li>Нагрузочное (Load testing)
</li>
<li>Объемное тестирование (Volume testing)
</li>
<li>Выносливости (Soak/Endurance testing)
</li>
<li>Стабильности/надежности (Stability / Reliability testing)
</li>
<li>Шиповое (Spike)
</li>
<li>Отказоустойчивости (Stability testing)
</li>
<li>Масштабируемости (Scalability test)
</li>
</ul>
<li>Отказ и восстановление (Failover and Recovery testing)
</li>
<li>Удобство пользования (Usability testing)
</li>
<li>Тестирование установки (Installation testing)
</li>
<li>Тестирование безопасности (Security and Access Control testing)
</li>
<li>Конфигурационное (Configuration testing)
</li>
</ul>
<li>Связанное с изменениями:
</li>
<ul>
<li>Регрессионное (Regression testing)
</li>
<li>Санитарное (Sanity testing)
</li>
<li>Дымовое (Smoke testing)
</li>
<li>Тестирование сборки (Build Verification testing)
</li>
</ul>
</ul>
В разных источниках предлагается разный взгляд:

<img src="https://lh5.googleusercontent.com/wKytfmj7ee7u7zgaRb-B1nfJwO-oTu_Q8Yidnf6df0BTZldvdGF-PqfaV4TgZp3sXnD60A3W4RzBniexE5SmESozeXHZJkT67_M_4kgt4WYxLsgiQqxEIwFCsA4UpfaJm-URQv7w">
<img src="https://lh4.googleusercontent.com/d6u6n4M8HenGww1y10nZZpQP22k-BrYomMm6WiZuY0jQhZxUubtRN1tXvFPyCJqp2RuZCDtjtuCf-GyXPzakS8g8IZXcAGRTr7jir3tp5UTXkZLAD_2139wAf3MbGJoMUDD2hACk">
<img src="https://lh3.googleusercontent.com/1MO0Dp2MwPU_ZOD46tlGIPKnGlrmvWog4E-cpVt5jm3jzEYkFx9IYYh9ONWaSVInu7M-JMVXd_H0mlqt87UkQ3s9HDgdHWD-yMEn6hCujYnOcPt5gnwuHVGuREr2ScAw9N2wds-e">

<h2>Типы тестирования? (White/Black/Grey Box)</h2>
Самым высоким уровнем в иерархии подходов к тестированию будет понятие типа, которое может охватывать сразу несколько смежных техник тестирования. То есть, одному типу тестирования может соответствовать несколько его видов. Отличаются они знанием внутреннего устройства объекта тестирования.
<h2>Что означает тестирование черного ящика?</h2>
Summary: Мы не знаем, как устроена внутри тестируемая система.
Тестирование методом «черного ящика», также известное как тестирование, основанное на спецификации или тестирование поведения – техника тестирования, основанная на работе исключительно с внешними интерфейсами тестируемой системы.
– тестирование, как функциональное, так и нефункциональное, не предполагающее знания внутреннего устройства компонента или системы.
– тест-дизайн, основанный на технике черного ящика – процедура написания или выбора тест-кейсов на основе анализа функциональной или нефункциональной спецификации компонента или системы без знания ее внутреннего устройства.
Почему именно «черный ящик»? Тестируемая программа для тестировщика – как черный непрозрачный ящик, содержания которого он не видит. Целью этой техники является поиск ошибок в таких категориях:
– неправильно реализованные или недостающие функции;
– ошибки интерфейса;
– ошибки в структурах данных или организации доступа к внешним базам данных;
– ошибки поведения или недостаточная производительности системы;
Таким образом, мы не имеем представления о структуре и внутреннем устройстве системы. Нужно концентрироваться на том, ЧТО программа делает, а не на том, КАК она это делает.
Пример:
Тестировщик проводит тестирование веб-сайта, не зная особенностей его реализации, используя только предусмотренные разработчиком поля ввода и кнопки. Источник ожидаемого результата – спецификация.
Поскольку это тип тестирования, по определению он может включать другие его виды. Тестирование черного ящика может быть как функциональным, так и нефункциональным. Функциональное тестирование предполагает проверку работы функций системы, а нефункциональное – соответственно, общие характеристики нашей программы.
Техника черного ящика применима на всех уровнях тестирования (от модульного до приемочного), для которых существует спецификация. Например, при осуществлении системного или интеграционного тестирования, требования или функциональная спецификация будут основой для написания тест-кейсов.
Техники тест-дизайна, основанные на использования черного ящика, включают:
– классы эквивалентности;
– анализ граничных значений;
– таблицы решений;
– диаграммы изменения состояния;
– тестирование всех пар.
Преимущества:
– тестирование производится с позиции конечного пользователя и может помочь обнаружить неточности и противоречия в спецификации;
– тестировщику нет необходимости знать языки программирования и углубляться в особенности реализации программы;
– тестирование может производиться специалистами, независимыми от отдела разработки, что помогает избежать предвзятого отношения;
– можно начинать писать тест-кейсы, как только готова спецификация.
Недостатки:
– тестируется только очень ограниченное количество путей выполнения программы;
– без четкой спецификации (а это скорее реальность на многих проектах) достаточно трудно составить эффективные тест-кейсы;
– некоторые тесты могут оказаться избыточными, если они уже были проведены разработчиком на уровне модульного тестирования;
Противоположностью техники черного ящика является тестирование методом белого ящика, речь о котором пойдет ниже.
<h2>Что означает тестирование белого ящика?</h2>
Тестирование методом белого ящика (также: прозрачного, открытого, стеклянного ящика; основанное на коде или структурное тестирование) – метод тестирования ПО, который предполагает, что внутренняя структура/устройство/реализация системы известны тестировщику. Мы выбираем входные значения, основываясь на знании кода, который будет их обрабатывать. Точно так же мы знаем, каким должен быть результат этой обработки. Знание всех особенностей тестируемой программы и ее реализации – обязательны для этой техники. Тестирование белого ящика – углубление во внутреннее устройство системы, за пределы ее внешних интерфейсов.
Техника белого ящика применима на разных уровнях тестирования – от модульного до системного, но главным образом применяется именно для реализации модульного тестирования компонента его автором.
Преимущества:
– тестирование может производиться на ранних этапах: нет необходимости ждать создания пользовательского интерфейса;
– можно провести более тщательное тестирование, с покрытием большого количества путей выполнения программы.
Недостатки:
– для выполнения тестирования белого ящика необходимо большое количество специальных знаний
Основным методом тестирования Белого ящика является анализ покрытия кода. Анализ покрытия кода устраняет пробелы в наборе тестовых примеров. Он определяет области программы, которые не покрываются набором Test case. После выявления пробелов вы создаете контрольные примеры для проверки непроверенных частей кода, тем самым повышая качество программного продукта.
<ul>
<li>Охват операторов: - Этот метод требует, чтобы каждое возможное утверждение в коде было проверено хотя бы один раз в процессе тестирования разработки ПО.
</li>
<li>Покрытие ветвления - этот метод проверяет все возможные пути (если-еще и другие условные циклы) программного приложения.
</li>
</ul>
Помимо вышесказанного, существует множество типов покрытия, таких как покрытие условий, покрытие нескольких условий, покрытие пути, покрытие функций и т. д. Каждый метод имеет свои достоинства и пытается протестировать (охватить) все части программного кода. Используя покрытие Statement и Branch, вы обычно достигаете 80-90% покрытия кода, что является достаточным.
<h2>Что означает тестирование серого ящика? (Grey box)</h2>
Тестирование методом серого ящика – метод тестирования ПО, который предполагает комбинацию White Box и Black Box подходов. То есть, внутреннее устройство программы нам известно лишь частично. Предполагается, например, доступ к внутренней структуре и алгоритмам работы ПО для написания максимально эффективных тест-кейсов, но само тестирование проводится с помощью техники черного ящика, то есть, с позиции пользователя. Либо нам не доступна внутренняя реализация функций, но мы знаем на уровень ниже, чем пользователи – интерфейсы/эндпоинты и т.п.
Техника серого ящика применима на разных уровнях тестирования – от модульного до системного, но главным образом применяется на интеграционном уровне для проверки взаимодействия разных модулей программы.
Пример тестирования «серого ящика»: при тестировании веб-сайтов на битые ссылки, если тестировщик сталкивается с какой-либо проблемой с этими ссылками, он может сразу же внести изменения в HTML-код и проверить в реальном времени.
Методы:
<ul>
<li>Матричное тестирование: этот метод тестирования включает в себя определение всех переменных, которые существуют в их программах. 
</li>
<li>Регрессионное тестирование: чтобы проверить, повлияло ли изменение в предыдущей версии другие аспекты программы в новой версии. 
</li>
<li>Тестирование ортогональных массивов или OAT: обеспечивает максимальное покрытие кода с минимальным количеством тестов. 
</li>
<li>Pattern testing: это тестирование выполняется на данных истории предыдущих дефектов системы. В отличие от тестирования черного ящика, в тестировании серого ящика копаются в коде и определяют причину сбоя.
</li>
</ul>
<h2>Основные отличия White/grey/black box?</h2>
<img src="https://lh3.googleusercontent.com/zLG0Og9z_pcH-Idqhj7-uH6TwRb0fMhaICI-Q5ITCmwDUpIq59SURBm0A4oeF6LRdubXzgIB270UsdoLnZSSv9QnHU2h5ohHWljsyaEVLaDPOiPUemtso56lkV7gewnYVpy2_5j5">
<h2>Что такое пирамида / уровни тестирования? (Testing Levels)</h2>
«Пирамида тестов» — метафора, которая означает группировку тестов программного обеспечения по разным уровням детализации. Она также дает представление, какое количество тестов должно быть в каждой из этих групп. 
<img src="https://lh6.googleusercontent.com/5AXlFPyJejfB3ItXS0NeMSKHTa_ty2lmavi4C_8B2Q2f5lovFxiRoWe32kdt7dIdeffo8qCoFsxXV-vnIemrOELuOeKidwk4ZdeLeOdSdBSQl77_amcF9dkZDo7QCwm1QXqHNMY8">
… В тесте более высокого уровня вы не тестируете всю условную логику и пограничные случаи, которые уже покрыты юнит-тестами более низкого уровня. Убедитесь, что тест высокого уровня фокусируется только на том, что не покрыто тестами более низкого уровня.
Правило трех А(AAA) (arrange, act, assert) или триада «дано, когда, тогда» — хорошая мнемоника, чтобы поддерживать хорошую структуру тестов. 

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/post/358950/">Пирамида тестов на практике</a>
</li>
<li><a href="https://habr.com/ru/post/358178/">Антипаттерны тестирования ПО</a>
</li>
<li><a href="https://telegra.ph/Unit-API-i-GUI-testy--chem-otlichayutsya-02-11">Unit, API и GUI тесты — чем отличаются</a>
</li>
<li><a href="https://dou.ua/lenta/columns/test-cases-dev-qa-analyst/">Почему тестировать должны не только QA. Распределяем тест-кейсы между Dev, Analyst и QA</a>
</li>
<li><a href="https://martinfowler.com/articles/practical-test-pyramid.html">The Practical Test Pyramid</a>
</li>
<li><a href="https://martinfowler.com/bliki/TestPyramid.html">Test Pyramid</a>
</li>
</ul>
<h2>Что такое деструктивное/разрушающее/негативное тестирование? (DT - Destructive testing)</h2>
ОТРИЦАТЕЛЬНОЕ ТЕСТИРОВАНИЕ - тип тестирования ПО для поиска точек отказа в программном обеспечении, который проверяет систему на обработку исключительных ситуаций (срабатывание валидаторов на некорректные данные), а также проверяет, что вызываемая приложением функция не выполняется при срабатывании валидатора. Неожиданные условия могут быть чем угодно, от неправильного типа данных до хакерской атаки. Целью отрицательного тестирования является предотвращение сбоя приложений из-за некорректных входных данных. Просто проводя положительное тестирование, мы можем только убедиться, что наша система работает в нормальных условиях. Мы должны убедиться, что наша система может справиться с непредвиденными условиями, чтобы обеспечить 100% безошибочную систему.
Типичные примеры: ввести неправильно составленный e-mail и номер телефона, загрузить файл не предусмотренного расширения или размера. 
Для деструктивного тестирования существует множество способов его тестирования: 
<ul>
<li>Метод анализа точек отказа: это пошаговое прохождение системы, проводящее оценку того, что может пойти не так в разных точках. Для этой стратегии может быть использована помощь BA (Business Analyst). 
</li>
<li>Экспертная проверка тестировщика: проанализируйте или дайте на ревью ваши Test вашему коллеге-тестировщику, который менее знаком с системой/функцией 
</li>
<li>Бизнес-анализ тестовых случаев. Конечные пользователи или эксперты могут подумать о многих допустимых сценариях, которые иногда тестировщики могут не учитывать или упустить, так как все их внимание будет сосредоточено на тестировании требований. 
</li>
<li>Проведите предварительное тестирование с использованием контрольных таблиц (run sheets). Исследовательское тестирование с использованием контрольных таблиц поможет определить, что было проверено, повторить тесты и позволит вам контролировать охват тестами. 
</li>
<li>Используйте другой источник: вы можете попросить кого-нибудь сломать программный продукт и проанализировать различные сценарии.
</li>
</ul>

Доп. материал:
<a href="https://testmatick.com/ru/top-10-negativnyh-test-kejsov-ispolzuemyh-vo-vremya-testirovaniya-po/">Топ 10 негативных кейсов</a>
<h2>Что такое недеструктивное/неразрушающее/позитивное тестирование? (NDT – Non Destructive testing)</h2>
НЕДЕСТРУКТИВНОЕ ТЕСТИРОВАНИЕ - это тип тестирования программного обеспечения, который включает в себя правильное взаимодействие с программным обеспечением. Другими словами, неразрушающее тестирование (NDT) также можно назвать позитивным тестированием или тестированием «счастливого пути». Это дает ожидаемые результаты и доказывает, что программное обеспечение ведет себя так, как ожидалось. Пример: - Ввод правильных данных в модуль входа в систему и проверка, принимает ли он учетные данные и переходит на следующую страницу
<h2>Что подразумевается под компонентным/модульным/юнит тестированием? (Component/Module/Unit testing)</h2>
С этими терминами происходит путаница и даже глоссарий ISTQB не проясняет ситуацию. Обычно эти термины используют как синонимы, а конкретика варьируется от компании к компании. Но если копнуть и попробовать разобраться, получается примерно следующее:
Модульное тестирование (юнит-тестирование). Модульные тесты используются для тестирования какого-либо одного логически выделенного и изолированного элемента системы (отдельные методы класса или простая функция, subprograms, subroutines, классы или процедуры) в коде. Очевидно, что это тестирование методом белого ящика и чаще всего оно проводится самими разработчиками. Целью тестирования модуля является не демонстрация правильного функционирования модуля, а демонстрация наличия ошибки в модуле, а также в определении степени готовности системы к переходу на следующий уровень разработки и тестирования. На уровне модульного тестирования проще всего обнаружить дефекты, связанные с алгоритмическими ошибками и ошибками кодирования алгоритмов, типа работы с условиями и счетчиками циклов, а также с использованием локальных переменных и ресурсов. Ошибки, связанные с неверной трактовкой данных, некорректной реализацией интерфейсов, совместимостью, производительностью и т.п. обычно пропускаются на уровне модульного тестирования и выявляются на более поздних стадиях тестирования. Изоляция тестируемого блока достигается с помощью заглушек (stubs), манекенов (dummies) и макетов (mockups). Являясь по способу исполнения структурным тестированием или тестированием "белого ящика", модульное тестирование характеризуется степенью, в которой тесты выполняют или покрывают логику программы (исходный текст). Тесты, связанные со структурным тестированием, строятся по следующим принципам:
<ul>
<li>На основе анализа потока управления. В этом случае элементы, которые должны быть покрыты при прохождении тестов, определяются на основе структурных критериев тестирования С0, С1,С2. К ним относятся вершины, дуги, пути управляющего графа программы (УГП), условия, комбинации условий и т. п.
</li>
<li>На основе анализа потока данных, когда элементы, которые должны быть покрыты, определяются при помощи потока данных, т. е. информационного графа программы.
</li>
</ul>
Тестирование на основе потока управления. Особенности использования структурных критериев тестирования С0,С1,С2 были рассмотрены ранее. К ним следует добавить критерий покрытия условий, заключающийся в покрытии всех логических (булевских) условий в программе. Критерии покрытия решений (ветвей - С1) и условий не заменяют друг друга, поэтому на практике используется комбинированный критерий покрытия условий/решений, совмещающий требования по покрытию и решений, и условий.
К популярным критериям относятся критерий покрытия функций программы, согласно которому каждая функция программы должна быть вызвана хотя бы один раз, и критерий покрытия вызовов, согласно которому каждый вызов каждой функции в программе должен быть осуществлен хотя бы один раз. Критерий покрытия вызовов известен также как критерий покрытия пар вызовов (call pair coverage).
Тестирование на основе потока данных. Этот вид тестирования направлен на выявление ссылок на неинициализированные переменные и избыточные присваивания (аномалий потока данных ). Предложенная там стратегия требовала тестирования всех взаимосвязей, включающих в себя ссылку (использование) и определение переменной, на которую указывает ссылка (т. е. требуется покрытие дуг информационного графа программы). Недостаток стратегии в том, что она не включает критерий С1, и не гарантирует покрытия решений.
Стратегия требуемых пар также тестирует упомянутые взаимосвязи. Использование переменной в предикате дублируется в соответствии с числом выходов решения, и каждая из таких требуемых взаимосвязей должна быть протестирована. К популярным критериям принадлежит критерий СР, заключающийся в покрытии всех таких пар дуг v и w, что из дуги v достижима дуга w, поскольку именно на дуге может произойти потеря значения переменной, которая в дальнейшем уже не должна использоваться. Для "покрытия" еще одного популярного критерия Cdu достаточно тестировать пары (вершина, дуга), поскольку определение переменной происходит в вершине УГП, а ее использование - на дугах, исходящих из решений, или в вычислительных вершинах.
Методы проектирования тестовых путей для достижения заданной степени тестированности в структурном тестировании. Процесс построения набора тестов при структурном тестировании принято делить на три фазы:
<ul>
<li>Конструирование УГП.
</li>
<li>Выбор тестовых путей.
</li>
<li>Генерация тестов, соответствующих тестовым путям.
</li>
</ul>
Первая фаза соответствует статическому анализу программы, задача которого состоит в получении графа программы и зависящего от него и от критерия тестирования множества элементов, которые необходимо покрыть тестами. На третьей фазе по известным путям тестирования осуществляется поиск подходящих тестов, реализующих прохождение этих путей. Вторая фаза обеспечивает выбор тестовых путей. Выделяют три подхода к построению тестовых путей:
<ul>
<li>Статические методы.
</li>
<li>Динамические методы.
</li>
<li>Методы реализуемых путей.
</li>
</ul>
Статические методы. Самое простое и легко реализуемое решение - построение каждого пути посредством постепенного его удлинения за счет добавления дуг, пока не будет достигнута выходная вершина управляющего графа программы. Эта идея может быть усилена в так называемых адаптивных методах, которые каждый раз добавляют только один тестовый путь (входной тест), используя предыдущие пути (тесты) как руководство для выбора последующих путей в соответствии с некоторой стратегией. Чаще всего адаптивные стратегии применяются по отношению к критерию С1. Основной недостаток статических методов заключается в том, что не учитывается возможная нереализуемость построенных путей тестирования.
Динамические методы. Такие методы предполагают построение полной системы тестов, удовлетворяющих заданному критерию, путем одновременного решения задачи построения покрывающего множества путей и тестовых данных. При этом можно автоматически учитывать реализуемость или нереализуемость ранее рассмотренных путей или их частей. Основной идеей динамических методов является подсоединение к начальным реализуемым отрезкам путей дальнейших их частей так, чтобы: 1) не терять при этом реализуемости вновь полученных путей; 2) покрыть требуемые элементы структуры программы.
Методы реализуемых путей. Данная методика заключается в выделении из множества путей подмножества всех реализуемых путей. После чего покрывающее множество путей строится из полученного подмножества реализуемых путей.
Достоинство статических методов состоит в сравнительно небольшом количестве необходимых ресурсов, как при использовании, так и при разработке. Однако их реализация может содержать непредсказуемый процент брака (нереализуемых путей). Кроме того, в этих системах переход от покрывающего множества путей к полной системе тестов пользователь должен осуществить вручную, а эта работа достаточно трудоемкая. Динамические методы требуют значительно больших ресурсов как при разработке, так и при эксплуатации, однако увеличение затрат происходит, в основном, за счет разработки и эксплуатации аппарата определения реализуемости пути (символический интерпретатор, решатель неравенств). Достоинство этих методов заключается в том, что их продукция имеет некоторый качественный уровень - реализуемость путей. Методы реализуемых путей дают самый лучший результат.
Компонентное тестирование — тип тестирования ПО, при котором тестирование выполняется для каждого отдельного компонента отдельно, без интеграции с другими компонентами. Его также называют модульным тестированием (Module testing), если рассматривать его с точки зрения архитектуры. Как правило, любое программное обеспечение в целом состоит из нескольких компонентов. Тестирование на уровне компонентов (Component Level testing) имеет дело с тестированием этих компонентов индивидуально. Это один из самых частых типов тестирования черного ящика, который проводится командой QA. Для каждого из этих компонентов будет определен сценарий тестирования, который затем будет приведен к Test case высокого уровня -> детальным Test case низкого уровня с предварительными условиями.
Исходя из глубины уровней тестирования, компонентное тестирование можно классифицировать как:
<ul>
<li>Тестирование компонентов в малом (CTIS — Component testing In Small). Тестирование компонентов может проводиться с или без изоляции остальных компонентов в тестируемом программном обеспечении или приложении. Если это выполняется с изоляцией другого компонента, то это называется CTIS. Пример: веб-сайт, на котором есть 5 разных веб-страниц, тестирование каждой веб-страницы отдельно и с изоляцией других компонентов.
</li>
</ul>
<ul>
<li>Тестирование компонентов в целом (CTIL — Component testing In Large). Тестирование компонентов, выполненное без изоляции других компонентов в тестируемом программном обеспечении или приложении, называется CTIL. Давайте рассмотрим пример, чтобы понять это лучше. Предположим, что есть приложение, состоящее из трех компонентов, таких как Компонент A, Компонент B и Компонент C. Разработчик разработал компонент B и хочет его протестировать. Но для того, чтобы полностью протестировать компонент B, некоторые его функции зависят от компонента A, а некоторые — от компонента C. Функциональный поток: A -> B -> C, что означает, что существует зависимость от B как от A, так и от C, заглушка - вызываемая функция, а драйвер - вызывающая функция. Но компонент A и компонент C еще не разработаны. В этом случае, чтобы полностью протестировать компонент B, мы можем заменить компонент A и компонент C заглушкой и драйверами по мере необходимости. Таким образом, в основном, компоненты A & C заменяются заглушками и драйверами, которые действуют как фиктивные объекты до тех пор, пока они фактически не будут разработаны.
</li>
</ul>

<table>
<tr>
<td>Unit testing
</td><td>Component testing
</td></tr>
<tr>
<td>Тестирование отдельных программ, модулей, функций для демонстрации того, что программа выполняется согласно спецификации
</td><td>Тестирование каждого объекта или частей программного обеспечения отдельно с или без изоляции других объектов
</td></tr>
<tr>
<td>Проверка в(на) соответствии с design documents
</td><td>Проверка в(на) соответствии с test requirements, use case
</td></tr>
<tr>
<td>Пишутся и выполняются(обычно) разработчиками
</td><td>Тестировщиками
</td></tr>
<tr>
<td>Выполняется первым
</td><td>Выполняется после Unit
</td></tr>
</table>

Другой источник:
Разница между компонентным и модульным тестированием: По-существу эти уровни тестирования представляют одно и тоже, разница лишь в том, что в компонентном тестировании в качестве параметров функций используют реальные объекты и драйверы, а в модульном тестировании - конкретные значения.

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/company/skyeng/blog/521324/">Я сомневался в юнит-тестах, но…</a>
</li>
<li><a href="https://habr.com/ru/company/qiwi/blog/510608/">Юнит-тесты переоценены</a>
</li>
</ul>
<h2>Что подразумевается под интеграционным тестированием? (Integration testing)</h2>
Интеграционное тестирование предназначено для проверки насколько хорошо два или более модулей ПО взаимодействуют друг с другом, а также взаимодействия с различными частями системы (операционной системой, оборудованием либо связи между различными системами). С технологической точки зрения интеграционное тестирование является количественным развитием модульного, поскольку так же, как и модульное тестирование, оперирует интерфейсами модулей и подсистем и требует создания тестового окружения, включая заглушки ( Stub ) на месте отсутствующих модулей. Основная разница между модульным и интеграционным тестированием состоит в целях, то есть в типах обнаруживаемых дефектов, которые, в свою очередь, определяют стратегию выбора входных данных и методов анализа. В частности, на уровне интеграционного тестирования часто применяются методы, связанные с покрытием интерфейсов, например, вызовов функций или методов, или анализ использования интерфейсных объектов, таких как глобальные ресурсы, средства коммуникаций, предоставляемых операционной системой. Больше: <a href="https://www.intuit.ru/studies/courses/48/48/lecture/1432?page=1">https://www.intuit.ru/studies/courses/48/48/lecture/1432?page=1</a>
Уровни интеграционного тестирования:
<ul>
<li>Компонентный интеграционный уровень (Component Integration testing): Проверяется взаимодействие между компонентами системы после проведения компонентного тестирования.
</li>
<li>Системный интеграционный уровень (System Integration testing): Проверяется взаимодействие между разными системами после проведения системного тестирования.
</li>
</ul>
Подходы к интеграционному тестированию:
<ul>
<li>Подход Большого взрыва:
</li>
<li>Инкрементальный подход:
</li>
<ul>
<li>Нисходящий подход
</li>
<li>Подход снизу-вверх
</li>
<li>Сэндвич-подход
</li>
</ul>
</ul>
Некоторые утверждают, что всех участников (например, вызываемые классы) тестируемого субъекта следует заменить на имитации (mocks) или заглушки (stubs), чтобы создать идеальную изоляцию, избежать побочных эффектов и сложной настройки теста. Другие утверждают, что на имитации и заглушки следует заменять только участников, которые замедляют тест или проявляют сильные побочные эффекты (например, классы с доступом к БД или сетевыми вызовами). Иногда эти два вида юнит-тестов называют одинокими (solitary) в случае тотального применения имитаций и заглушек или общительными (sociable) в случае реальных коммуникаций с другими участниками.
Информация должна приходить в течение нескольких секунд или нескольких минут с быстрых тестов на ранних этапах конвейера. И наоборот, более длительные тесты — обычно с более широкой областью — размещаются на более поздних этапах, чтобы не тормозить фидбек от быстрых тестов. Как видите, этапы конвейера развертывания определяются не типами тестов, а их скоростью и областью действия. Поэтому очень разумно может быть разместить некоторые из самых узких и быстрых интеграционных тестов на ту же стадию, что и юнит-тесты — просто потому что они дают более быструю обратную связь
Доп. материал:
<ul>
<li><a href="https://tproger.ru/articles/integracionnye-testy-v-mikroservisah/">Интеграционные тесты в микросервисах</a>
</li>
<li><a href="https://intuit.ru/studies/courses/48/48/lecture/1434">Лекция 6: Интеграционное тестирование и его особенности для объектно-ориентированного программирования</a>
</li>
</ul>
<h2>Разница между Unit testing и Integration testing?</h2>
Именно здесь больше всего споров о названиях. «Область» интеграционных тестов также весьма противоречива, особенно по характеру доступа к приложению (тестирование в черном или белом ящике; разрешены mock-объекты или нет). На практике получается так: если тест…
<ul>
<li>использует базу данных,
</li>
<li>использует сеть для вызова другого компонента/приложения,
</li>
<li>использует внешнюю систему (например, очередь или почтовый сервер),
</li>
<li>читает/записывает файлы или выполняет другие операции ввода-вывода,
</li>
<li>полагается не на исходный код, а на бинарник приложения,
</li>
</ul>
… то это интеграционный, а не модульный тест

<img src="https://lh3.googleusercontent.com/rfOAqBWrJ5y_D6_tgcJGp9M-lEIlWxeAn3zWxYMDaXkL-6T-CBgymdtHlZ0HKuucvZyejFqKUHcO_a0HKenap6WnPkl4KBj5Mz4RWkMAKWEfGRluxPIXbMPcUJ9qC9tQunT55rTV">
Подведем итог: хотя теоретически можно использовать только интеграционные тесты, на практике
<ul>
<li>Юнит-тесты легче поддерживать.
</li>
<li>Юнит-тесты легко воспроизводят пограничные случаи и редкие ситуации.
</li>
<li>Юнит-тесты выполняются гораздо быстрее интеграционных тестов.
</li>
<li>Сбойные юнит-тесты легче исправить, чем интеграционные.
</li>
</ul>
Если у вас есть только интеграционные тесты, то вы впустую тратите и время разработки, и деньги компании. Нужны как модульные, так и интеграционные тесты одновременно. Они не взаимоисключающие.
<h2>Что такое системное интеграционное тестирование? (SIT - System Integration testing)</h2>
Это тип тестирования программного обеспечения, проводимого в интегрированной аппаратной и программной среде для проверки поведения всей системы. Это тестирование, проведенное на полной интегрированной системе для оценки соответствия системы ее установленным требованиям. SIT выполняется для проверки взаимодействия между модулями программной системы. Оно занимается проверкой требований к программному обеспечению высокого и низкого уровня, указанных в Software Requirements Specification/Data and the Software Design Document. Он также проверяет сосуществование программной системы с другими и тестирует интерфейс между модулями программного приложения. В этом типе тестирования модули сначала тестируются индивидуально, а затем объединяются в систему. Например, программные и / или аппаратные компоненты объединяются и тестируются постепенно, пока не будет интегрирована вся система.
<h2>Что подразумевается под инкрементальным подходом? (Incremental Approach)</h2>
При таком подходе тестирование выполняется путем объединения двух или более логически связанных модулей. Затем другие связанные модули поэтапно добавляются и тестируются для правильного функционирования. Процесс продолжается до тех пор, пока все модули не будут соединены и успешно протестированы. Осуществляется двумя разными методами: Снизу-вверх и сверху-вниз.
<h2>Что подразумевается под подходом снизу-вверх? (Bottom-Up Approach)</h2>
В восходящей стратегии каждый модуль на более низких уровнях последовательно тестируется с более высокоуровневыми модулями, пока не будут протестированы все модули. Требуется помощь драйверов для тестирования. Данный подход считается полезным, если все или практически все модули, разрабатываемого уровня, готовы. Также данный подход помогает определить по результатам тестирования уровень готовности приложения.
Преимущества: Локализация ошибок проще. Не тратится время на ожидание разработки всех модулей, в отличие от подхода Большого взрыва 
Недостатки: Критические модули (на верхнем уровне архитектуры ПО), которые контролируют поток приложения, тестируются последними и могут быть подвержены дефектам. Ранний прототип невозможен.
<img src="https://lh5.googleusercontent.com/3OXvBS-5b6ClVPNOksMO1nO9IuG5l4IKpcFcTfVFAJkb0ABby7wsdZu_8YflWOaFT0WGud9rXRkTZrBO8wzz7put0eWDqSpLkDu1Gb-VghigbKFfrIbiN5RMm55YKiZB-BG-6k2Y">
<h2>Что подразумевается под подходом сверху-вниз? (Top-Down Approach)</h2>
Вначале тестируются все высокоуровневые модули, и постепенно один за другим добавляются низкоуровневые. Все модули более низкого уровня симулируются заглушками с аналогичной функциональностью, затем по мере готовности они заменяются реальными активными компонентами.
Преимущества: Локализация неисправностей проще. Возможность получить ранний прототип. Основные недостатки дизайна могут быть найдены и исправлены в первую очередь. Недостатки: Нужно много заглушек. Модули на более низком уровне тестируются недостаточно.
<img src="https://lh6.googleusercontent.com/aqen2464jdbgFFAsX0OdNWGyfQyLGfE5BPoDwYCCX0GMSGZrZyCwT5hkw7CLsvGItmPtYpC0pzL4f2IBfg1hivyYTGFH6KIGQzJkzU6DLU8tv3gmz9syYNb1D1RFncXtc4qNZ-X7">
<h2>Что подразумевается под гибридным/сэндвич-подходом? (Sandwich Approach)</h2>
Представляет собой комбинацию подходов сверху вниз и снизу-вверх. Здесь верхние модули тестируются с нижними модулями, а нижние модули интегрируются с верхними модулями и тестируются. Эта стратегия использует и заглушки и драйверы.
<img src="https://lh3.googleusercontent.com/9SvWxP9sbOEcigN9CBYsXwTnLlbGOhhbd_SqazHOgRmtOwoYPiExZtubi2qgFmcxOuSDU6OKnc6RBYdm5_FL8cHfpLJ1iaq7Tr4UAdrOfFCydpQ-0K_vAsQhgyzXo-7kNfnxCmO8">
<h2>Что подразумевается под подходом Большого взрыва?  (Big Bang Approach)</h2>
Все или практически все разработанные модули собираются вместе в виде законченной системы или ее основной части, и затем проводится интеграционное тестирование. Такой подход очень хорош для сохранения времени. Однако если Test case и их результаты записаны не верно, то сам процесс интеграции сильно осложнится, что станет преградой для команды тестирования при достижении основной цели интеграционного тестирования
<h2>В чем разница между тест-драйвером и тест-заглушкой? (Test Driver and Test Stub)</h2>
Тестовый драйвер - это фрагмент кода, который вызывает тестируемый программный компонент. Это полезно при тестировании по принципу «снизу-вверх». Тестовая заглушка - это фиктивная программа, которая интегрируется с приложением для полной функциональности. Они актуальны для тестирования, в котором используется нисходящий подход. Давайте возьмем пример. 
1. Допустим, есть сценарий для проверки интерфейса между модулями A и B. Мы разработали только модуль-A. Затем мы можем проверить модуль-A, если у нас есть реальный модуль-B или фиктивный модуль для него. В этом случае мы называем модуль-B тестовой заглушкой. 
2. Теперь модуль B не может отправлять или получать данные напрямую из модуля A. В таком сценарии мы перемещаем данные из одного модуля в другой, используя некоторые внешние функции, называемые Test Driver.
Заглушки и драйверы не реализуют всю логику программного модуля, а только моделируют обмен данными с вызывающим модулем. Заглушка: вызывается тестируемым модулем. Драйвер: вызывает модуль для тестирования.
<h2>Что подразумевается под системным тестированием? </h2>
Системное тестирование качественно отличается от интеграционного и модульного уровней. Системное тестирование рассматривает тестируемую систему в целом и оперирует на уровне пользовательских интерфейсов, в отличие от последних фаз интеграционного тестирования, которое оперирует на уровне интерфейсов модулей. Различны и цели этих уровней тестирования. На уровне системы часто сложно и малоэффективно анализировать прохождение тестовых траекторий внутри программы или отслеживать правильность работы конкретных функций. Основная задача системного тестирования - в выявлении дефектов, связанных с работой системы в целом, таких как неверное использование ресурсов системы, непредусмотренные комбинации данных пользовательского уровня, несовместимость с окружением, непредусмотренные сценарии использования, отсутствующая или неверная функциональность, неудобство в применении и тому подобное.
Системное тестирование производится над проектом в целом с помощью метода "черного ящика". Структура программы не имеет никакого значения, для проверки доступны только входы и выходы, видимые пользователю.
Категории тестов системного тестирования:
<ul>
<li>Полнота решения функциональных задач.
</li>
<li>Стрессовое тестирование - на предельных объемах нагрузки входного потока.
</li>
<li>Корректность использования ресурсов (утечка памяти, возврат ресурсов).
</li>
<li>Оценка производительности.
</li>
<li>Эффективность защиты от искажения данных и некорректных действий.
</li>
<li>Проверка инсталляции и конфигурации на разных платформах.
</li>
<li>Корректность документации
</li>
</ul>
Для минимизации рисков, связанных с особенностями поведения системы в той или иной среде, во время тестирования рекомендуется использовать окружение максимально приближенное к тому, на которое будет установлен продукт после выдачи. Системное тестирование относят к черному ящику.
Можно выделить два подхода к системному тестированию:
<ul>
<li>на базе требований (requirements based): Для каждого требования пишутся <a href="http://www.protesting.ru/testing/testcase.html">Test case</a>, проверяющие выполнение данного требования.
</li>
<li>на базе случаев использования (use case based): На основе представления о способах использования продукта создаются случаи использования системы (Use Cases). По конкретному случаю использования можно определить один или более сценариев. На проверку каждого сценария пишутся <a href="http://www.protesting.ru/testing/testcase.html">Test case</a>, которые должны быть протестированы.
</li>
</ul>
Доп. материал:
<a href="https://intuit.ru/studies/courses/48/48/lecture/1436">Лекция 7: Разновидности тестирования: системное и регрессионное тестирование</a>

<h2>Можем ли мы провести системное тестирование на любом этапе? </h2>
Нет. Системное тестирование следует начинать, только если все модули написаны и работают правильно. Тем не менее, это должно произойти до UAT (пользовательского приемочного тестирования).
<h2>Что такое функциональное тестирование?</h2>
Функциональное тестирование рассматривает заранее указанное поведение и основывается на анализе спецификаций функциональности компонента или системы в целом.
Функциональные тесты основываются на функциях, выполняемых системой, и могут проводиться на всех уровнях тестирования (компонентном, интеграционном, системном, приемочном). Как правило, эти функции описываются в требованиях, функциональных спецификациях или в виде случаев использования системы (use cases).
Тестирование в перспективе «требования» использует спецификацию функциональных требований к системе как основу для дизайна Test case. В этом случае необходимо сделать список того, что будет тестироваться, а что нет, приоритезировать требования на основе рисков (если это не сделано в документе с требованиями), а на основе этого приоритезировать тестовые сценарии. Это позволит сфокусироваться и не упустить при тестировании наиболее важный функционал.
Тестирование в перспективе «бизнес-процессы» использует знание этих самых бизнес-процессов, которые описывают сценарии ежедневного использования системы. В этой перспективе тестовые сценарии (test scripts), как правило, основываются на случаях использования системы (use cases).
Преимущества функционального тестирования:
<ul>
<li>имитирует фактическое использование системы;
</li>
</ul>
Недостатки функционального тестирования:
<ul>
<li>возможность упущения логических ошибок в программном обеспечении;
</li>
<li>вероятность избыточного тестирования.
</li>
</ul>
<h2>Что такое тестирование совместимости/взаимодействия? (Compatibility/Interoperability testing)</h2>
Тестирование взаимодействия - функциональное тестирование, проверяющее способность приложения/устройства взаимодействовать с одним и более компонентами/системами/устройствами и включающее в себя тестирование совместимости (compatibility testing) и интеграционное тестирование (integration testing). 
ПО с хорошими характеристиками взаимодействия может быть легко интегрировано с другими системами, не требуя каких-либо серьезных модификаций. В этом случае, количество изменений и время, требуемое на их выполнение, могут быть использованы для измерения возможности взаимодействия. Например, тестирование совместимости проводится между смартфонами и планшетами для проверки передачи данных через Bluetooth.
Существуют разные уровни тестирования совместимости:
<ul>
<li>Аппаратное обеспечение: проверяет совместимость программного обеспечения с различными аппаратными конфигурациями. 
</li>
<li>Операционные системы: Он проверяет ваше программное обеспечение на совместимость с различными операционными системами, такими как Windows, Unix*, Mac OS и т. д. 
</li>
<li>Программное обеспечение: проверяет ваше разработанное программное обеспечение на совместимость с другим программным обеспечением. Например, приложение MS Word должно быть совместимо с другими программами, такими как MS Outlook, MS Excel, VBA и т. д. 
</li>
<li>Сеть: оценка производительности системы в сети с различными параметрами, такими как пропускная способность, скорость работы, емкость. 
</li>
<li>Браузер: проверяет совместимость вашего сайта с различными браузерами, такими как Firefox, Google Chrome, Internet Explorer и т. д. 
</li>
<li>Устройства: проверяет совместимость вашего программного обеспечения с различными устройствами, такими как устройства USB-порта, принтеры и сканеры, другие мультимедийные устройства и Bluetooth. 
</li>
<li>Mobile: проверка совместимости вашего программного обеспечения с мобильными платформами, такими как Android, iOS и т. д. 
</li>
<li>Версии программного обеспечения. Он проверяет совместимость вашего программного приложения с различными версиями программного обеспечения. Например, проверка вашего Microsoft Word на совместимость с Windows 7, Windows 7 SP1, Windows 7 SP2, Windows 7 SP3.
</li>
</ul>
Существует два типа проверки версий:
<ul>
<li>Тестирование обратной совместимости предназначено для проверки поведения разработанного аппаратного / программного обеспечения с использованием более старых версий аппаратного / программного обеспечения. 
</li>
<li>Тестирование прямой совместимости заключается в проверке поведения разработанного аппаратного / программного обеспечения с использованием более новых версий аппаратного / программного обеспечения.
</li>
</ul>
Пример тестирования взаимодействия: 
<ul>
<li>Подключите (connect) два или более устройств от разных производителей 
</li>
<li>Проверьте связь между устройствами 
</li>
<li>Проверьте, может ли устройство отправлять / получать пакеты или фреймы друг от друга 
</li>
<li>Проверьте, правильно ли обрабатываются данные на уровне сети и объектов 
</li>
<li>Проверьте, правильно ли работают реализованные алгоритмы 
</li>
<li>Результат в порядке: проверьте следующий результат. Результат не в порядке: используйте инструменты мониторинга, чтобы обнаружить источник ошибки 
</li>
<li>Отчет о результатах в тестовом отчете.
</li>
</ul>
<h2>Что такое тестирование на соответствие? (Conformance/Compilance testing)</h2>
CONFORMANCE testing - это тип тестирования программного обеспечения, который удостоверяет, что система программного обеспечения соответствует стандартам и правилам, определенным IEEE, W3C или ETSI. Цель проверки соответствия состоит в том, чтобы определить, в какой степени отдельная реализация конкретного стандарта соответствует индивидуальным требованиям этого стандарта. Включает в себя: 
<ul>
<li>Производительность
</li>
<li>Функции 
</li>
<li>Прочность (Robustness)
</li>
<li>Совместимость (Interoperability) 
</li>
<li>Поведение системы
</li>
</ul>
Тестирование соответствия может быть логическим или физическим, и оно включает в себя следующие типы тестирования: 
<ul>
<li>Тестирование на соответствие (Compliance testing)
</li>
<li>Нагрузочное тестирование (<a href="https://www.guru99.com/load-testing-tutorial.html">Load testing</a>)
</li>
<li>Стресс тестирование (<a href="https://www.guru99.com/stress-testing-tutorial.html">Stress testing</a>)
</li>
<li>Объемное тестирование (Volume testing)
</li>
</ul>

<table>
<tr>
<td>Conformance testing
</td><td>Compliance testing
</td></tr>
<tr>
<td>Conformance является формальным и точным способом тестирования стандартов
</td><td>Compliance является неформальным и менее точным способом тестирования стандартов
</td></tr>
<tr>
<td>Сертификация Conformance применима только к операционной системе, имеющей официальный Certification Authority
</td><td>Операционная система, которая обеспечивает единый API (Portable Operating System Interface), считается совместимой
</td></tr>
<tr>
<td>Conformance testing используется для тестирования системы, которая обеспечивает полную поддержку данных стандартов
</td><td>Compliance testing используется для тестирования системы, обеспечивающей поддержку некоторых из указанных стандартов
</td></tr>
</table>
Тестирование соответствия также называется Type testing, который является формальным способом тестирования.
<h2>Что такое нефункциональное тестирование?</h2>
НЕФУНКЦИОНАЛЬНОЕ тестирование определяется как тип тестирования ПО для проверки нефункциональных аспектов ПО. Оно предназначено для проверки готовности системы по нефункциональным параметрам, которые никогда не учитываются при функциональном тестировании.
<ul>
<li>Нефункциональное тестирование должно повысить удобство использования, эффективность, ремонтопригодность и portability продукта. 
</li>
<li>Помогает снизить производственный риск и затраты, связанные с нефункциональными аспектами продукта. 
</li>
</ul>
Позволяет:
<ul>
<li>оптимизировать способ установки, настройки, выполнения, управления и мониторинга продукта. 
</li>
<li>Собирать и производить измерения и метрики для внутренних исследований и разработок. 
</li>
<li>Улучшать и расширять знания о поведении продукта и используемых технологиях.
</li>
</ul>

Основные нефункциональные типы тестирования:
<ul>
<li>Производительности (Performance)
</li>
<ul>
<li>Стрессовое (Stress testing)
</li>
<li>Тестирование емкости/способностей (Capacity testing)
</li>
<li>Нагрузочное (Load testing)
</li>
<li>Объемное тестирование (Volume testing)
</li>
<li>Выносливости/стабильности/надежности (Soak/Endurance/Stability/Reliability testing)
</li>
<li>Шиповое (Spike)
</li>
<li>Масштабируемости (Scalability Test)
</li>
</ul>
<li>Тестирование времени отклика (Response Time testing)
</li>
<li>Тестирование на отказоустойчивость (Failover testing)
</li>
<li>Тестирование совместимости (Compatibility testing)
</li>
<li>Тестирование на удобство пользования (Usability testing)
</li>
<li>Тестирование на поддерживаемость/ремонтопригодность (Maintainability testing)
</li>
<li>Тестирование безопасности (Security testing)
</li>
<li>Тестирование аварийного восстановления (Disaster Recovery testing)
</li>
<li>Тестирование на соответствие (Compliance testing)
</li>
<li>Тестирование переносимости (Portability testing)
</li>
<li>Тестирование эффективности (Efficiency testing)
</li>
<li>Базовое тестирование (Baseline testing)
</li>
<li>Тестирование документации (Documentation testing)
</li>
<li>Тестирование восстановления (Recovery testing)
</li>
<li>Интернационализация (Globalization/Internationalization testing)
</li>
<li>Тестирование локализации (Localization testing)
</li>
</ul>
<h2>Основные понятия в тестировании производительности?</h2>
<ul>
<li>Время задержки (Latency) - временной интервал между запросом и ответом. Например, у вашего сервиса время задержки составляет 100ms, что означает, что такому сервису потребуется 100 миллисекунд на обработку запроса и генерирование ответа. Как правило, чем ниже время задержки, тем лучше клиентский опыт.
</li>
<li>Время ответа (Response time) - время, необходимое для ответа на запрос 
</li>
<li>Пропускная способность (Throughput) - фактическое количество запросов (или пользователей), которое может обработать система за определенное время. В то время как время задержки говорит вам только о времени, метрика пропускной способности информирует об объеме данных, полученных и обработанных в момент времени. Важно не отделять показатели времени задержки от пропускной способности, т.к. высокий показатель времени задержки часто прямо связан с увеличением показателей метрики пропускной способности. Пропускная способность обычно измеряется в rps – (кол-во) запросов в секунду (requests per second).
</li>
<li>Ширина пропускания канала (Bandwidth) - максимальное число запросов (или пользователей), которое может обработать система. В отличие от пропускной способности ширина пропускания канала измеряет максимальный объем, который может обработать приложение.
</li>
<li>Транзакции в секунду. Пользовательские транзакции – это последовательность действий пользователя в интерфейсе. Сравнивая реальное время прохождения транзакции с ожидаемой (или количество транзакций в секунду), вы сможете сделать вывод о том, насколько успешной системой было пройдено нагрузочное тестирование.
</li>
<li>Процент ошибок рассчитывается как отношение невалидных ответов к валидным за промежуток времени.
</li>
<li>Про Average, медианы, перцентили и т.п. углубляться в рамках этой статьи не буду, есть в гугле.
</li>
</ul>
<h2>Тестирование производительности клиентской части и серверной, в чем разница?</h2>
Оценка скорости работы клиентской и серверной частей веб-приложения осуществляется двумя разными видами тестирования: для Frontend применяется тестирование клиентской части, или Client-Side testing, а для Back-end – тестирование серверной части.
Основная цель тестирования клиентской части состоит в измерении времени, необходимого браузеру, для загрузки HTML-страницы. Наиболее важными показателями здесь являются количество загружаемых данных, их объем, а также количество выполненных запросов.
Собрать данную статистику можно как с использованием встроенных инструментов браузера (DevTools), так и с помощью специализированных инструментов и онлайн-сервисов, которые позволяют замерить необходимые показатели с учетом интересующего региона.
Помимо общего веса страницы, инструменты предоставляют детализированную информацию по каждому из компонентов. Изучив параметры запросов, можно обнаружить ряд проблем, приводящих к ухудшению скорости отображения страницы. К примеру, подгружается слишком большая картинка и Javascript, или отправляется значительное количество запросов.
Другая необходимая проверка направлена на анализ заголовков кэширования, поскольку корректность его выполнения при повторном посещении страницы позволяет повысить скорость загрузки страницы до 80%.
Тестирование серверной части направлено на анализ выполнения запросов и получения соответствующего ответа от Back-end.
Цели данного вида тестирования:
<ul>
<li>Измерить время отклика самых важных бизнес-транзакций;
</li>
<li>Определить предельный уровень допустимой нагрузки;
</li>
<li>Выявить «узкие» места в производительности системы;
</li>
<li>Составить рекомендации по улучшению производительности;
</li>
<li>Найти возможные дефекты, проявляющиеся только при одновременной работе большого количества пользователей.
</li>
</ul>

<h2>В общем виде что такое тестирование производительности?</h2>
Это класс тестирования ПО, который фокусируется на производительности системы при определенной нагрузке. Он не ищет напрямую ошибки или дефекты. Он производит аналитику на основе эталонных тестов и предоставляет разработчику всю диагностическую информацию, необходимую для выявления проблем производительности и узких мест. При этом происходит:
<ul>
<li>измерение времени выполнения выбранных операций при определенных интенсивностях выполнения этих операций
</li>
<li>определение количества пользователей, одновременно работающих с приложением
</li>
<li>определение границ приемлемой производительности при увеличении нагрузки (при увеличении интенсивности выполнения этих операций)
</li>
<li>исследование производительности на высоких, предельных, стрессовых нагрузках
</li>
</ul>

Важно понимать, что все подвиды тестирования производительности это, грубо говоря, одно и то же, просто в зависимости от конкретного подвида выбираются разные параметры (показатели нагрузки/пользователей, длительности и т.п.) и собираются соответствующие метрики. Точкой отсчета принято брать результаты Capacity testing. 
В реальном мире проводят только часть из перечисленных подвидов в соответствии с бюджетом и приоритетами данного ПО, а параметры тестов и метрики могут корректироваться в разных ситуациях.

<img src="https://lh6.googleusercontent.com/XNuV1_4ya69jlZ7lkW-Dovc1xycy-zvrcGAKyoQxni7AITleD6eO4lsHsIp2PVA-CzpHCFrCX0MX9vBZRMHroN9i1YfDD70rIL0VdNq2593APZqVDkF-cVpLSByaOXR8XXTFuvgB">
Небольшая заметка. Несмотря на необходимость понимания многих математических и статистических концепций, многие тестировщики и менеджеры либо не имеют достаточных знаний в области математики и статистики, либо не пользуются ими. Это приводит к значительным искажениям и неверной интерпретации результатов тестирования производительности. Поэтому хороший специалист должен обладать и смежными знаниями.

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/company/tinkoff/blog/514314/">Анализ результатов нагрузочного тестирования</a>
</li>
<li><a href="https://habr.com/ru/company/vdsina/blog/536304/">Нагрузочное тестирование выполнять сложно, а инструменты далеки от совершенства. Почему?</a>
</li>
<li><a href="https://tproger.ru/articles/nagruzochnoe-testirovanie-osobennosti-professii/">Нагрузочное тестирование: особенности профессии</a>
</li>
</ul>

<h2>Что такое тестирование емкости/способностей? (Capacity)</h2>
Capacity — базовый тест, который обычно выполняется первым. Все последующие тесты на среднее время ответа, регенерацию системы, утилизацию ресурсов нужно выполнять с оглядкой на результаты Capacity. Емкость системы измеряется в rps (requests per second). Используемый подход: ступенчато повышаем нагрузку до момента, когда время ответа начнет расти экспоненциально. Экспоненциальный рост времени ответа, как правило, связан с полной утилизацией одного из ресурсов, из-за которого запросы вместо моментальной обработки выстраиваются друг за другом и ждут своей очереди на обработку. 
<img src="https://lh5.googleusercontent.com/NFbeBOzq9h_517Zw0uK569eq3k0kWY2BBiORQVKKTa1Gqi0EuS3KeYNQ2Y5NfI7fpFJexd1CaC4SeDhXDz4Be9oS_ryYROMbNHoJ-CKOFinOHxeNH4r6Oh50lgxHyYDxxUgarqGw">
Capacity point – точка, где перестает расти Throughput, но увеличивается Response Time, то есть система перестает справляться с запросами.
Исходя из этого тестирования выбираются значения для stress, load и soak/endurance тестов. Для stress берется значение близкое к capacity point, но немного меньше. Для load количество пользователей из зоны деградации. 
Важно, ваша цель, не получить кол-во rps, при котором все взрывается, а понять, какой именно ресурс станет узким местом, при повышении нагрузки. Поэтому, если обстреливаемый вами сервер не покрыт мониторингом — можете даже не начинать тест. Общий подход к сбору телеметрии — чем больше метрик собирается, тем лучше.
В некоторых случаях Capacity называют так же Scalability (масштабируемость), но в целом это не равнозначные понятия.
<h2>Что означает тестирование масштабируемости? (Scalability)</h2>
Профиль нагрузки тот же, что и при нагрузочном тестировании. Что получаем в результате? Ответы на следующие вопросы:
<ul>
<li>Увеличится ли производительность приложения, если добавить дополнительные аппаратные ресурсы?
</li>
<li>Увеличится ли производительность пропорционально количеству добавленных аппаратных средств?
</li>
</ul>
Разница между тестированием емкости/способностей и тестированием масштабируемости? (Capacity vs Scalability)
Тестирование масштабируемости - это тестирование программного приложения для измерения его способности увеличивать или уменьшать масштаб с точки зрения любых его нефункциональных возможностей. Тестирование производительности, масштабируемости и надежности обычно группируется аналитиками качества ПО. 
Тестирование емкости измеряет, сколько пользователей может обработать приложение. Это подмножество тестирования масштабируемости, в котором при тестировании масштабируемости вы получите меру емкости приложения. Тестирование масштабируемости измеряет, насколько хорошо приложение справляется с растущим числом пользователей. Если вы тестируете масштабируемость до тех пор, пока приложение не выйдет из строя, у вас будет мера того, сколько пользователей (емкость) может обработать приложение.
<h2>Расскажите о стрессовом тестировании? (Stress testing)</h2>
Стрессовое тестирование выполняется самым первым, если нет отдельного Capacity тестирования, хотя по факту это все равно будет Capacity, т.к. нагрузка берется «с потолка». Позволяет проверить насколько приложение и система в целом работоспособны в условиях высокой нагрузки. Нагрузка на систему будет возрастать непрерывно до тех пор, пока не будет достигнут один из критериев его остановки. Пример: стресс-тест банковской системы был остановлен при превышении отметки в 1500 пользователей, когда высокая загруженность процессора (более 80%) привела к увеличению среднего времени отклика в пять раз и массовому появлению ошибок HTTP(S).
<img src="https://lh3.googleusercontent.com/aIJG3A1Mujx5ChXCbyeoY7SBwy06KdJSOjREYmcbiBXJdUdBDMxypKzoxodqx3l4JU7ouVi2zLrmZw8OSOHy_QxwxuYZc2qh65G2VOhuqVSrponf-MQNWmAFGwacN8luIGCaoRmc">
<h2>Расскажите о нагрузочном тестировании? (Load)</h2>
Нагрузочное тестирование - это тестирование, имитирующее работу определенного количества бизнес пользователей на каком-либо общем (разделяемом ими) ресурсе. Этот тип тестирования производительности выполняется для диагностики поведения системы при увеличении рабочей нагрузки.
Нагрузка на систему обычно подается на протяжении 1-2 часов (в некоторых источниках: 4-8 часов, хотя это уже больше endurance), количество пользователей для нагрузочного теста берется из зоны деградации (в некоторых источниках: определяется в количестве 80% от результата максимальной производительности). В это время собираются метрики производительности: количество запросов в секунду, транзакций в секунду, время отклика от сервера, процент ошибок в ответах, утилизация аппаратных ресурсов и т. д. 
<img src="https://lh3.googleusercontent.com/KQDgZCIEO4LqnoxMqJNaTZ3F7_bxgN7oKJfQzY_uw7FUdT8ssHCirc5E1J9l6L9lF_PXaVQIg6J1M1YsQiLv7MTAaccr3w2WmB3_0BSxo454ossgqrPGDAErf2eal5Pt0IUycExM">

<h2>Что такое объемное тестирование? (Volume testing)</h2>
Объемное тестирование предназначено для прогнозирования того, может ли система / приложение обрабатывать большой объем данных. Это тестирование сосредоточено на наполнении базы данных продукта в реальных сценариях использования.
Пример 1: отправка через POST-запросы очень большого количества данных. 
Пример 2: как изменится производительность приложения спустя X лет, если аудитория приложения вырастет в Y раз?
<h2>Тестирование выносливости/стабильности/надежности (Soak/Endurance/Stability/Reliability testing)</h2>
Задачей тестирования стабильности является проверка работоспособности приложения при длительном (многочасовом) тестировании со средним уровнем нагрузки. Время выполнения операций может играть в данном виде тестирования второстепенную роль. При этом на первое место выходит проверка на утечки памяти, время отклика, правильность подключения и закрытия подключения к модулям (например, БД) и т.п. в течение длительного времени, чтобы гарантировать, что после длительного периода время отклика системы останется таким же или лучше, чем на начало теста. Этот тип тестирования выполняется в самом конце (а где-то по ночам). Так же он помогает управлять будущими нагрузками, ведь нам необходимо понять, сколько дополнительных ресурсов (таких как ЦП, емкость диска, использование памяти или пропускная способность сети) необходимы для поддержки использования в будущем.
<h2>Что такое спайк/шиповое тестирование? (Spike)</h2>
Этот вид тестирования предназначен для определения поведения системы при внезапном увеличении нагрузки (большого количества пользователей) на систему. Например, дни распродаж в интернет-магазине.
<h2>Что такое тестирование устойчивости? (Resilence)</h2>
Проверка устойчивости проводится для того, чтобы убедиться, что система способна вернуться в исходное состояние после кратковременного напряжения. Например, если в интернет-магазине действует скидка на определенные товары на короткое время, скажем, один час в день.

Доп.материал:
<a href="https://github.com/Netflix/chaosmonkey">Chaos Monkey</a>
<h2>Что такое тестирование времени отклика? (Response time testing)</h2>
Время ответа относится ко времени, которое требуется одному системному узлу для ответа на запрос другого. Среднее время ответа - это среднее время, затрачиваемое на каждый запрос в оба конца. Пиковое время отклика помогает нам определить, какие компоненты потенциально проблематичны. Коэффициент ошибок - это математический расчет, который отображает процент проблемных запросов. Три критических значения времени отклика: 0,1 секунды, 1,0 секунды и 10 секунд.
<h2>Что такое Ramp тестирование? </h2>
Это метод тестирования, который предлагает ступенчато поднимать нагрузку до тех пор, пока система не выйдет из строя. 
<h2>Что такое тестирование хранилища? (Storage testing)</h2>
Тестирование хранилища определяется как тип тестирования программного обеспечения, который проверяет, сохраняет ли тестируемое приложение соответствующие данные в соответствующих каталогах и достаточно ли у него места для предотвращения неожиданного завершения из-за недостатка дискового пространства. Это также называется тестированием производительности хранилища (Storage Performance testing).
Зачем оно нужно? 
<ul>
<li>Медленное хранилище означает медленное время отклика, длительные запросы и более низкую availability приложений. 
</li>
<li>Медленное хранилище - это накладные расходы на обслуживание серверной инфраструктуры. 
</li>
<li>Также помогает найти практическое ограничение хранилища перед деплоем. 
</li>
<li>Помогает понять, как система будет реагировать при замене или обновлении аппаратного обеспечения.
</li>
</ul>
Типы:
<ul>
<li>Application testing: Тестирование приложений с примерами запросов в production like environment
</li>
<ul>
<li>Сравните время ответа OLTP 
</li>
<li>Сравните время выполнения batch 
</li>
<li>Сравните rates непрерывной потоковой передачи
</li>
</ul>
<li>Application Simulation: Проведите тестирование с использованием стандартного программного обеспечения, аналогичного целевому приложению 
</li>
<ul>
<li>Протестировать на пиковые значения IOPS для баз данных 
</li>
<li>Тест пика для data streaming environments 
</li>
<li>Проверка задержек хранилища для обмена сообщениями или других однопоточных приложений
</li>
</ul>
<li>Benchmarking: Провести тестирование с использованием стандартного программного обеспечения. 
</li>
<ul>
<li>Проверка на повреждение данных.
</li>
</ul>
</ul>
<h2>Что такое тестирование на отказ и восстановление? (Failover and Recovery testing)</h2>
Тестирование на отказ и восстановление (Failover and Recovery testing) проверяет тестируемый продукт с точки зрения способности противостоять и успешно восстанавливаться после возможных сбоев, возникших в связи с ошибками ПО, отказами оборудования или проблемами связи/сети. Целью данного вида тестирования является проверка систем восстановления (или дублирующих основной функционал систем), которые, в случае возникновения сбоев, обеспечат сохранность и целостность данных тестируемого продукта.
Тестирование на отказ и восстановление очень важно для систем, работающих по принципу "24x7". Если Вы создаете продукт, который будет работать, например, в интернете, то без проведения данного вида тестирования Вам просто не обойтись. Т.к. каждая минута простоя или потеря данных в случае отказа оборудования, может стоить вам денег, потери клиентов и репутации на рынке.
Методика подобного тестирования заключается в симулировании различных условий сбоя и последующем изучении, и оценке реакции защитных систем. В процессе подобных проверок выясняется, была ли достигнута требуемая степень восстановления системы после возникновения сбоя.
Для наглядности рассмотрим некоторые варианты подобного тестирования и общие методы их проведения. Объектом тестирования в большинстве случаев являются весьма вероятные эксплуатационные проблемы, такие как:
<ul>
<li>Отказ электричества на компьютере-сервере
</li>
<li>Отказ электричества на компьютере-клиенте
</li>
<li>Незавершенные циклы обработки данных (прерывание работы фильтров данных, прерывание синхронизации).
</li>
<li>Объявление или внесение в массивы данных невозможных или ошибочных элементов.
</li>
<li>Отказ носителей данных.
</li>
</ul>
Стоит заметить, что тестирование на отказ и восстановление – это весьма продукт-специфичное тестирование. Разработка тестовых сценариев должна производиться с учетом всех особенностей тестируемой системы. Принимая во внимание довольно жесткие методы воздействия, стоит также оценить целесообразность проведения данного вида тестирования для конкретного программного продукта.
<h2>Что вы знаете о Тестировании удобства пользования? (Usability testing)</h2>
Тестирование удобства пользования - это метод тестирования, направленный на установление степени удобства использования, обучаемости, понятности и привлекательности для пользователей разрабатываемого продукта в контексте заданных условий.
Тестирование удобства пользования дает оценку уровня удобства использования приложения по следующим пунктам:
<ul>
<li>производительность, эффективность (efficiency) - сколько времени и шагов понадобится пользователю для завершения основных задач приложения, например, размещение новости, регистрации, покупка и т. д. ? (меньше - лучше)
</li>
<li>правильность (accuracy) - сколько ошибок сделал пользователь во время работы с приложением? (меньше - лучше)
</li>
<li>активизация в памяти (recall) – как много пользователь помнит о работе приложения после приостановки работы с ним на длительный период времени? (повторное выполнение операций после перерыва должно проходить быстрее чем у нового пользователя)
</li>
<li>эмоциональная реакция (emotional response) – как пользователь себя чувствует после завершения задачи - растерян, испытал стресс? Порекомендует ли пользователь систему своим друзьям? (положительная реакция - лучше)
</li>
</ul>
Проверка удобства использования может проводиться как по отношению к готовому продукту, посредством тестирования черного ящика (black box testing), так и к интерфейсам приложения (API), используемым при разработке - тестирование белого ящика (white box testing). В этом случае проверяется удобство использования внутренних объектов, классов, методов и переменных, а также рассматривается удобство изменения, расширения системы и интеграции ее с другими модулями или системами. Использование удобных интерфейсов (API) может улучшить качество, увеличить скорость написания и поддержки разрабатываемого кода, и как следствие улучшить качество продукта в целом.
Отсюда становится очевидно, что тестирование удобства пользования может производиться на разных уровнях разработки ПО: модульном, интеграционном, системном и приемочном.


Доп. материал:
<a href="https://vc.ru/marketing/200995-vkusnyy-i-zdorovyy-gayd-po-yuzabiliti-testirovaniyam">Вкусный и здоровый гайд по юзабилити-тестированиям</a>
<h2>Отличия тестирование на удобство пользования и тестирования доступности? (Usability Vs. Accessibility testing)</h2>
USABILITY testing показывает, насколько проста в использовании и удобна система программного обеспечения. Здесь небольшой набор целевых конечных пользователей «использует» программную систему для выявления дефектов юзабилити. Основное внимание в этом тестировании уделяется простоте использования приложения пользователем, гибкости в управлении средствами управления и способности системы выполнять свои задачи. Это также называется тестированием пользовательского опыта (UX – "Ю-Экс", user experience). Это тестирование рекомендуется на начальном этапе разработки SDLC, что позволяет лучше понять ожидания пользователей. Исследования (Virzi, 1992 и Neilsen Landauer, 1993) показывают, что 5 пользователей достаточно для выявления 80% проблем с юзабилити, хотя некоторые исследователи предлагают другие цифры.
Тестирование доступности (accessibility testing) - это подмножество юзабилити-тестирования. Его цель - убедиться в том, что наш продукт удобен в использовании для людей с различными видами инвалидности или особенностей восприятия. Это могут быть проблемы со зрением, слухом или ограничения в подвижности рук. 
Ваш продукт должен правильно работать с соответствующим ПО. Примеры такого программного обеспечения:
<ul>
<li>Speech Recognition Software - ПО преобразует произнесенное слово в текст, который служит вводом для компьютера. 
</li>
<li>Программа для чтения с экрана - используется для озвучивания текста, отображаемого на экране 
</li>
<li>Программное обеспечение для увеличения экрана - используется для увеличения масштаба элементов и облегчения чтения для пользователей с нарушениями зрения. 
</li>
<li>Специальная клавиатура, облегчающая ввод для пользователей, у которых проблемы с двигательными функциями.
</li>
</ul>
Еще один из примеров - люди с цветовой слепотой (дальтонизмом). Эта особенность довольно широко распространена. Различными видами цветовой слепоты страдают около 8 % мужчин и 0,4 % женщин - не так уж мало!
Цвет не должен быть единственным способом передачи информации. Если вы используете цвет для того, чтобы, допустим, отобразить статус, эту информацию стоит продублировать еще каким-то образом - геометрическими фигурами, иконками или текстовым комментарием. 
Хорошая контрастность. Хорошая контрастность обеспечивает нормальную видимость элементов управления и текста даже для людей, не различающих те или иные оттенки.
Есть отличный инструмент для тестирования веб-сайтов на предмет доступности для людей с различными формами цветовой слепоты: Color Blind Web Page Filter.
 <img src="https://lh3.googleusercontent.com/yq2LgYAT7WG6k1-uARt38HzPsKtfIFZCL2YaSwdVI-50X6uXChgPjaiiQFsARtf06z4aPVGlaATms2MH_WSPNvn2yafEGQ3G8_lEoPFXzliwCNU9S37fqsUbrEyG5p6CrdyYEsdY">
Если вы хотите сократить количество тестов, можно ограничиться только тремя фильтрами: дейтеранопия, протанопия и тританопия. Это наиболее выраженные формы цветовой слепоты (не считая крайне редкого черно-белого зрения). Остальные люди с особенностями цветовосприятия видят больше оттенков, и если ваш UI достаточно хорошо виден с этими тремя фильтрами, то и для остальных будет отображаться корректно.
Пример чек-листа:
<ul>
<li>Предоставляет ли приложение клавиатурные эквиваленты для всех действий мышью и окон? 
</li>
<li>Предоставляются ли инструкции как часть пользовательской документации или руководства? Легко ли понять и использовать приложение, используя документацию? 
</li>
<li>Упорядочены ли вкладки логически для обеспечения плавной навигации? 
</li>
<li>Предусмотрены ли сочетания клавиш для меню? 
</li>
<li>Поддерживает ли приложение все операционные системы? 
</li>
<li>Четко ли указано время отклика каждого экрана или страницы, чтобы конечные пользователи знали, как долго ждать? 
</li>
<li>Все ли надписи правильно написаны? 
</li>
<li>Являются ли цвета подходящим для всех пользователей? 
</li>
<li>Правильно ли используются изображения или значки, чтобы их было легко понять конечным пользователям? 
</li>
<li>Есть ли звуковые оповещения? 
</li>
<li>Может ли пользователь настроить аудио или видео элементы управления? 
</li>
<li>Может ли пользователь переопределить шрифты по умолчанию для печати и отображения текста? 
</li>
<li>Может ли пользователь настроить или отключить мигание, вращение или перемещение элементов? 
</li>
<li>Убедитесь, что цветовое кодирование никогда не используется в качестве единственного средства передачи информации или указания на действие 
</li>
<li>Видна ли подсветка с инвертированными цветами? 
</li>
<li>Тестирование цвета в приложении путем изменения контрастности 
</li>
<li>Правильно ли слышат люди с ограниченными возможностями все имеющее отношение к аудио и видео?
</li>
<li>Протестируйте все мультимедийные страницы без мультимедиа-оборудования. 
</li>
<li>Предоставляется ли обучение пользователям с ограниченными возможностями, что позволит им ознакомиться с программным обеспечением или приложением?
</li>
</ul>

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/company/redmadrobot/blog/504110/">QA и его роль в создании ресурсов для людей с ограниченными возможностями</a>
</li>
<li><a href="https://habr.com/ru/company/edison/blog/474472/">Чеклист по UX из 30 пунктов для мобильных приложений</a>
</li>
<li><a href="https://cdn2.hubspot.net/hubfs/5358007/WCAG_2.1_Checklist.pdf">Web Content Accessibility Guidelines</a>
</li>
</ul>
<h2>Что такое тестирование интерфейса?</h2>
Это тип интеграционного теста, который проверяет, правильно ли установлена ​​связь между двумя различными программными системами или их частями (модулями). Соединение, которое объединяет два компонента, называется интерфейсом. Этот интерфейс в компьютерном мире может быть чем угодно, как API, так и веб-сервисами и т. д.  Тестирование этих подключаемых сервисов или интерфейса называется Тестированием интерфейса.
Тестирование интерфейса включает в себя тестирование двух основных сегментов: 
<ul>
<li>Интерфейс веб-сервера и сервера приложений 
</li>
<li>Интерфейс сервера приложений и базы данных
</li>
</ul>
<h2>Что такое тестирование рабочего процесса/воркфлоу? (Workflow testing)</h2>
Это тип тестирования программного обеспечения, который проверяет, что каждый software workflow точно отражает данный бизнес-процесс. Workflow - это серия задач для получения желаемого результата, которая обычно включает несколько этапов или шагов. Для любого бизнес-процесса тестирование этих последовательных шагов определяется как «WorkFlow testing».
Например, убедитесь, что система может быть установлена ​​на платформе пользователя и работает правильно. Тестирование рабочего процесса проводится поэтапно. Вот как вы будете выполнять Workflow testing:
<ul>
<li>Начальная фаза (Inception phase): эта фаза включает начальное планирование испытаний и тестирование прототипа 
</li>
<li>Фаза разработки (Elaboration phase): Эта фаза включает базовую архитектуру тестирования 
</li>
<li>Фаза строительства (Construction phase): эта фаза включает в себя значительные испытания в каждой сборке 
</li>
<li>Фаза перехода (Transition phase): Эта фаза включает в себя регрессионные тесты и повторные тесты исправлений
</li>
</ul>
Тестирование workflow выполняется:
<ul>
<li>Test engineer: планирует цели теста и график. Определяет Test case и процедуры. Оценивает результаты теста.
</li>
<li>Component engineer: Разработка тестовых компонентов. Автоматизирует некоторые тестовые процедуры.
</li>
<li>Integration Tester: Выполнение интеграционных тестов и выявление дефектов 
</li>
<li>System Testers: Выполнение системных тестов и отчеты о дефектах
</li>
</ul>
<h2>Что вы знаете о пользовательском приемочном тестировании? (UAT – User Acceptance testing)</h2>
Пользовательское приемочное тестирование (UAT) - это тип тестирования, выполняемый конечным пользователем или клиентом для проверки / принятия ПО перед его перемещением в production. UAT выполняется на заключительном этапе тестирования после выполнения функциональных, интеграционных и системных испытаний. Основной целью UAT является проверка end-to-end business flow. Он не фокусируется на косметических ошибках, орфографических ошибках или тестировании системы. Приемочное тестирование пользователя выполняется в отдельной среде тестирования с настройкой данных, аналогичных производственным. Это своего рода тестирование черного ящика, в котором будут участвовать два или более конечных пользователя. Этапы:
<ul>
<li>Анализ бизнес-требований 
</li>
<li>Создать плана тестирования UAT 
</li>
<li>Определить Test Scenario 
</li>
<li>Создать Test case UAT 
</li>
<li>Подготовить Test Data (Production like Data) 
</li>
<li>Запустить Test case
</li>
<li>Записать результаты
</li>
<li>Подтвердить бизнес-цели
</li>
</ul>
<h2>Что такое эксплуатационное приемочное тестирование? (OAT - Operational Acceptance testing)</h2>
ИСПЫТАНИЕ НА ЭКСПЛУАТАЦИЮ (OAT) - это тип тестирования программного обеспечения, который оценивает операционную готовность программного приложения до его выпуска в производство. Целью эксплуатационного тестирования является обеспечение бесперебойной работы системы в ее стандартной операционной среде (SOE - standard operating environment). Это также называется Оперативное тестирование (Operational testing). Эксплуатационное приемочное тестирование обеспечивает соответствие системы и компонентов в стандартной операционной среде приложения (SOE). Типы OAT:
<ul>
<li>Installation testing
</li>
<li>Load & Performance Test Operation
</li>
<li>Backup and Restore testing
</li>
<li><a href="https://www.guru99.com/what-is-security-testing.html">Security testing</a>
</li>
<li>Code Analysis
</li>
<li>Fail over testing
</li>
<li>Recovery testing
</li>
<li>End-to-End<a href="https://www.guru99.com/test-environment-software-testing.html"> Test Environment </a>Operational testing
</li>
<li>Operational Documentation Review
</li>
</ul>
Примеры Test case:
<ul>
<li>Резервные копии, сделанные на одном сайте, могут быть развернуты на тот же сайт 
</li>
<li>Резервные копии, сделанные на одном сайте, можно развернуть на другом сайте. 
</li>
<li>Внедрение любых новых функций в живую производственную среду не должно отрицательно влиять на целостность текущих производственных услуг. 
</li>
<li>Процесс внедрения может быть воспроизведен с использованием действующей документации 
</li>
<li>Каждый компонент может быть отключен и успешно запущен в согласованные сроки. 
</li>
<li>Для оповещений - все критические оповещения должны идти в TEC и ссылаться на документ правильного разрешения. 
</li>
<li>Оповещения созданы и выдаются при превышении согласованных пороговых значений 
</li>
<li>Любая документация по восстановлению, созданная или измененная, включая сервисные диаграммы, действительна 
</li>
<li>Это должно быть передано в соответствующие области поддержки. 
</li>
<li>Любой компонент, на который влияет сбой, должен показывать рекомендуемый порядок перезапуска, время завершения и т. д. 
</li>
</ul>
<h2>Расскажите об инсталляционном тестировании?</h2>
Тестирование инсталляции (установки) направленно на проверку успешной инсталляции и настройки, а также обновления или удаления ПО, как десктопного, так и мобильного.
Тестирование инсталляции в большинстве своем не входит в Веб-тестирование, являясь специализированным тестированием установки приложений на различные операционные системы.
Следующие проверки должны быть выполнены для этапов:
Установка. 
<ul>
<li>Установка должна начаться при клике по кнопке, подтверждающей данное действие
</li>
<li>Установки во всех поддерживаемых окружениях и на всех поддерживаемых платформах
</li>
<li>Установки в неподдерживаемых окружениях, а также в нужных окружениях с некорректными настройками
</li>
<li>Права, которые требует инсталляция (чаще всего они должны быть админскими), проверить установить приложение как гость
</li>
<li>Установки в clean state (при отсутствии любых возможных связанных файлов и предыдущих версий)
</li>
<li>Подсчитывается ли при установке количество свободного места на диске и выдается ли предупреждение если места недостаточно
</li>
<li>Установки загруженного ранее приложения, а также прямая установка с использованием сети/беспроводного соединения
</li>
<li>Восстановится ли процесс установки при внезапном его прерывании (отключение устройства, отказ сети, отключение беспроводного соединения)
</li>
<li>Установка приложения, его запуск, удаление приложения должны возвращать систему в исходное состояние
</li>
<li>Распознается ли наличие в системе приложений/программ, необходимых для корректной работы устанавливаемого приложения
</li>
<li>Повторный запуск установки приложения при уже текущем должен выдавать корректное сообщение, двойная установка должна быть исключена
</li>
<li>Процесс установки может быть настраиваемый/дефолтный. Убедиться, что оба корректно работают
</li>
<li>Наличие кнопки, которая предложит сохранить приложение в определенную папку, а также указывает дефолтное местоположение ("C:/programs/.")
</li>
<li>Правильно ли установлены, сохранены ли в корректных папках файлы приложения
</li>
<li>Наличие созданных ярлыков, корректно ли они расположены
</li>
<li>После установки в системной вкладке " Программы и компоненты" должны быть доступны: название приложения, иконка, имя издателя, размер приложения, дата установки и номер версии
</li>
<li>Настройки переменных сред PATH
</li>
<li>Убедиться, что лицензионный ключ сохраняется в Windows Registry library
</li>
<li>Поддерживает ли приложение функции ‘UnInstall’, ‘Modify’, ‘ReInstall’ и корректно ли они работают
</li>
<li>Работа приложения с уже существующими DLL-файлами, с DLL-файлами приложений, которые необходимы для корректной работы устанавливаемого приложения
</li>
<li>Наличие информации/сообщение о том, когда истекает срок действия установленной пробной версии приложения
</li>
</ul>
Обновление:
<ul>
<li>Поддерживает ли приложение функцию обновления/автообновления
</li>
<li>При попытке установить ранее установленную версию приложения система должна ее распознать и выдать корректное сообщение
</li>
<li>Сохраняются ли пользовательские настройки при попытке загрузить новую версию/обновить старую версию
</li>
<li>При попытке обновить версию должны быть доступны функции удалить приложение и восстановить приложение
</li>
<li>Стандартные проверки как при первичной установке приложения
</li>
<li>Убедиться, что номер версии приложения сменился новым
</li>
<li>Запустить приложение и убедиться, что оно работает корректно
</li>
</ul>
Откат до предыдущей версии:
<ul>
<li>Попробовать установить старую версию на более новую
</li>
<li>Наличие корректного сообщения при попытке отката
</li>
<li>Убедиться, что приложение работает корректно
</li>
</ul>
Удаление приложения:
<ul>
<li>Не остается ли в системе никаких папок/файлов/ярлыков/ключей реестра после полного удаления приложения
</li>
<li>Корректно ли работает система после установки и последующего удаления приложения
</li>
</ul>
<h2>Что вы знаете о тестировании безопасности? (Security and Access Control testing)</h2>
Это тип тестирования ПО, который выявляет уязвимости, угрозы и риски. Целью тестов безопасности является выявление всех возможных лазеек и слабых мест в ПО, которые могут привести к потере информации, доходов, репутации компании, сотрудников или клиентов. Общая стратегия безопасности основывается на трех основных принципах:
<ul>
<li>Конфиденциальность - сокрытие определенных ресурсов или информации
</li>
<li>Целостность – ресурс может быть изменен только в соответствии с полномочиями пользователя
</li>
<li>Доступность - ресурсы должны быть доступны только авторизованному пользователю, внутреннему объекту или устройству
</li>
</ul>
Тестирование безопасности обычно выполняет отдельный специалист по безопасности. В ходе тестирования безопасности испытатель играет роль взломщика. Ему разрешено все:
<ul>
<li>попытки узнать пароль с помощью внешних средств;
</li>
<li>атака системы с помощью специальных утилит, анализирующих защиты;
</li>
<li>подавление, ошеломление системы (в надежде, что она откажется обслуживать других клиентов);
</li>
<li>целенаправленное введение ошибок в надежде проникнуть в систему в ходе восстановления;
</li>
<li>просмотр несекретных данных в надежде найти ключ для входа в систему.
</li>
</ul>
При неограниченном времени и ресурсах хорошее тестирование безопасности взломает любую систему. Задача проектировщика системы — сделать цену проникновения более высокой, чем цена получаемой в результате информации.
Типы тестирования безопасности:
<ul>
<li>Сканирование уязвимостей/оценка защищенности (Vulnerability Scanning) выполняется с помощью автоматизированного ПО для сканирования системы на наличие известных сигнатур уязвимостей. 
</li>
<li>Сканирование безопасности (Security Scanning) включает в себя выявление слабых сторон сети и системы, а затем предоставляет решения для снижения этих рисков. Это сканирование может быть выполнено как ручным, так и автоматизированным.
</li>
<li>Тестирование на проникновение (Penetration testing) - этот тип тестирования имитирует атаку злоумышленника. Это тестирование включает анализ конкретной системы для проверки потенциальных уязвимостей при попытке внешнего взлома. 
</li>
<li>Оценка рисков (Risk Assessment) тестирование включает анализ рисков безопасности, наблюдаемых в организации. Риски классифицируются как Низкие, Средние и Высокие. Это тестирование рекомендует меры по снижению риска. 
</li>
<li>Аудит безопасности (Security Auditing) - внутренняя проверка приложений и операционных систем на наличие уязвимостей. Аудит также может быть выполнен путем построчной проверки кода 
</li>
<li>Этический взлом (Ethical hacking) - совершается с целью выявления проблем безопасности в системе. Это делается White Hat хакерами - это специалисты по безопасности, которые использует свои навыки законным способом для помощи в выявлении дефектов системы, в отличии от Black Hat (преступников) или Gray Hat (что-то между).
</li>
<li>Оценка состояния (Posture Assessment) объединяет сканирование безопасности, этический взлом и оценки рисков, чтобы показать общее состояние безопасности организации.
</li>
</ul>

<table>
<tr>
<td>SDLC фаза
</td><td>Security Processes
</td></tr>
<tr>
<td>Requirements
</td><td>Анализ безопасности для требований и проверка случаев злоупотребления / неправильного использования
</td></tr>
<tr>
<td>Design
</td><td>Анализ рисков безопасности для проектирования. Разработка плана тестирования с учетом тестирования безопасности
</td></tr>
<tr>
<td>Coding and Unit testing
</td><td>Статическое и динамическое тестирование безопасности и тестирование белого ящика 
</td></tr>
<tr>
<td>Integration testing
</td><td>Тестирование черного ящика
</td></tr>
<tr>
<td>System testing
</td><td>Тестирование черного ящика и сканирование уязвимостей
</td></tr>
<tr>
<td>Implementation
</td><td>Тестирование на проникновение, сканирование уязвимостей
</td></tr>
<tr>
<td>Support
</td><td>Анализ воздействия патчей
</td></tr>
</table>

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/company/ruvds/blog/537456/">Топ-10 уязвимостей мобильных приложений и способы их устранения</a>
</li>
<li><a href="https://habr.com/ru/post/526878/">Безопасность веб-приложений: от уязвимостей до мониторинга</a>
</li>
<li><a href="https://habr.com/ru/company/group-ib/blog/535092/">Социотехническое тестирование: какое лучше выбрать в 2021 году?</a>
</li>
<li><a href="https://www.youtube.com/playlist?list=PLrCZzMib1e9owORdnWTvZIkSCqRFFbHGA">Анализ безопасности веб-проектов</a>
</li>
<li><a href="https://www.youtube.com/playlist?list=PLrCZzMib1e9qiiSWgZ6pI5HiQzFc4hhdo">Безопасность интернет-приложений</a>
</li>
<li><a href="https://habr.com/ru/company/varonis/blog/524308/">Red Teaming — комплексная имитация атак. Методология и инструменты</a>
</li>
<li><a href="https://www.youtube.com/channel/UCGfxztXUoBeGNVv6UTpUQHw/videos">cHack</a>
</li>
<li><a href="https://owasp.org/www-project-top-ten/">OWASP Top Ten</a>
</li>
<li><a href="https://santoku-linux.com/">Santoku Linux</a> 
</li>
<li><a href="https://www.kali.org/">Kali Linux</a>
</li>
<li><a href="https://github.com/FSecureLABS/drozer">https://github.com/FSecureLABS/drozer</a>
</li>
<li><a href="https://habr.com/ru/post/542190/">SQL-инъекции' union select null,null,null --</a>
</li>
<li><a href="https://www.software-testing.ru/library/testing/security/3398-ross-site-scripting">Что такое XSS-уязвимость и как тестировщику не пропустить ее</a>
</li>
</ul>
<h2>Что означает оценка уязвимости/защищенности? (Vulnerability Assessment)</h2>
Это процесс оценки рисков безопасности в программной системе с целью уменьшения вероятности угрозы. Уязвимость - это любые ошибки или слабости в процедурах безопасности системы, разработке, реализации или любом внутреннем контроле, которые могут привести к нарушению политики безопасности системы. Целью оценки уязвимости является снижение возможности несанкционированного доступа для злоумышленников (хакеров). Анализ проникновения зависит от двух механизмов, а именно от оценки уязвимости и тестирования на проникновение (VAPT - Vulnerability Assessment and Penetration testing).
Методы:
<ul>
<li>Активное тестирование 
</li>
<ul>
<li>Inactive testing, тестировщик вводит новые test data и анализирует результаты. 
</li>
<li>В процессе тестирования тестировщики создают интеллектуальную модель процесса, и она будет расти и дальше во время взаимодействия с тестируемым программным обеспечением. 
</li>
<li>Выполняя тест, тестировщик будет активно вовлекаться в процесс обнаружения новых Test case и новых идей. Вот почему это называется Active testing. 
</li>
</ul>
<li>Пассивное тестирование 
</li>
<ul>
<li>Пассивное тестирование - отслеживание результатов запуска тестируемого программного обеспечения без введения новых Test case или data. 
</li>
</ul>
<li>Тестирование сети 
</li>
<ul>
<li>Тестирование сети - это процесс измерения и записи текущего состояния работы сети за определенный период времени. 
</li>
<li>Тестирование в основном проводится для прогнозирования работы сети под нагрузкой или для выявления проблем, создаваемых новыми сервисами. 
</li>
<li>Нам нужно проверить следующие характеристики сети: 
</li>
<ul>
<li>Уровни утилизации 
</li>
<li>Количество пользователей 
</li>
<li>Использование приложения 
</li>
</ul>
</ul>
<li>Распределенное Тестирование 
</li>
<ul>
<li>Распределенные тесты применяются для тестирования распределенных приложений, то есть приложений, работающих с несколькими клиентами одновременно. По сути, тестирование распределенного приложения означает тестирование его клиентской и серверной частей по отдельности, но с помощью метода распределенного тестирования мы можем протестировать их все вместе. 
</li>
<li>Части теста будут взаимодействовать друг с другом во время теста. Это делает их синхронизированными соответствующим образом. Синхронизация является одним из наиболее важных моментов в распределенном тестировании.
</li>
</ul>
</ul>
<h2>Расскажите подробнее о тестировании на проникновение? (Penetration testing)</h2>
PENETRATION testing - это тип тестирования безопасности, который выявляет уязвимости, угрозы, риски в программном приложении, сети или веб-приложении, которые может использовать злоумышленник. Тестирование на проникновение показывает реальную картину существующей угрозы в системе безопасности и определяет уязвимости организации к ручным атакам. Проведение пентеста на регулярной основе позволит определить технические ресурсы, инфраструктуру, физические и кадровый арсенал содержащие в себе слабые аспекты, которые требуют развития и усовершенствования. Данный вид тестирования выполняется как вручную, так и автоматически и может быть как Black Box, так и Grey и White. Ввиду необходимости наличия специфических знаний и опыта для выполнения этого вида тестирования привлекается отдельный специалист – пентестер. Примеры кейсов тестирования на проникновение:
<ul>
<li>Тест на проникновение в сеть:
</li>
<ul>
<li>выявлении уязвимостей сетевого и системного уровня;
</li>
<li>определение неправильных конфигураций и настроек;
</li>
<li>выявление уязвимости беспроводной сети;
</li>
<li>мошеннические услуги;
</li>
<li>отсутствие <a href="http://withsecurity.ru/kak-pridumat-nadezhnyj-parol-i-zapomnit-ego">надежных паролей</a> и наличие слабых протоколов.
</li>
</ul>
<li><a href="http://withsecurity.ru/pentest-mobilnyh-prilozheniy-na-chto-obratit-vnimanie">Тест на проникновение приложений</a>:
</li>
<ul>
<li>выявление недостатков прикладного уровня;
</li>
<li>подделка запросов;
</li>
<li>применение злонамеренных скриптов;
</li>
<li>нарушение работы управления сеансами;
</li>
<li>и т.п.
</li>
</ul>
<li>Тест на физическое проникновение:
</li>
<ul>
<li>взлом физических барьеров;
</li>
<li>проверка и взлом замков;
</li>
<li>нарушения работы и обход датчиков;
</li>
<li>вывод из строя камер видеонаблюдения;
</li>
<li>и т. д. 
</li>
</ul>
</ul>

<h2>Отличия Vulnerability Assessment от Penetration testing?</h2>
Оба этих вида отличаются друг от друга по силе и задачам, которые они выполняют. Однако для составления исчерпывающего отчета по тестированию уязвимостей рекомендуется сочетание обеих процедур.

<table>
<tr>
<td> 
</td><td>Vulnerability Assessment
</td><td>Penetration testing
</td></tr>
<tr>
<td>Working
</td><td>Нахождений уязвимостей
</td><td>Выявление и использование уязвимостей
</td></tr>
<tr>
<td>Mechanism
</td><td>Обнаружение и сканирование
</td><td>Симуляция
</td></tr>
<tr>
<td>Focus
</td><td>Ширина
</td><td>Глубина
</td></tr>
<tr>
<td>Coverage of Completeness
</td><td>Высокое покрытие
</td><td>Низкое
</td></tr>
<tr>
<td>Cost
</td><td>Низкая стоимость
</td><td>Высокая
</td></tr>
<tr>
<td>Performed By
</td><td>Внутренний персонал
</td><td>Атакующий или пентестер
</td></tr>
<tr>
<td>How often to Run
</td><td>После каждой сборки
</td><td>Реже, зависит от политики безопасности компании и продукта
</td></tr>
<tr>
<td>Result
</td><td>Предоставит частичную информацию об уязвимостях
</td><td>Предоставит полную информацию об уязвимостях
</td></tr>
<tr>
<td>
</td><td>
</td><td>
</td></tr>
</table>
<h2>Что такое Fuzz тестирование?</h2>
FUZZ testing (fuzzing) – это метод тестирования ПО методом черного ящика, один из типов тестирования безопасности, который вводит недействительные или случайные данные, называемые FUZZ, в систему программного обеспечения для обнаружения ошибок кодирования и лазеек в безопасности. Данные вводятся с использованием автоматических или полуавтоматических методов тестирования, после чего система отслеживается на предмет различных исключений, таких как сбой системы или сбой встроенного кода и т. д.  
Обычно fuzzing обнаруживает наиболее серьезные ошибки или дефекты безопасности. Это очень экономически эффективный метод тестирования. Fuzzing - один из самых распространенных методов хакеров, используемых для обнаружения уязвимости системы (сюда относятся популярные SQL- или скриптовые инъекции). Примеры фаззеров:
<ul>
<li>Mutation-Based Fuzzers: изменяет существующие образцы данных для создания новых test data. Это очень простой и понятный подход, он начинается с действительных образцов и постоянно корректирует каждый байт или файл.
</li>
<li>Generation-Based Fuzzers: определяет новые данные на основе ввода модели. Он начинает генерировать ввод с нуля на основе спецификации.
</li>
<li>PROTOCOL-BASED-fuzzer: самый успешный фаззер - это детальное знание тестируемого формата протокола. Понимание зависит от спецификации. Это включает в себя запись массива спецификации в инструмент, а затем с помощью метода генерации тестов на основе модели проходится спецификация и добавляется неравномерность в содержимое данных, последовательность и т. д.  Это также известно как синтаксическое тестирование, грамматическое тестирование, тестирование надежности, и т. д.  Fuzzer может генерировать Test case из существующего или использовать допустимые или недействительные входные данные.
</li>
</ul>

Типы ошибок, обнаруживаемых Fuzz testing:
<ul>
<li>Сбои ассертов и утечки памяти (Assertion failures and memory leaks). Эта методология широко используется для больших приложений, где ошибки влияют на безопасность памяти, что является серьезной уязвимостью. 
</li>
<li>Некорректный ввод (Invalid input). Фаззеры используются для генерирования неверного ввода, который используется для тестирования процедур обработки ошибок, и это важно для программного обеспечения, которое не контролирует его ввод. Простой фаззинг может быть способом автоматизации отрицательного тестирования. 
</li>
<li>Исправление ошибок (Correctness bugs). Fuzzing также может использоваться для обнаружения некоторых типов ошибок «правильности». Например, поврежденная база данных, плохие результаты поиска и т. д. 
</li>
</ul>


Доп. материал:
<a href="https://habr.com/ru/company/tensor/blog/527304/">Фаззинг тестирование веб-интерфейса. Расшифровка доклада</a>
<h2>Можно ли отнести тестирование безопасности или нагрузочное тестирование к функциональным видам тестирования?</h2>
Данные виды во многих источниках относят к нефункциональным видам тестирования, но если это является основной функцией приложения, то можно отнести и к функциональным. 

Мнение:
"<..> Есть функциональное требование: 
"Пользователь должен иметь возможность перевести деньги со своей карты на другую карту по номеру". 
Это функциональное требование (ну, на самом деле это целая тонна требований, но обобщим их до одной user story). 
Оно отвечает на вопрос "какие операции должен уметь выполнять сервис". 
К этой функциональности может предъявляться еще куча требований - по безопасности, по скорости, по отказоустойчивости, и т.д.  Они описывают то, как система должна работать, а не что она должна уметь. 
Нефункциональные требования могут быть критичными, могут блокировать выпуск той или иной функциональности. Но это все еще свойство фичи, а не какая-то самостоятельная ее функция. 
В то же время, есть, например, функциональные требования безопасности, типа "автоматически блокировать транзакции обладающие характеристиками А, Б, В".  © @azshoo
Это снова нас возвращает к тому, что система должна обладать какими-то функциями."
<h2>Что вы знаете о конфигурационном тестировании? (Configuration testing)</h2>
Конфигурационное тестирование (Configuration testing) — специальный вид тестирования, направленный на проверку работы ПО при различных аппаратных и программных конфигурациях системы (заявленных платформах, поддерживаемых драйверах, при различных конфигурациях компьютеров и т. д. )
В зависимости от типа проекта конфигурационное тестирование может иметь разные цели:
<ul>
<li>Проект по профилированию работы системы
Цель Тестирования: определить оптимальную конфигурацию оборудования, обеспечивающую требуемые характеристики производительности и времени реакции тестируемой системы.
</li>
<li>Проект по миграции системы с одной платформы на другую
Цель Тестирования: Проверить объект тестирования на совместимость с объявленным в спецификации оборудованием, операционными системами и программными продуктами третьих фирм.
</li>
</ul>
Для клиент-серверных приложений конфигурационное тестирование можно условно разделить на два уровня (для некоторых типов приложений может быть актуален только один):
<ul>
<li>Серверный
</li>
<li>Клиентский
</li>
</ul>
На первом (серверном) уровне, тестируется взаимодействие выпускаемого ПО с окружением, в которое оно будет установлено:
<ul>
<li>Аппаратные средства (тип и количество процессоров, объем памяти, характеристики сети / сетевых адаптеров и т. д.)
</li>
<li>Программные средства (ОС, драйвера и библиотеки, стороннее ПО, влияющее на работу приложения и т. д.)
</li>
</ul>
Основной упор здесь делается на тестирование с целью определения оптимальной конфигурации оборудования, удовлетворяющего требуемым характеристикам качества (эффективность, портативность, удобство сопровождения, надежность).
На следующем (клиентском) уровне, ПО тестируется с позиции его конечного пользователя и конфигурации его рабочей станции. На этом этапе будут протестированы следующие характеристики: удобство использования, функциональность. Для этого необходимо будет провести ряд тестов с различными конфигурациями рабочих станций:
<ul>
<li>Тип, версия и битность операционной системы (подобный вид тестирования называется кроссплатформенное тестирование)
</li>
<li>Тип и версия Web браузера, в случае если тестируется Web приложение (подобный вид тестирования называется кросс-браузерное тестирование)
</li>
<li>Тип и модель видеоадаптера (при тестировании игр это очень важно)
</li>
<li>Работа приложения при различных разрешениях экрана
</li>
<li>Версии драйверов, библиотек и т. д.  (для JAVA приложений версия JAVA машины очень важна, тоже можно сказать и для .NET приложений касательно версии .NET библиотеки)
</li>
</ul>
и т. д. 
Перед началом проведения конфигурационного тестирования рекомендуется:
<ul>
<li>создавать матрицу покрытия (матрица покрытия - это таблица, в которую заносят все возможные конфигурации),
</li>
<li>проводить приоритезацию конфигураций (на практике, скорее всего, все желаемые конфигурации проверить не получится),
</li>
<li>шаг за шагом, в соответствии с расставленными приоритетами, проверять каждую конфигурацию.
</li>
</ul>
Уже на начальном этапе становится очевидно, что чем больше требований к работе приложения при различных конфигурациях рабочих станций, тем больше тестов нам необходимо будет провести. В связи с этим, рекомендуем, по возможности, автоматизировать этот процесс, так как именно при конфигурационном тестировании автоматизация реально помогает сэкономить время и ресурсы. Конечно же автоматизированное тестирование не является панацеей, но в данном случае оно окажется очень эффективным помощником.
В итоге: конфигурационным называется тестирование совместимости выпускаемого продукта (ПО) с различным аппаратным и программным средствами.
Основные цели - определение оптимальной конфигурации и проверка совместимости приложения с требуемым окружением (оборудованием, ОС и т. д.). Автоматизация конфигурационного тестирования позволяет избежать лишних расходов
Примечание: в ISTQB вообще не говорится о таком виде тестирования как конфигурационное. Согласно глоссарию, данный вид тестирования рассматривается там как тестирование портируемости:
configuration testing: See portability testing.
portability testing: The process of testing to determine the portability of a software product.
<h2>Что подразумевается под проверкой на дым / дымовым тестированием? (Smoke testing)</h2>
Смоук тестирование рассматривается как короткий цикл тестов, выполняемый для каждой новой сборки для подтверждения того, что ПО стартует и выполняет основные функции без критических и блокирующих дефектов. В случае отсутствия таковых дефектов дымовое тестирование объявляется пройденным, и команда QA может начинать дальнейшее тестирование полного цикла, в противном случае, сборка объявляется дефектной, что делает дальнейшее тестирование пустой тратой времени и ресурсов. Сборка возвращается на доработку и исправление.
Аналогами дымового тестирования являются Build Verification testing и Acceptance testing, выполняемые на функциональном уровне командой тестирования, по результатам которых делается вывод о том, принимается или нет установленная версия ПО в тестирование, эксплуатацию или на поставку заказчику.
Если мы говорим про сайт интернет-магазина, то сценарий будет примерно следующим:
<ul>
<li>Сайт открывается
</li>
<li>Можно выбрать случайный товар и добавить его в корзину
</li>
<li>Можно оформить и оплатить заказ
</li>
</ul>
Если мы говорим про мобильное приложение, например, messenger, то:
<ul>
<li>Приложение устанавливается и запускается
</li>
<li>Можно авторизоваться
</li>
<li>Можно написать сообщение случайном контакту
</li>
</ul>

Синонимом в некоторых источниках указан breath testing.
Небольшая шпаргалка по степени важности:
<ul>
<li>smoke - самое важное
</li>
<li>critical path -  повседневное
</li>
<li>extended - все
</li>
</ul>

В русском языке термин ошибочно переводят как проверка дыма, корректнее уж говорить "на дым". <a href="https://ru.wikipedia.org/wiki/Smoke_test">История термина:</a> Первое свое применение этот термин получил у печников, которые, собрав печь, закрывали все заглушки, затапливали ее и смотрели, чтобы дым шел только из положенных мест.
Повторное «рождение» термина произошло в радиоэлектронике. Первое включение нового радиоэлектронного устройства, пришедшего из производства, совершается на очень короткое время (меньше секунды). Затем инженер руками ощупывает все микросхемы на предмет перегрева. Сильно нагревшаяся за эту секунду микросхема может свидетельствовать о грубой ошибке в схеме. Если первое включение не выявило перегрева, то прибор включается снова на большее время. Проверка повторяется. И так далее несколько раз. Выражение «smoke-test» используется инженерами в шуточном смысле, так как появления дыма, а значит и порчи частей устройства, стараются избежать.

Доп. материал:
<a href="https://testing-companies.com/qa-outsourcing-smoke-testing-critical-path-testing-extended-testing/">QA Outsourcing: Smoke Testing, Critical Path Testing, Extended Testing</a>
<h2>Что такое тестирование встряхиванием? (Shake out testing)</h2>
Стандартного определения ISO для теста на встряхивание для ПО не существует. Говорят, что это синоним к Smoke тестированию.
<h2>Что подразумевается под санитарным тестированием? (Sanity testing)</h2>
Для начала стоит сказать, что санитарным оно в русскоязычной среде назвалось по совершенно непонятным причинам, но гуглится только так. На самом же деле корректно говорить тестирование на вменяемость или разумность.
Санитарное тестирование - это узконаправленное тестирование достаточное для доказательства того, что конкретная функция работает согласно заявленным в спецификации требованиям. Является подмножеством регрессионного тестирования. Используется для определения работоспособности определенной части приложения после изменений, произведенных в ней или окружающей среде. Обычно выполняется вручную.

Доп. материалы:
<a href="https://www.merriam-webster.com/dictionary/sanity">Definition of sanity</a>
<a href="http://tryqa.com/what-is-sanity-testing/">What is Sanity testing? Advantages, disadvantages & differences</a>
<h2>Отличие санитарного тестирования от дымового? (Sanity vs Smoke testing)</h2>
Эти виды тестирования имеют "вектора движения", направления в разные стороны. В отличии от дымового (Smoke testing), санитарное тестирование (Sanity testing) направлено вглубь проверяемой функции, в то время как дымовое направлено вширь, для покрытия тестами как можно большего функционала в кратчайшие сроки.

Доп. материал:
<a href="https://habr.com/ru/post/358142/">В чем разница Smoke, Sanity, Regression, Re-test и как их различать?</a>
<h2>Что вы знаете про регрессионное тестирование? (Regression testing)</h2>
При корректировках программы необходимо гарантировать сохранение качества. Для этого используется регрессионное тестирование - дорогостоящая, но необходимая деятельность в рамках этапа сопровождения, направленная на перепроверку корректности измененной программы. В соответствии со стандартным определением, регрессионное тестирование - это выборочное тестирование, позволяющее убедиться, что изменения не вызвали нежелательных побочных эффектов, или что измененная система по-прежнему соответствует требованиям.
Главной задачей этапа сопровождения является реализация систематического процесса обработки изменений в коде. После каждой модификации программы необходимо удостовериться, что на функциональность программы не оказал влияния модифицированный код. Если такое влияние обнаружено, говорят о регрессионном дефекте. Для регрессионного тестирования функциональных возможностей, изменение которых не планировалось, используются ранее разработанные тесты. Одна из целей регрессионного тестирования состоит в том, чтобы, в соответствии с используемым критерием покрытия кода (например, критерием покрытия потока операторов или потока данных), гарантировать тот же уровень покрытия, что и при полном повторном тестировании программы. Для этого необходимо запускать тесты, относящиеся к измененным областям кода или функциональным возможностям.
Другая цель регрессионного тестирования состоит в том, чтобы удостовериться, что программа функционирует в соответствии со своей спецификацией, и что изменения не привели к внесению новых ошибок в ранее протестированный код. Эта цель всегда может быть достигнута повторным выполнением всех тестов регрессионного набора, но более перспективно отсеивать тесты, на которых выходные данные модифицированной и старой программы не могут различаться. Важной задачей регрессионного тестирования является также уменьшение стоимости и сокращение времени выполнения тестов.
Можно заключить, что регрессионное тестирование выполняется чтобы минимизировать регрессионные риски. То есть, риски того, что при очередном изменении продукт перестанет выполнять свои функции. С регрессионным тестированием плотно связана другая активность - импакт анализ (или иначе, анализ влияния изменений). Обычно под импакт анализом имеют в виду одно из следующих:
<ol>
<li>Попытку оценить регрессионные риски еще на этапе планирования изменений (этим определением, по моему опыту, чаще пользуются менеджеры и разработчики);
</li>
<li>Попытку определить объем регрессионного тестирования с учетом изменений, которые уже произошли (это определение чаще используют сами тестировщики). У Пола Джеррарда есть серия статей, где более детально раскрывается понятие импакт анализа, причем не только с позиции тестировщика.
Очевидно, что от эффективности импакт анализа зависит эффективность регрессионного тестирования. Но не всегда тщательно проведенный импакт анализ позволяет сократить затраты на последующее тестирование.
</li>
</ol>
Обоснование корректности метода отбора тестов. Перечислим некоторые особенности реализации регрессионного тестирования:
<ul>
<li>Некоторые участки кода программы не получают управление при выполнении некоторых тестов.
</li>
<li>Если участок кода реализует требование, но измененный фрагмент кода не получает управления при выполнении теста, то он и не может воздействовать на значения выходных данных программы при выполнении данного теста.
</li>
<li>Даже если участок кода, реализующий требование, получает управление при выполнении теста, это далеко не всегда отражается на выходных данных программы при выполнении данного теста. Действительно, если изменяется первый блок программы, например, путем добавления инициализации переменной, все пути в программе также изменяются, и, как следствие, требуют повторного тестирования. Однако может так случиться, что только на небольшом подмножестве путей действительно используется эта инициализированная переменная.
</li>
<li>Не каждый тест, проверяющий код, находящийся на одном пути с измененным кодом, обязательно покрывает этот измененный код.
</li>
<li>Код, находящийся на одном пути с измененным кодом, может не воздействовать на значения выходных данных измененных модулей программы.
</li>
<li>Не всегда каждый оператор программы воздействует на каждый элемент ее выходных данных.
</li>
</ul>
Предположим, что изменения в программе ограничиваются одним оператором. Если при выполнении какого-либо теста на исходной программе этот оператор никогда не получает управление, можно с уверенностью сказать, что он не получит управление и в ходе выполнения теста на новой программе, а результаты тестирования новой и старой программ будут совпадать. Следовательно, нет необходимости выполнять этот тест на новой программе. Указанный метод легко можно обобщить для случая нескольких изменений: если тест не задействует ни одного измененного оператора, и его входные данные не изменились, код, выполняемый им в измененной программе, будет в точности таким же, как в первоначальной версии. Такой тест не выявляет различий между двумя версиями системы; следовательно, нет необходимости прогонять его повторно. Если тест не затрагивает ни одного оператора вывода, поведение которого зависит от измененных операторов, это означает, что, несмотря на изменения в программе, все операторы, которые получают управление при выполнении этого теста, не изменят вывод системы по отношению к предыдущей версии. Таким образом, нет необходимости повторно прогонять и тесты такого рода.
Следовательно, необходимо ориентироваться на выбор только тех тестов, которые покрывают измененный код, воздействующий, в свою очередь, на вывод программы. Такой подход гарантирует, что будут выбраны только тесты, обнаруживающие изменения, и метод будет, как говорят, точным.
Классификация тестов при отборе.
Создание наборов регрессионных тестов рекомендуется начинать с множества исходных тестов. При заданном критерии регрессионного тестирования все исходные тесты подразделяются на четыре подмножества:
<ul>
<li>Множество тестов, пригодных для повторного использования. Это тесты, которые уже запускались и пригодны к использованию, но затрагивают только покрываемые элементы программы, не претерпевшие изменений. При повторном выполнении выходные данные таких тестов совпадут с выходными данными, полученными на исходной программе. Следовательно, такие тесты не требуют перезапуска.
</li>
<li>Множество тестов, требующих повторного запуска. К ним относятся тесты, которые уже запускались, но требуют перезапуска, поскольку затрагивают, по крайней мере, один измененный покрываемый элемент, подлежащий повторному тестированию. При повторном выполнении такие тесты могут давать результат, отличный от результата, показанного на исходной программе. Множество тестов, требующих повторного запуска, обеспечивает хорошее покрытие структурных элементов даже при наличии новых функциональных возможностей.
</li>
<li>Множество устаревших тестов. Это тесты, более не применимые к измененной программе и непригодные для дальнейшего тестирования, поскольку они затрагивают только покрываемые элементы, которые были удалены при изменении программы. Их можно удалить из набора регрессионных тестов.
</li>
<li>Новые тесты, которые еще не запускались и могут быть использованы для тестирования.
</li>
</ul>
Сразу после создания тест вводится в структуру базы данных как новый. После исполнения новый тест переходит в категорию тестов, пригодных для повторного использования либо устаревших. Если выполнение теста способствовало увеличению текущей степени покрытия кода, тест помечается как пригодный для повторного использования. В противном случае он помечается как устаревший и отбрасывается. Существующие тесты, повторно запущенные после внесения изменения в код, также классифицируются заново как пригодные для повторного использования или устаревшие в зависимости от тестовых траекторий и используемого критерия тестирования.
<img src="https://lh6.googleusercontent.com/nqirFfSu2IyEeva_AnCfbr2UeS0JlOarIep7zkQJB2U2jtFiill8K5miqrYj1IJy9IfN5KmkDwQ5yD7X92-8KyWQc_fZelMfjA8rGAY7VJ9JP4osmPLogehSOq79k5KVwJISwut0">
Классификация тестов по отношению к изменениям в коде требует анализа последствий изменений. Тесты, активирующие код, затронутый изменениями, могут требовать повторного запуска или оказаться устаревшими. Чтобы тест был включен в класс тестов, требующих повторного запуска, он должен быть затронут изменениями в коде, а также должен способствовать увеличению степени покрытия измененного кода по используемому критерию. Затронутым элементом теста может быть траектория, выходные значения, или и то, и другое. Чтобы тест был включен в класс тестов, пригодных для повторного использования, он должен вносить вклад в увеличение степени покрытия кода и не требовать повторного запуска.
Степень покрытия кода определяется для тестов, пригодных для повторного использования, поскольку к этому классу относятся тесты, не требующие повторного запуска и способствующие увеличению степени покрытия до желаемой величины. Если имеется компонент программы, не задействованный пригодными для повторного использования тестами, то вместо них выбираются и выполняются с целью увеличения степени покрытия тесты, требующие повторного запуска. После запуска такой тест становится пригодным для повторного использования или устаревшим. Если тестов, требующих повторного запуска, больше не осталось, а необходимая степень покрытия кода еще не достигнута, порождаются дополнительные тесты и тестирование повторяется.
Окончательный набор тестов собирается из тестов, пригодных для повторного использования, тестов, требующих повторного запуска, и новых тестов. Наконец, устаревшие и избыточные тесты удаляются из набора тестов, поскольку избыточные тесты не проверяют новые функциональные возможности и не увеличивают покрытие.

Дополнительный материал.
<ul>
<li><a href="https://www.intuit.ru/studies/courses/48/48/lecture/1446?page=1">Регрессионное тестирование: разновидности метода отбора тестов</a>
</li>
<li><a href="https://www.intuit.ru/studies/courses/48/48/lecture/1448">Регрессионное тестирование: методики, не связанные с отбором тестов и методики порождения тестов</a>
</li>
<li><a href="https://www.intuit.ru/studies/courses/48/48/lecture/1450">Регрессионное тестирование: алгоритм и программная система поддержки</a>
</li>
</ul>
<h2>Типы регрессии по Канеру?</h2>
Сэм Канер описал 3 основных типа регрессионного тестирования:
<ul>
<li>Регрессия багов (Bug regression) — попытка доказать, что исправленная ошибка на самом деле не исправлена
</li>
<li>Регрессия старых багов (Old bugs regression) — попытка доказать, что недавнее изменение кода или данных сломало исправление старых ошибок, т.е. старые баги стали снова воспроизводиться.
</li>
<li>Регрессия побочного эффекта (Side effect regression) — попытка доказать, что недавнее изменение кода или данных сломало другие части разрабатываемого приложения
</li>
</ul>

<h2>Объясните, что такое тестирование N+1?</h2>
Вариант регрессионного тестирования представлен как N+1. В этом методе тестирование выполняется в несколько циклов, в которых ошибки, обнаруженные в тестовом цикле «N», устраняются и повторно тестируются в тестовом цикле N + 1. Цикл повторяется, пока не будет найдено ни одной ошибки.
<h2>Что означает подтверждающее тестирование? (confirmation/re-testing)</h2>
Повторное тестирование - это тип тестирования, выполняемый для проверки того, что конкретный дефект устранен после исправления кода.
<h2>В чем разница между повторным и регрессионным тестированием?</h2>
<ul>
<li>Регрессионное тестирование проводится для подтверждения того, что недавнее изменение программы или кода не оказало неблагоприятного воздействия на существующие функции. Повторное тестирование проводится для подтверждения того, что тест-кейсы, которые не прошли, проходят после устранения дефектов. 
</li>
<li>Цель регрессионного тестирования подтвердить, что новые изменения кода не должны иметь побочных эффектов для существующих функций. Повторное тестирование проводится на основе исправлений дефектов. 
</li>
<li>Проверка дефектов не является частью регрессионного тестирования. Проверка дефекта является частью повторного тестирования 
</li>
<li>В зависимости от проекта и наличия ресурсов, регрессионное тестирование может проводиться параллельно с повторным тестированием. Приоритет повторного тестирования выше, чем регрессионное тестирование, поэтому оно проводится перед регрессионным тестированием. 
</li>
<li>Вы можете сделать автоматизацию для регрессионного тестирования, ручное тестирование может быть дорогим и трудоемким. 
</li>
<li>Регрессионное тестирование называется общим (generic) тестированием. Повторное тестирование - это плановое (planned) тестирование.
</li>
<li>Регрессионное тестирование проводится для пройденных Test case. Повторное тестирование проводится только для неудачных тестов. 
</li>
<li>Регрессионное тестирование проверяет наличие неожиданных побочных эффектов. Повторное тестирование гарантирует, что первоначальная ошибка была исправлена.
</li>
<li>Регрессионное тестирование проводится только тогда, когда есть какие-либо изменения или изменения становятся обязательными в существующем проекте. Повторное тестирование выполняет дефект с теми же данными и той же средой с разными входными данными с новой сборкой (build). 
</li>
<li>Test case для регрессионного тестирования могут быть получены из функциональной спецификации, user tutorials and manuals, а также defect reports в отношении исправленных проблем. Test case для повторного тестирования не могут быть получены до начала тестирования.
</li>
</ul>

<h2>Что вы знаете о тестировании сборки? (Build Verification Test)</h2>
Тестирование, направленное на определение соответствия, выпущенной версии, критериям качества для начала тестирования. По своим целям является аналогом Дымового Тестирования, направленного на приемку новой версии в дальнейшее тестирование или эксплуатацию. Вглубь оно может проникать дальше, в зависимости от требований к качеству выпущенной версии.
<h2>Что такое тестирование потоков? (Thread testing) </h2>
Тестирование потоков определяется как тип тестирования программного обеспечения, который проверяет основные функциональные возможности конкретной задачи (потока). Обычно проводится на ранней стадии фазы интеграционного тестирования. Тестирование на основе потоков является одной из дополнительных стратегий, принятых в ходе тестирования системной интеграции. Поэтому его, вероятно, следует более правильно назвать «тестом взаимодействия потоков» (thread interaction test).
Тестирование на основе потоков подразделяется на две категории:
<ul>
<li>Однопоточное тестирование включает одну транзакцию приложения за раз 
</li>
<li>Многопоточное тестирование включает одновременно несколько активных транзакций
</li>
</ul>
Как производить:
<ul>
<li>Тестирование на основе потоков является обобщенной формой тестирования на основе сеансов (session-based testing), в котором сеансы являются формой потока, но поток не обязательно является сеансом. 
</li>
<li>Для тестирования потока, поток или программа (небольшая функциональность) интегрируются и тестируются постепенно как подсистема, а затем выполняются для всей системы. 
</li>
<li>На самом низком уровне оно предоставляет интеграторам лучшее представление о том, что тестировать. 
</li>
<li>Вместо непосредственного тестирования программных компонентов требуется, чтобы интеграторы сосредоточились на тестировании логических путей выполнения в контексте всей системы.
</li>
</ul>
<h2>Что такое тестирование документации? (Documentation testing)</h2>
Плохая документация может повлиять на качество продукта. Хорошая документация по продукту играет решающую роль в конечном продукте. Тестирование артефактов, разработанных до, во время и после тестирования продукта, называется тестированием документации. Это нефункциональный тип тестирования программного обеспечения. Мы знаем, что дефекты, обнаруженные на этапе тестирования, более дорогостоящие, чем если бы они были обнаружены на этапе требований. Стоимость исправления ошибки увеличивается тем больше, чем позже вы найдете ее. Таким образом, тестирование документации может начаться с самого начала процесса разработки программного обеспечения, чтобы сэкономить большую сумму денег. Некоторые часто проверяемые артефакты:
<ul>
<li>Requirement documents
</li>
<li>Test Plan
</li>
<li>Test case
</li>
<li>Traceability Matrix (RTM)
</li>
</ul>
<h2>Какие вы знаете уровни тестирования данных?</h2>
Тесты группируются в зависимости от того, где они добавлены в SDLC, или от уровня детализации, который они содержат. В целом, существует четыре уровня или слоя тестирования: модульное тестирование, интеграционное тестирование, системное тестирование и приемочное тестирование. Целью уровней тестирования является систематизация тестирования программного обеспечения и простота выявления всех возможных Test case на определенном уровне. 
Здесь работает хорошая аналогия с пирамидой тестирования. Это распределение по количеству тестов на разных уровнях приложения.
<ul>
<li>Unit-слой — это когда тестируется один модуль программы, чаще всего это одна функция или метод. Таких тестов должно быть больше всего. Unit-тест для данных — это когда мы определяем требования для каждой ячейки. Нет смысла тестировать дальше, если у нас есть ошибки на уровне ячеек. Если, например, в фамилии содержатся цифры, то какой смысл проверять что-то дальше? Возможно, там должны быть буквы, похожие на эти цифры. И тогда нам нужно все исправлять и проверять следующий уровень, чтобы у нас все было в единственном числе и не было дубликатов, если так сказано в требованиях.
</li>
<li>Integration-слой — это когда несколько кусков программы тестируются вместе. Слой API для данных — это когда мы говорим о всей таблице. Допустим, у нас могут быть дубликаты, но не больше ста штук. Если у нас город-миллионник, то на одной улице не может жить миллион человек. Поэтому если мы сделаем выборку по улице, то количество адресов должно быть десять тысяч или тысяча — это надо определить. А если у нас миллион, то с данными что-то не так.
</li>
<li>System-слой — это когда вся программа тестируется полностью. В случае с данными этот слой означает, что тестируется вся система. Здесь включается статистика. Например, мы говорим, что у нас не может быть больше 30% мужчин, рожденных после 1985 года. Или мы говорим, что 80% данных должны быть одного типа.
</li>
<li>Приемочное тестирование - это тест, проводимый для определения того, удовлетворяются ли требования спецификации или контракта в соответствии с его поставкой. Приемочное тестирование в основном выполняется пользователем или заказчиком. Тем не менее, другие акционеры могут быть вовлечены в этот процесс.
</li>
</ul>
<h2>Что такое подкожный тест? (Subcutaneous test)</h2>
Тест, который выполняется не для конечного пользовательского интерфейса, а для интерфейса, расположенного чуть ниже поверхности (пример - API).


Доп. материал:
<a href="https://martinfowler.com/bliki/SubcutaneousTest.html">Subcutaneous Test</a>
<h2>Расскажите о локализации, глобализации и интернационализации? (Localization/ globalization/internationalization testing)</h2>
Глобализированное ПО - это ПО, функционирующее одинаково независимо от географической, культурной и национальной среды. Тестирование глобализации концентрируется на выявлении потенциальных проблем в дизайне продукта, которые могут испортить глобализацию. Например, разработчик должен заложить в CSS основу для вертикального текста, если в будущем планируется локализовать продукт на язык с вертикальным письмом или обработку почтовых индексов для разных стран (где-то цифры, где-то цифры с буквами и т.п.). Оно гарантирует, что код может обрабатывать желаемую международную поддержку без нарушения какой-либо функциональности. А также, что не будет никакой потери данных и проблем с отображением. 

Тестирование глобализации, в свою очередь, можно разделить на два подвида:
<ul>
<li>Тестирование интернационализации (118N);
</li>
<li>Тестирование локализации (L10N);
</li>
</ul>

(Цифра означает количество пропущенных букв, типа как k8s - kubernetes)

Интернализация ПО – это особый процесс, при котором веб-софт создается таким образом, чтобы оно было равноудаленным от какой-либо культуры и (или) специфики определенного географического региона.
Например, одна из задач по интернационализации ПО– корректное редактирование логики всех подключенных параметров форматирования (формат даты, времени, цифровое и валютное форматирование).
Также, тестировщики во время проверки на соответствие ПО требованиям 118N тестируют работу продукта на равномерность работы в разных регионах и культурах мира.
Основной задачей тестирования интернациональности является проверка того, может ли программный код работать со всей международной поддержкой без нарушения функциональности, что может привести к потере данных или проблемам целостности информации.
В основном, фокус тестирования интернациональности направлен на:
<ul>
<li>Тестирование языковой совместимости. Проводятся проверки того, может ли веб-продукт корректно работать в определенной языковой среде;
</li>
<li>Проверка функциональности: полное выполнение регрессионных тестов в разнообразных языковых средах (корректное отображение специфической информации – даты, времени и валюты);
</li>
<li>Тестирование на корректность отображения графического интерфейса;
</li>
<li>Проверка удобства пользования: тестирование простоты использования ПО на различных операционных системах, разнообразных устройствах и прочее.
</li>
</ul>

Локализация ПО – деятельность по модификации ПО в соответствии с определенными региональными настройками (языком, географической территорией, кодировкой и прочим), которая должна бесперебойно работать.
В данный вид проверки входит необходимость выполнения работ по переводу всего контента программного обеспечения для конечного пользователя. Во время перевода должны учитываться иконки, информационная графика, справочные материалы, техническая документация и иные культурные особенности регионов, где в будущем будет доступно это программное обеспечение.

На что обратить внимание:
<ul>
<li>Длина переведенных слов
</li>
<li>Параметры шрифта пользовательского интерфейса
</li>
<li>Ввод текста в разных локализациях
</li>
<li>RTL-языки (справа-налево) или вертикальных
</li>
<li>Перевод сокращений или аббревиатур
</li>
<li>Мета-теги (проблемы с SEO или отображением имени вкладки (title, description, keywords))
</li>
<li>Соответствие мер исчисления, валюты, postal code и т.п.
</li>
</ul>

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/company/alconost/blog/521330/">Локализационное тестирование: зачем оно нужно приложению или сайту?</a>
</li>
<li><a href="https://habr.com/ru/company/otus/blog/523112/">Почему интернационализация и локализация имеют значение</a>
</li>
<li><a href="https://habr.com/ru/post/532836/">Гайд по тестированию локализации и интернационализации, а также большой и полезный checklist</a>
</li>
<li><a href="https://lokalise.com/">Accelerate localization from code to delivery</a>
</li>
</ul>
<h2>Что такое исследовательское тестирование? (Exploratory testing)</h2>
Исследовательское Тестирование — одновременно является и техникой, и видом тестирования. Такое тестирование подразумевает под собой одновременно изучение проекта, функционала, проектирование тест кейсов в уме и тут же их исполнение, не записывая и не создавая тестовую документацию.
Такой вид тестирования обычно не предусматривается в тест плане и тест кейсы выполняются и модифицируются динамически. Эффективность такого тестирования напрямую зависит от опыта тестировщика ранее имевшим дело с этим приложением, платформой, знанием мест скопления возможных багов и рисками которые относятся к конкретному продукту.
Цель данного тестирования — это углубление в познании продукта, приложения и нахождения «на лету» возможных багов. Также такое тестирование помогает в дальнейшем проектировании тест кейсов для покрытия функционала данного приложения. Исследовательское тестирование широко используется в Agile-моделях.
 <img src="https://lh4.googleusercontent.com/YPaEupYJfq4gLD7JmQK6QxjN1efOTzdbyjHMi5sKMNKQPrM_ViRnvydi1uYQjpTb4_rEHrOuq-98Y8juAwGsSq3Wz0q0A6xwqOliBYWgodNQdtPcG0_9NMEeRJ4S_WYHDRj1Acr-">
Доп. материал:
<ul>
<li><a href="https://habr.com/ru/post/535094/">Исследовательское тестирование: пустая трата времени или мощный инструмент?</a>
</li>
<li><a href="https://www.satisfice.com/rapid-testing-methodology">Rapid Software Testing Methodology</a>
</li>
<li><a href="https://www.satisfice.com/exploratory-testing">Exploratory Testing</a>
</li>
<li><a href="http://www.testingeducation.org/BBST/exploratory/">Exploratory Testing</a>
</li>
<li><a href="http://www.testingeducation.org/BBST/exploratory/BBSTExploring.pdf">Exploratory Testing</a>
</li>
<li><a href="https://silo.tips/download/exploratory-testing-dynamics">Exploratory Testing Dynamics</a>
</li>
<li><a href="https://www.kaner.com/pdfs/QAIExploring.pdf">A Tutorial in Exploratory Testing</a>
</li>
<li><a href="https://medium.com/@cristina.mtys/tips-for-your-next-exploratory-testing-session-22b4421b9620">Plan your next exploratory testing session</a>
</li>
</ul>
<h2>Что вы знаете о турах Виттакера в исследовательском тестировании?</h2>
Чтобы систематизировать исследовательское тестирование можно использовать идею туров. Туры – это идеи и инструкции по исследованию программного продукта, объединенные определенной общей темой или целью. Туры, как правило, ограничены по времени – длительность тестовой сессии не должна превышать 4 часа. Идею туров развивали в своих работах Канер, Бах, Хендриксон, Болтон, Кохл и другие. Джеймс Виттакер (James A. Whittaker), хоть и не придумал саму идею туров, но предложил свой подход к исследовательскому тестированию с использованием туров и в своей книге "Exploratory Software Testing" в доступной форме озвучил идею туров и описал сами туры.
Тур – это своего рода план тестирования, он отражает основные цели и задачи, на которых будет сконцентрировано внимание тестировщика во время сессии исследовательского тестирования. При этом Виттакер использует метафору, что тестировщик – это турист, а тестируемое приложение – это город. Обычно у туриста (тестировщика) мало времени, поэтому он выполняет конкретную задачу в рамках выбранного тура, ни на что другое не отвлекаясь. Город (ПО) разбит на районы: деловой центр, исторический район, район развлечений, туристический район, район отелей, неблагополучный район.

Доп. материал:
<ul>
<li><a href="https://habr.com/ru/post/328990/">Туры в исследовательском тестировании. Личный перевод из книги Д. Виттакера «Исследовательское тестирование ПО»</a>
</li>
<li><a href="https://www.software-testing.ru/library/testing/testing-for-beginners/2965-exploratory-software-testing">Переводы туров для исследовательского тестирования</a>
</li>
<li><a href="https://www.software-testing.by/blog/exploratory-testing-exploratory-tours/">Исследовательское тестирование и исследовательские туры Виттакера</a>
</li>
</ul>
<h2>Что такое Свободное или Интуитивное тестирование? (Adhoc) </h2>
Часто его путают с другим видом тестирования «Exploratory testing» – «Исследовательское тестирование».
Свободное тестирование (ad-hoc testing) – это вид тестирования, который выполняется без подготовки к тестированию продукта, без определения ожидаемых результатов, проектирования тестовых сценариев. Это неформальное, импровизационное тестирование. Оно не требует никакой документации, планирования, процессов, которых следует придерживаться при выполнении тестирования. Такой способ тестирования в большинстве случаев дает большее количество заведенных отчетов об ошибке.  Это обусловлено тем, что тестировщик на первых шагах приступает к тестированию основной функциональной части продукта и выполняет как позитивные, так и негативные варианты возможных сценариев.
Чаще всего такое тестирование выполняется, когда владелец продукта не обладает конкретными целями, проектной документацией и ранее поставленными задачами. При этом тестировщик полагается на свое общее представление о продукте, сравнение с похожими продуктами, собственный опыт. Однако при тестировании ad-hoc имеет смысл владеть общей информацией о продукте, особенно если проект очень сложный и большой. Поэтому нужно хорошее представление о целях проекта, его назначении и основных функциях, и возможностях. А дальше уже можно приступать к ad-hoc тестированию.
Виды свободного тестирования (ad-hoc testing):
<ul>
<li>Buddy testing – процесс, когда 2 человека, как правило разработчик и тестировщик, работают параллельно и находят дефекты в одном и том же модуле тестируемого продукта. Такой вид тестирования помогает тестировщику выполнять необходимые проверки, а разработчику исправлять множество дефектов на ранних этапах.
</li>
<li>Pair testing – процесс, когда 2 тестировщика проверяют один модуль и помогают друг другу. К примеру, один может искать дефекты, а второй их документировать. Таким образом, у одного тестировщика будет функция, скажем так, обнаружителя, у другого – описателя.
</li>
<li>Monkey testing – произвольное тестирование продукта с целью как можно быстрее, используя различные вариации входных данных, нарушить работу программы или вызвать ее остановку (простыми словами – сломать).
</li>
</ul>

Различия между Buddy testing и Pair testing:
<ul>
<li>Buddy testing (Совместное тестирование) – это сочетание модульного тестирования и системного тестирования между разработчиком и тестировщиком.
</li>
<li>Pair testing (Парное тестирование) – выполняется только тестировщиками с разным уровнем знаний и опыта (такое сочетание поможет поделиться взглядами и идеями).
</li>
</ul>

Основные преимущества ad-hoc testing:
<ul>
<li>нет необходимости тратить время на подготовку документации;
</li>
<li>самые важные дефекты зачастую обнаруживаются на ранних этапах;
</li>
<li>часто применяется, когда берут нового сотрудника. С помощью этого метода, человек усваивает за 3 дня то, что, разбираясь тестовыми случаями, разбирал бы неделю – это называется форсированное обучение новых сотрудников;
</li>
<li>возможность найти трудновоспроизводимые и трудноуловимые дефекты, которые невозможно было бы найти, используя стандартные сценарии проверок.
</li>
</ul>

Если нам нужно провести ad-hoc тестирование интернет-магазина, то этот краткий список может помочь с тем, что нужно проверить:
<ul>
<li>все возможности сайта доступны без регистрации;
</li>
<li>корректность отображения анимаций и картинок;
</li>
<li>все возможности сайта доступны после регистрации;
</li>
<li>процесс регистрации;
</li>
<li>процесс добавления/удаления из корзины;
</li>
<li>процесс оплаты покупок;
</li>
<li>удобство в пользовании для новичков, простота, подсказки, помощь.
</li>
</ul>
<h2>Что вы знаете о мутационном тестировании? (Mutation testing)</h2>
Mutation testing - это тип тестирования программного обеспечения, в котором мы мутируем (меняем) определенные выражения в исходном коде и проверяем, способны ли Test case найти ошибки. Это тип тестирования белого ящика, который в основном используется для модульного тестирования. Изменения в мутантной программе сохраняются крайне небольшими, поэтому это не влияет на общую цель программы. Цель Mutation testing - оценить качество Test case, которые должны быть достаточно надежными, чтобы не выполнять мутантный код. Этот метод также называется стратегией тестирования на основе ошибок, так как он включает в себя создание ошибки в программе. 
<ul>
<li>Шаг 1: Ошибки вводятся в исходный код программы путем создания множества версий, называемых мутантами. Каждый мутант должен содержать одну ошибку, и цель состоит в том, чтобы заставить версию мутанта потерпеть неудачу, что демонстрирует эффективность Test case. 
</li>
<li>Шаг 2: Test case применяются к исходной программе, а также к программе мутанта. 
</li>
<li>Шаг 3: Сравните результаты оригинальной и мутантной программы. 
</li>
<li>Шаг 4: Если исходная программа и программы-мутанты генерируют разные выходные данные, то этот мутант уничтожается by the Test case. Следовательно, Test case достаточно хорош, чтобы обнаружить изменение между оригинальной и мутантной программой. 
</li>
<li>Шаг 5: Если исходная программа и программа-мутант генерируют одинаковые выходные данные, мутант остается в живых. В таких случаях необходимо создать более эффективные Test case, которые убивают всех мутантов.
</li>
</ul>
Что изменить в программе мутантов? Есть несколько методов, которые могут быть использованы для создания мутантных программ: 
<ul>
<li>Операторы замены операндов (Operand replacement operators) – например, в условии if (x> y) поменять местами значения x и y
</li>
<li>Операторы модификации выражений (Expression Modification Operators) – например, в условии if (х == у) Мы можем заменить == на >=
</li>
<li>Операторы модификации операторов (Statement modification Operators) – например, удалить часть else в конструкции if-else или удалить целиком конструкцию if-else, чтобы проверить, как ведет себя программа
</li>
</ul>
Оценка мутации = (убитые мутанты / общее количество мутантов) * 100

Автоматизированные инструменты для разных ЯП: mutmut, Humbug и Infection и т.п. 

Доп. материал:
<a href="https://habr.com/ru/post/334394/">Мутационное тестирование</a>
<h2>Что означает механизм тестирования по ключевым словам? (Keyword Driven testing Framework)</h2>
Это скриптовая техника, которая использует файлы данных, которые содержат ключевые слова, связанные с тестируемым ПО. Эти ключевые слова описывают набор действий, необходимых для выполнения определенного шага. Тест на основе ключевых слов состоит из ключевых слов высокого и низкого уровня, включая аргументы ключевых слов, которые составлены для описания действия Test case. Это также называется тестированием на основе таблиц (table-driven testing) или тестированием на основе action word (action word based testing). В тестировании по ключевым словам вы сначала идентифицируете набор ключевых слов, а затем связываете действие (или функцию), связанную с этими ключевыми словами. Здесь каждое действие тестирования, такое как открытие или закрытие браузера, щелчок мыши, нажатия клавиш и т. д., описывается ключевым словом, таким как openbrowser, click, Typtext и т. д.  Тестирование на основе ключевых слов обычно выполняется с помощью автоматического тестирования. 
<h2>Что вы знаете о тестировании интерфейса прикладного программирования (API - Application Programming Interface)? </h2>
Каждый день используя любимые мобильные приложения и веб-ресурсы вы незаметно взаимодействуете с API, скрытым под интерфейсом пользователя.
API действует как интерфейс между двумя программными приложениями и позволяет им связываться друг с другом на оговоренных правилах и не залезая в реализацию предоставляемых функций. Простой пример: вы можете встроить на свою главную страницу сайта маленький виджет прогноза погоды, который будет отправлять определенный правилами запрос к API некоего сервиса погоды и получать определенный правилами ответ, содержащий посылку с данными.
Еще более простой пример: примите официанта в качестве API ресторана. В ресторане вы даете заказ на основе блюд, определенных в меню. Официант принимает ваш заказ и на этом ваше участие заканчивается и вам не интересно, что там произойдет дальше. От официанта вы ожидаете только итог – вам приносят заказанное блюдо. 
Можете попробовать взаимодействие с API сами: отправляете GET запрос на <a href="https://reqres.in/api/users">https://reqres.in/api/users</a>, и получаете в ответ список пользователей. Это очень удобно, когда вы хотите предоставить интерфейс взаимодействия со своим сервисом сторонним лицам. Например, у google, instagram, vk и, в общем-то, всех популярных продуктов есть открытая часть API. То есть у вас есть документ с перечнем того, что и как можно спросить и что вам на это придет в ответ. Взаимодействовать с API можно и с веб-страницы, и с помощью специальных инструментов и напрямую из кода. Помимо этого, API еще чаще используется для внутренних нужд как архитектурное решение для связи между сервисами или вообще представлять собой не веб-взаимодействие, а решение внутри кода одного продукта (таким образом, гипотетически API может быть и у десктопного приложения и практически где угодно).
Тестирование API - это тип тестирования который включает в себя тестирование API напрямую, а также в рамках интеграционного тестирования, чтобы проверить, соответствует ли API ожиданиям с точки зрения функциональности, надежности, производительности и безопасности приложения. В тестировании API наш основной упор будет сделан на уровне бизнес-логики архитектуры программного обеспечения. 

<img src="https://lh6.googleusercontent.com/l1nV69iecqE78_9FkGox0wJnnRWBa5EYtH-brZxsAF-BYCzTucY09YCocUZnDTYCse-XcAIajcpS0oHanhJCKAIAy2n2MBMNTKNMFcjFjXoP6TPA2PIdS0-fbhu1EhNdZwkcQmp9">
Мнение:
"Тестирование API - не какой-то отдельный вид или тип тестирования, это просто еще один способ взаимодействия с системой. В случае с UI у вас есть, условно, страница набором полей, которые вы заполняете, отправляете и ждете реакции от системы. В случае с API у вас есть эндпоинт и набор параметров.  Посылаете запрос -> получаете ответ -> валидируете ответ. Часть из этих тестов будет негативными, часть перейдет в "контрактное" тестирование, часть уйдет в тестирование валидации. Вся остальная логика тестирования - про приоритеты, техники тест-дизайна и прочее остается неизменным. 

С чего начать. 
<ol>
<li>Почитать про инструменты, что это такое и как оно работает. 
</li>
<li>Потренироваться на любом открытом API посылать/получать/обрабатывать запросы любым удобным вам способом - хоть с помощью python (разобраться можно за 2-3 вечера неспешного изучения с нуля), хоть с помощью GUI инструментов, хоть с помощью CURL. 
</li>
<li>Получить список функциональности API:
</li>
<ol>
<li> - Кто является "клиентом" для этого АПИ (использует его ваше приложение/фронтенд или вы его отдаете во вне). 
</li>
<li>- Какие функции доступны через API. 
</li>
</ol>
<li>Для списка функциональности выше составить список функциональных тест-кейсов, начиная с того, что представляет большую бизнес значимость. 
</li>
<li>Для того же списка функциональности получить все нужные данные: 
</li>
<ol>
<li>- Эндпоинты (если они есть в вашем случае). 
</li>
<li>- Схему авторизации. 
</li>
<li>- Документацию (если есть) или описание работы. 
</li>
</ol>
<li>Дополнить список функциональных проверок из п.3 более подробными тестами про схему взаимодействия, авторизацию, тестирование контракта, валидацию значений и пр. 
</li>
<li>Начать писать запросы следуя списку тест-кейсов из п.3 и 4 с помощью инструмента, который выбрали в п.1"
</li>
</ol>
© @azshoo

Типы тестирования API:
<ul>
<li>Unit testing: Для проверки функциональности отдельной операции
</li>
<li>Functional testing: Чтобы проверить функциональность более широких сценариев с помощью блока результатов unit-тестирования, протестированных вместе
</li>
<li>Load testing: Чтобы проверить функциональность и производительность под нагрузкой
</li>
<li>Runtime/Error Detection: Мониторинг приложения для выявления проблем, таких как исключения и утечки ресурсов
</li>
<li>Security testing: Чтобы гарантировать, что реализация API защищена от внешних угроз 
</li>
<li>UI testing: Это выполняется как часть end-to-end integration тестов, чтобы убедиться, что каждый аспект пользовательского интерфейса функционирует должным образом. 
</li>
<li>Interoperability and WS Compliance testing: Совместимость и WS Compliance testing - это тип тестирования, который применяется к SOAP API. Функциональная совместимость между API-интерфейсами SOAP проверяется путем обеспечения соответствия профилям функциональной совместимости веб-служб. Соответствие WS- * проверено, чтобы гарантировать, что стандарты, такие как WS-Addressing, WS-Discovery, WS-Federation, WS-Policy, WS-Security и WS-Trust, должным образом реализованы и используются
</li>
<li>Penetration testing: Чтобы найти уязвимости при атаках злоумышленников
</li>
<li>Fuzz testing: Для проверки API путем принудительного ввода в систему некорректных данных для попытки принудительного сбоя
</li>
</ul>
Примеры для тестирования API: 
<ul>
<li>Возвращаемое значение на основе входных условий: его относительно легко проверить, поскольку входные данные могут быть определены и результаты могут быть проверены. 
</li>
<li>Ничего не возвращает: при отсутствии возвращаемого значения проверяется поведение API в системе. 
</li>
<li>Вызов другого API / события / прерывания: если выход API инициирует какое-либо событие или прерывание, то эти события и прерывания listeners следует отслеживать 
</li>
<li>Обновление структуры данных: Обновление структуры данных будет иметь определенный эффект или влияние на систему, и это должно быть проверено 
</li>
<li>Изменение определенных ресурсов: если вызов API изменяет некоторые ресурсы, его следует проверить путем доступа к соответствующим ресурсам.
</li>
</ul>
Доп. материал:
<ul>
<li><a href="https://www.youtube.com/watch?v=7D7AMmgxt_I&t=1540s&ab_channel=QASTARTUP-ITTrainingCenter">Курс Тестирование ПО. Занятие 29. Тестирование API | QA START UP</a>
</li>
<li><a href="https://dou.ua/lenta/columns/api-testing-stages/">От шока до принятия: пять стадий тестирования API</a>
</li>
<li><a href="https://software-testing.ru/library/testing/testing-automation/3382-api-testing">Тестирование API</a>
</li>
<li><a href="https://habr.com/ru/company/jugru/blog/525298/">Swagger/OpenAPI Specification как основа для ваших приемочных тестов</a>
</li>
<li><a href="https://habr.com/ru/company/nix/blog/534156/">История одного сервера и тестировщика Васи</a>
</li>
<li><a href="https://www.howtogeek.com/343877/what-is-an-api/">What Is an API?</a>
</li>
<li><a href="https://www.youtube.com/watch?v=kUPWQMalWNk&feature=youtu.be&ab_channel=ArtsiomRusauQALife">Тестирование API простыми словами за 8 минут / Тестировщик API</a>
</li>
</ul>
<h2>Как протестировать API без документации/черным ящиком?</h2>
Если Вам по какой-то причине предстоит проделать эту неблагодарную работу, определитесь, насколько все плохо и какая у Вас есть информация об объекте тестирования.

Известно ли какие порты для Вас открыты? Знаете ли Вы нужные endpoints?
Если дело совсем плохо - просканируйте порты, например, с помощью netcat. Открытые порты сохраните в файл.
Эта операция займет довольно много времени. Можете почитать советы по работе с Nmap и Netcat. 
Если Вам известен нужный порт и соответствующий endopoint - переберите все возможные HTTP методы. Начните с наиболее очевидных POST, PUT, GET. Для ускорения процесса напишите скрипт, например, на Python.

В худшем случае, когда ни порт ни endpoints неизвестны Вам, скорее всего придется перебирать все открытые порты и генерировать endpoints, которые подходят по смыслу.

Разработчики обычно не особо заморачиваются и закладывают минимально-необходимую информацию. Так что включите воображение и попробуйте придумать endpoints опираясь на бизнес логику и принятые в Вашей компании стандарты.

Если ни endpoints ни бизнес логика Вам неизвестны, то у меня есть подозрение, что Вы тестируете API с не самыми хорошими намерениями.

<h2>Тестирование клиентской части и серверной, в чем разница? (Frontend testing Vs. Backend testing?)</h2>
<img src="https://lh3.googleusercontent.com/pxJmlG2P53pOIW6wYUhc2eNaOkyhVok_Y_rnOBsMzIApYQqv0kho32UilY66FTRJISRr7TP-8w92l5xAqgWcWpA163OcpTL1uCm4mKRY1nD6JfZDjPKQw2fC-lbTwQLJKGg8m8fU">
Frontend testing - это тип тестирования, который проверяет уровень представления 3-уровневой архитектуры. С точки зрения непрофессионала, вы проверяете GUI - все, что видно на экране, на стороне клиента. Для веб-приложения интерфейсное тестирование будет включать проверку функциональных возможностей, таких как формы, графики, меню, отчеты и т. д., а также связанный Javascript. Frontend testing - это термин, охватывающий различные стратегии тестирования, включая оценку производительности фронтенда, которая является хорошей практикой перед тестированием приложения с высокими пользовательскими нагрузками. Тестировщик должен хорошо понимать бизнес-требования для выполнения этого типа тестирования. Ранее оптимизация производительности означала оптимизацию на стороне сервера. Это было связано с тем, что большинство веб-сайтов были в основном статичными, а большая часть обработки выполнялась на стороне сервера. Однако сегодня веб-приложения становятся более динамичными и в результате код на стороне клиента нередко становится причиной низкой производительности. 
Тестирование клиентской части невозможно в некоторых случаях: бэкенд разрабатывают быстрее, чем фронтенд; очевидно, если клиентская часть отсутствует в принципе ( самодостаточное приложение, терминальная команда).
Backend testing - это тип тестирования, который проверяет уровень приложений и базы данных 3-уровневой архитектуры. В сложном программном приложении, таком как ERP, внутреннее тестирование повлечет за собой проверку бизнес-логики на уровне приложений. Для более простых приложений бэкэнд-тестирование проверяет серверную часть или базу данных. Это означает, что данные, введенные в интерфейс, будут проверены в базе данных. Базы данных проверяются на наличие свойств ACID, операций CRUD, их схемы, соответствия бизнес-правилам. Базы данных также проверяются на безопасность и производительность. Производится проверка целостности данных, Проверка достоверности данных, Тестирование функций, процедур и триггеров. При внутреннем тестировании нет необходимости использовать графический интерфейс. Вы можете напрямую передавать данные с помощью браузера с параметрами, необходимыми для функции, чтобы получить ответ в некотором формате по умолчанию. Например, XML или JSON. Вы также подключаетесь к базе данных напрямую и проверяете данные с помощью SQL-запросов.

Доп. материал:<a href="https://habr.com/ru/company/funcorp/blog/518248/"> </a>
<ul>
<li><a href="https://habr.com/ru/post/510458/">Как найти границы на клиенте и сервере</a>
</li>
<li><a href="https://habr.com/ru/company/funcorp/blog/518248/">Как Иван ошибку в бэкенде локализовывал</a>
</li>
<li><a href="https://www.youtube.com/watch?v=XSeoWpSlcig&feature=youtu.be&ab_channel=PodlodkaPodcast">Круглый стол "Почему не стоит тестировать бэкенд руками"</a>
</li>
</ul>
<h2>Что подразумевают под эталонным тестированием? (Baseline testing)</h2>
Это подход к тестированию, в котором за точку отсчета берется базовая линия - это показатель конкретного ориентира, который служит основой для нового тестирования. В базовом тестировании тесты собирают и сохраняют все результаты, полученные в исходном коде, и сравнивают с эталонным базовым уровнем. Этот базовый уровень относится к последним принятым результатам испытаний. Если в исходном коде есть новые изменения, то для повторного выполнения тестов необходимо сформировать текущий базовый уровень. Если последние результаты будут приняты, то текущая базовая линия станет эталонной. По большей части Baseline testing относят к тестированию производительности.
<h2>В чем разница между Baseline и Benchmark testing?</h2>
<ul>
<li>Baseline предназначено для оценки производительности приложения. Benchmark сравнивает производительность приложения с отраслевым стандартом. 
</li>
<li>Baseline тестирование использует данные, собранные для повышения производительности. Benchmark возвращает информацию о целевом приложении по сравнению с другими приложениями.
</li>
<li>Baseline тестирование сравнивает текущую производительность с предыдущей производительностью приложения, тогда как Benchmark сравнивает производительность нашего приложения с производительностью конкурентов.
</li>
</ul>
<h2>Что такое параллельное/многопользовательское тестирование? (Concurrency/Multi-user testing)</h2>
Параллельное тестирование определяется как метод тестирования для обнаружения дефектов в приложении, когда в систему вошли несколько пользователей. Другими словами, отслеживание эффекта, когда несколько пользователей выполняют одно и то же действие одновременно. Параллельное тестирование также называется многопользовательским тестированием. Тестирование параллельной программы является более сложной задачей, чем тестирование последовательной программы, из-за недетерминированности и проблем синхронизации. Зачем оно нужно:
<ul>
<li>Определяет влияние одновременного доступа к одним и тем же записям базы данных, модулям или коду приложения. 
</li>
<li>Определяет и измеряет уровень взаимоблокировки, блокировки и использования однопоточного кода и ограничения доступа к общим ресурсам
</li>
</ul>
<h2>Как вы думаете, что такое тестирование на переносимость? </h2>
Тестирование переносимости — это тип тестирования программного обеспечения, который проводится для определения степени легкости или сложности, с которой программное приложение может быть эффективно и эффективно перенесено с одного аппаратного обеспечения, программного обеспечения или среды на другое.
Результаты тестирования переносимости представляют собой измерения того, насколько легко программный компонент или приложение будут интегрированы в среду, и затем эти результаты будут сравниваться с нефункциональным требованием переносимости программной системы. Измерение основано на сравнении стоимости адаптации программного обеспечения к новой среде и стоимости реконструкции.
Атрибуты тестирования переносимости:
<ul>
<li>Адаптивность: Адаптируемость определяется как способность программного приложения адаптироваться к конкретной среде без каких-либо усилий. Общие стандарты связи между несколькими системами помогают повысить адаптивность системы в целом.
</li>
<li>Installability: Устанавливаемость определяется как способность программного приложения быть установленным в желаемой среде без использования дополнительных ресурсов. Устанавливаемость выполняется на программном обеспечении, которое должно быть установлено в целевой среде.
</li>
<li>Заменяемость: Возможность замены определяется как способность программного приложения заменять другое программное обеспечение в конкретной среде. Приложение, которое заменяет предыдущее приложение, должно давать одинаковые результаты во всех целевых средах.
</li>
<li>Сосуществование: Сосуществование определяется как способность программного приложения работать с другим программным приложением в системе, не мешая друг другу и совместно используя один и тот же ресурс. Специально это тестирование используется в больших системах, которые включают в себя несколько подсистем.
</li>
</ul>
<h2>Что такое тестирование графического интерфейса/визуальное тестирование? (GUI - Graphical User Interface testing)</h2>
Существует два типа интерфейсов для компьютерного приложения. Интерфейс командной строки, где вы вводите текст, и компьютер отвечает на эту команду и GUI - графический интерфейс пользователя, где вы взаимодействуете с компьютером, используя графическое представление, а не текст. 
Цель тестирования графического интерфейса пользователя (GUI) - проверить функциональность интерфейса пользователя.
Примеры:
<ul>
<li>Тестирование размера, положения, ширины, высоты элементов. 
</li>
<li>Тестирование сообщений об ошибках, которые отображаются. 
</li>
<li>Тестирование разных разделов экрана. 
</li>
<li>Проверка шрифта, читаемый ли он или нет. 
</li>
<li>Тестирование экрана в разных разрешениях с помощью увеличения и уменьшения масштаба, например, 640 x 480, 600x800 и т. д. 
</li>
<li>Проверка выравнивания текстов и других элементов, таких как значки, кнопки и т. д. , находятся на своем месте или нет. 
</li>
<li>Тестирование цветов шрифтов. 
</li>
<li>Проверка цветов сообщений об ошибках, предупреждающих сообщений. 
</li>
<li>Проверка, имеет ли изображение хорошую четкость или нет. 
</li>
<li>Тестирование выравнивания изображений. 
</li>
<li>Проверка орфографии. 
</li>
<li>Пользователь не должен разочаровываться при использовании системного интерфейса. 
</li>
<li>Тестирование, является ли интерфейс привлекательным или нет. 
</li>
<li>Тестирование полос прокрутки в соответствии с размером страницы, если таковые имеются. 
</li>
<li>Тестирование отключенных полей, если таковые имеются. 
</li>
<li>Тестирование размера изображений. 
</li>
<li>Проверка заголовков, правильно ли они выровнены или нет. 
</li>
<li>Тестирование цвета гиперссылки.
</li>
</ul>

Визуальное тестирование проверяет корректность отображения пользователю web-сайта, мобильного или десктопного приложения, дизайн-системы, PDF-файла или отдельного изображения на наличие расхождений с спецификацией дизайна (рендеринг страниц, шрифтов, изображений и т. д.). Раньше выполнялось вручную, т.к., например, в случае веб-сайта классическое автоматизированное тестирование было бесполезно – большинство инструментов сверялись с DOM и не видели те ошибки, что человек мог увидеть вживую. Сейчас визуальное тестирование выполняется автоматизированными инструментами создания скриншотов и сверки их с эталоном. Там все еще очень много нюансов, но это уже не относится к статье о ручном тестировании.

Доп. материал:
<a href="https://habr.com/ru/company/oleg-bunin/blog/499638/">Эффективное тестирование верстки</a>
<h2>Что такое A/B тестирование?</h2>
A / B-тестирование также называется сплит-тестированием (split). При тестировании AB мы создаем и анализируем два варианта приложения, чтобы найти, какой вариант работает лучше с точки зрения пользовательского опыта, потенциальных клиентов, конверсий или любой другой цели, а затем в конечном итоге сохранить наиболее эффективный вариант. 
Давайте попробуем понять это на примере. Предположим, у нас есть интернет магазин и каталог отображается определенным образом. В какой-то момент (новые маркетинговые исследования/пожелания клиента и т. д.) решено изменить дизайн выдачи товаров в каталоге. Независимо от того, сколько проведено анализа, выпуск нового пользовательского интерфейса будет большим изменением и может иметь неприятные последствия. 
В этом случае мы можем использовать A / B-тестирование. Мы создадим интерфейс нового варианта и выпустим его для некоторого процента пользователей. Например - мы можем распределить пользователей в соотношении 50:50 или 80:20 между двумя вариантами - A и B. После этого в течение определенного периода времени мы будем наблюдать эффективность обоих вариантов. Таким образом, тестирование A/B помогает принять решение о выборе лучшего варианта.

Доп. материал:
<a href="https://habr.com/ru/company/skyeng/blog/518164/">Ошибки в дизайне A/B тестов, которые я думала, что никогда не совершу</a>
<h2>Что означает сквозное тестирование? (E2E - End–to–End)</h2>
Сквозное тестирование - это стратегия тестирования для выполнения тестов, которые охватывают все возможные потоки приложения от его начала до конца; проверяет программную систему вместе с ее интеграцией с внешними интерфейсами. Целью сквозного тестирования является создание полного производственного сценария, выявление программных зависимостей и утверждение, что между различными программными модулями и подсистемами передается правильный ввод. Сквозное тестирование обычно выполняется после функционального и системного тестирования. Оно использует реальные данные, такие как данные и тестовая среда, для имитации настроек в реальном времени. Сквозное тестирование также называется цепным тестированием (Chain testing).
Для чего оно нужно? Современные программные системы являются сложными и взаимосвязаны с несколькими подсистемами. Подсистема может отличаться от текущей системы или может принадлежать другой организации. Если какая-либо из подсистем выйдет из строя, вся система программного обеспечения может рухнуть. Это серьезный риск, и его можно избежать путем сквозного тестирования. 
<h2>В чем разница между E2E и системным тестированием?</h2>

<table>
<tr>
<td>End to End testing
</td><td>System testing
</td></tr>
<tr>
<td>Проверяет программную систему, а также взаимосвязанные подсистемы
</td><td>Проверяет только программную систему в соответствии со спецификациями требований.
</td></tr>
<tr>
<td>Проверяет весь E2E flow
</td><td>Проверяет функциональные возможности и функции системы.
</td></tr>
<tr>
<td>Все интерфейсы, бэкэнд-системы 
</td><td>Функциональное и нефункциональное тестирование 
</td></tr>
<tr>
<td>Выполняется после завершения System testing
</td><td>Выполняется после завершения Integration testing
</td></tr>
<tr>
<td>Сквозное тестирование включает проверку внешних интерфейсов, которые могут быть сложными для автоматизации. Следовательно, ручное тестирование является предпочтительным.
</td><td>Как ручное, так и автоматическое могут быть выполнены для тестирования системы
</td></tr>
</table>

<h2>Что такое параллельное тестирование? (Parallel testing)</h2>
Это тип тестирования ПО, который одновременно проверяет несколько приложений или подкомпонентов одного приложения, чтобы сократить время выполнения теста. При параллельном тестировании тестировщик запускает две разные версии программного обеспечения одновременно с одним и тем же вводом. Цель состоит в том, чтобы выяснить, ведут ли себя прежняя система и новая система одинаково или по-разному. Это гарантирует, что новая система достаточно способна для эффективной работы программного обеспечения.

 <img src="https://lh4.googleusercontent.com/nbGIawh-G-P2Ti_z4JFNHAeNjZe4akr_3d72SCmwiSiyMaGgj2AieL2r6spV4LQ2T2RGeHApth9s8PCqCYN1gOhICv7KylLgP2zVlwnm5m5xZLrOb2xLpxyd1hdWPHUxbpg71ihD">
Пример: когда какая-либо организация переходит от старой системы к новой, legacy является важной частью. Передача этих данных является сложным процессом. При тестировании программного обеспечения проверка совместимости вновь разработанной системы со старой системой осуществляется посредством «параллельного тестирования».
<table>
<tr>
<td>Это Parallel testing
</td><td>Это НЕ Parallel testing
</td></tr>
<tr>
<td><ul>
<li>Тестирование обновленного приложения по сравнению с предыдущим приложением. 
</li>
<li>Запуск старого сценария с новым программным обеспечением с зарезервированными условиями ввода. 
</li>
<li>Цель состоит в том, чтобы узнать, соответствует ли результат предыдущей системе. 
</li>
<li>Должен иметь знания о старой и недавно разработанной системе
</li>
</ul>
</td><td><ul>
<li>Тестирование только одного ПО 
</li>
<li>Кросс-браузерное или кроссплатформенное тестирование. 
</li>
<li>Цель состоит в том, чтобы выяснить проблему проектирования. 
</li>
<li>Знать разницу не обязательно.
</li>
</ul>
</td></tr>
</table>
<h1>----- Тест дизайн -----</h1>
<h2>Тест дизайн? (Test Design)</h2>
Этап процесса тестирования ПО, на котором проектируются и создаются Test case (тест кейсы), в соответствии с определенными ранее критериями качества и целями тестирования. План работы над тест дизайном:
<ul>
<li>анализ имеющихся проектных артефактов: документация (спецификации, требования, планы), модели, исполняемый код и т. д. 
</li>
<li>написание спецификации по тест дизайну (<a href="http://www.protesting.ru/documentation/sqe_test_design_specification_template.zip">Test Design Specification</a>)
</li>
<li>проектирование и создание <a href="http://www.protesting.ru/testing/testcase.html">Test case</a>
</li>
</ul>
Роли, ответственные за тест дизайн:
<ul>
<li>Тест аналитик - определяет "ЧТО тестировать?"
</li>
<li>Тест дизайнер - определяет "КАК тестировать?"
</li>
</ul>
Попросту говоря, задача тест аналитиков и дизайнеров сводится к тому, чтобы используя различные стратегии и техники тест дизайна, создать набор Test case, обеспечивающий оптимальное тестовое покрытие тестируемого приложения. Однако, на большинстве проектов эти роли не выделяется, а доверяется обычным тестировщикам, что не всегда положительно сказывается на качестве тестов, тестировании и, как из этого следует, на качестве ПО (конечного продукта).
<h2>Перечислите известные техники тест-дизайна?</h2>
<ul>
<li>Cтатические (Static):
</li>
<ul>
<li>Review:
</li>
<ul>
<li>Неформальное ревью (Informal review)
</li>
<li>Прохождение (Walkthrough)
</li>
<li>Техническое ревью (Technical Review)
</li>
<li>Инспекция (Inspection)
</li>
</ul>
<li>Статический анализ (Static Analysis):
</li>
<ul>
<li>Поток данных (Data Flow) 
</li>
<li>Поток управления (Control Flow)
</li>
<li>Путь (Path)
</li>
<li>Стандарты (Standards)
</li>
</ul>
</ul>
<li>Динамические (Dynamic):
</li>
<ul>
<li>Белый ящик (White-box)
</li>
<ul>
<li>Выражение (Statement)
</li>
<li>Решение (Decision)
</li>
<li>Ветвь (Branch)
</li>
<li>Условие (Condition)
</li>
<li>Конечный автомат (FSM)
</li>
</ul>
<li>Основанные на опыте (Experience-based):
</li>
<ul>
<li>Предугадывание ошибки (Error Guessing - EG)
</li>
<li>Исследовательское тестирование (Exploratory testing)
</li>
<li>Ad-hoc testing
</li>
</ul>
<li>Черный ящик (Black-box):
</li>
<ul>
<li>Эквивалентное Разделение (Equivalence Partitioning - EP)
</li>
<li>Анализ Граничных Значений (Boundary Value Analysis - BVA)
</li>
<li>Комбинаторные техники (<a href="https://sysgears.com/articles/test-design-techniques-overview/#combinatorial">Combinatorial Test Techniques</a>)
</li>
<li>Переходы между состояниями (State transition)
</li>
<li>Случаи использования (Use case testing)
</li>
</ul>
</ul>
</ul>

Альтернативный источник:
<ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#black-box">Specification-Based Testing Techniques (or Black Box techniques):</a>
</li>
<ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#equivalence-classes">Equivalence Partitioning</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#boundary-values">Boundary Value Analysis</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#combinatorial">Combinatorial Test Techniques:</a>
</li>
<ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#all-combinations">All Combinations</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#pairwise">Pairwise Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#each-choice">Each Choice Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#base-choice">Base Choice Testing</a>
</li>
</ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#decision-table">Decision Table Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#classification-tree">Classification Tree Method</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#state-transition">State Transition Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#cause-effect">Cause-Effect Graphing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#scenario">Scenario Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#random">Random Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#syntax">Syntax Testing</a>
</li>
</ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#white-box">Structure-Based Testing Techniques (or White Box techniques):</a>
</li>
<ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#statement">Statement Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#decision">Decision Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#conditions">Condition Testing:</a>
</li>
<ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#branch-condition">Branch Condition Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#branch-condition-combination">Branch Condition Combination Testing</a>
</li>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#mcdc">Modified Condition Decision Coverage (MCDC) Testing</a>
</li>
</ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#data-flow">Data Flow Testing</a>
</li>
</ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#experience">Experience-Based Testing Techniques:</a>
</li>
<ul>
<li><a href="https://sysgears.com/articles/test-design-techniques-overview/#error-guessing">Error Guessing</a>
</li>
</ul>
</ul>

Все методы тестирования на основе спецификаций (черного ящика) могут быть удобно описаны и систематизированы с помощью следующей таблицы:

<table>
<tr>
<td>Группа
</td><td>Техника
</td><td>Когда используется
</td></tr>
<tr>
<td>Элементарные методы: 
- сфокусированы на анализе входных / выходных параметров - могут быть объединены для обеспечения лучшего покрытия - обычно не используют и не зависят от других приемов
</td><td>Equivalence Partitioning
</td><td>Входные и выходные параметры имеют большое количество возможных значений
</td></tr>
<tr>
<td>Boundary Value Analysis
</td><td>Значения параметров имеют явные (например, четко определенные в документации) границы и диапазоны или неявные (например, известные технические ограничения) границы
</td></tr>
<tr>
<td>Комбинаторные стратегии: 
- объединить возможные значения нескольких входных / выходных параметров - можно использовать элементарные приемы, чтобы уменьшить количество возможных значений
</td><td>All Combinations
</td><td>Количество возможных комбинаций входов достаточно мало, или каждая отдельная комбинация входов приводит к определенному выходу
</td></tr>
<tr>
<td>Pairwise Testing
</td><td>Количество входных комбинаций чрезвычайно велико и должно быть сведено к приемлемому набору cases
</td></tr>
<tr>
<td>Each Choice Testing
</td><td>У вас есть функциональность, при которой конкретное значение параметра чаще вызывает ошибку чем комбинация значений
</td></tr>
<tr>
<td>Base Choice Testing
</td><td>Вы можете выделить набор значений параметров, которые имеют наибольшую вероятность использования
</td></tr>
<tr>
<td>Продвинутые техники: - помочь проанализировать Систему с точки зрения бизнес-логики, иерархических отношений, сценариев и т. д. - анализ основан на данных, организованных в виде таблиц, диаграмм и шаблонов - может полагаться на элементарные и комбинаторные методы для разработки Test case
</td><td>Decision Table Testing
</td><td>Существует набор комбинаций параметров и их выводов, описываемых бизнес-правилами или другими правилами.
</td></tr>
<tr>
<td>Classification Tree Method
</td><td>У вас есть иерархически структурированные данные, или данные могут быть представлены в виде иерархического дерева
</td></tr>
<tr>
<td>State Transition Testing
</td><td>В функциональности есть очевидные состояния, у которых переходы регулируются правилами (например, потоками)
</td></tr>
<tr>
<td>Cause-Effect Graphing
</td><td>Причины (входы) и следствия (выходы) связаны большим количеством сложных логических зависимостей
</td></tr>
<tr>
<td>Scenario Testing
</td><td>Есть четкие сценарии в функционале
</td></tr>
<tr>
<td>Другие
</td><td>Random Testing
</td><td>Вы должны подражать непредсказуемости реальных входных данных, или функциональность имеет несистематические дефекты
</td></tr>
<tr>
<td>Syntax Testing
</td><td>Функциональность имеет сложный синтаксический формат для ввода (например, коды, сложные имена электронной почты и т. д.)
</td></tr>
</table>

Методы тестирования на основе структуры (Structure-Based Testing Techniques): также известны как методика тестирования White Box, это означает, что мы знакомы с кодом, который собираемся тестировать. Чтобы понять эти методы, мы должны определить, что такое покрытие в контексте разработки теста. Вот хорошее определение из Книги ISTQB: Тестирование покрытия определенным образом измеряет количество тестов, выполненных набором тестов (полученных другим способом, например, с использованием методов, основанных на спецификациях). Везде, где мы можем посчитать вещи и сказать, была ли каждая из этих вещей проверена каким-либо тестом, мы можем измерить охват. Основная мера покрытия:

              Number of coverage items exercised
 Coverage = -------------------------------------- x 100%
                Total number of coverage items

где «coverage item» - это то, что мы смогли подсчитать и посмотреть, выполнил ли тест этот элемент или использовал его.
Для методов, основанных на спецификациях, это могут быть случаи использования, разделы эквивалентности, граничные значения, состояния из диаграммы перехода состояний, процент бизнес-правил из таблицы решений и т. д. Для методов, основанных на структуре, элементы покрытия представлены структурные элементы кода. В принципе, оценка покрытия означает, что мы должны решить, какие структурные элементы мы будем использовать (например, заявления или решения). Затем найдите общее количество этих элементов в коде. Введите дополнительные операторы (например, ведение журнала) рядом с каждым структурным элементом, чтобы выяснить, использовался ли этот элемент во время выполнения Test case. И, наконец, измерьте охват, выполнив тесты и используя формулу, упомянутую выше. Но, как правило, вы не должны думать обо всех этих шагах, потому что есть много автоматизированных инструментов для измерения покрытия. Методы структурного тестирования обычно подразумевают, что вы должны измерить покрытие для существующих наборов тестов (включая наборы черного ящика), а затем разработать дополнительные Test case белого ящика, основанные на элементах структурного кода, для достижения максимально возможного покрытия.

Доп. материал:
<ul>
<li><a href="https://egor-romanov.medium.com/%D1%82%D0%B5%D1%81%D1%82-%D0%B4%D0%B8%D0%B7%D0%B0%D0%B9%D0%BD-%D0%BC%D0%B5%D1%82%D0%BE%D0%B4%D0%BE%D0%BC-interface-model-state-7fa89c43934d">Тест дизайн методом Interface — Model — State</a>
</li>
<li><a href="http://kaner.com/pdfs/swparadigm.pdf">Paradigms Paradigms of Black Box Software Software Testing Testing</a>
</li>
<li><a href="http://www.testingeducation.org/BBST/testdesign/">Test Design: A Survey of Black Box Software Testing Techniques</a>
</li>
</ul>
<h2>Что такое статическое тестирование, когда оно начинается и что оно охватывает?</h2>
При статическом тестировании код не выполняется. Вы вручную проверяете код, документы требований и проектные документы на наличие ошибок. Отсюда и название «статичный». Основная цель этого тестирования - повысить качество программных продуктов путем выявления ошибок на ранних этапах цикла разработки. Это тестирование также называется Non-execution техникой или verification. Проверки могут также производиться автоматически (например, используя линтеры).
В статическом тестировании проверяются следующее: 
<ul>
<li>Unit Test cases
</li>
<li>Business Requirements Document (BRD)
</li>
<li>Use Cases
</li>
<li>System/Functional Requirements
</li>
<li>Prototype
</li>
<li>Prototype Specification Document
</li>
<li>DB Fields Dictionary Spreadsheet
</li>
<li>Test Data
</li>
<li>Traceability Matrix Document
</li>
<li>User Manual/Training Guides/Documentation
</li>
<li>Test Plan Strategy Document/Test cases
</li>
<li>Automation/Performance Test Scripts
</li>
</ul>
<h2>Что такое динамическое тестирование, когда оно начинается и что оно охватывает?</h2>
При динамическом тестировании выполняется код. Оно проверяет функциональное поведение ПО, использование памяти / процессора и общую производительность системы. Основная цель этого тестирования - подтвердить, что программный продукт работает в соответствии с требованиями бизнеса. Это тестирование также называется Execution technique или validation. Динамическое тестирование выполняется на всех уровнях тестирования, и это может быть либо тестирование черного, либо белого ящика.
Виды динамического тестирования: Модульное тестирование. Интеграционное тестирование: Системное тестирование. Кроме того, нефункциональное тестирование, такое как производительность, тестирование безопасности.
На примере: Предположим, мы тестируем страницу входа в систему, где у нас есть два поля с именем «Имя пользователя» и «Пароль», а имя пользователя ограничено буквенно-цифровым форматом. Когда пользователь вводит имя пользователя «VA610», система принимает это. Но когда пользователь вводит «VA610 @ 123», тогда приложение выдает сообщение об ошибке. Этот результат показывает, что код действует динамически на основе пользовательского ввода. 
<h2>Какие виды Review вы знаете?</h2>
<ul>
<li>Неофициальные reviews: это один из видов рецензирования, который не сопровождается каким-либо процессом поиска ошибок в документе. При использовании этого метода вы просто просматриваете документ и оставляете неофициальные комментарии к нему. 
</li>
<li>Технические reviews: команда, состоящая из ваших коллег, изучает технические характеристики программного продукта и проверяет, подходят ли он для проекта. Они пытаются найти любые несоответствия в спецификациях и стандартах. Этот обзор концентрируется главным образом на технической документации, связанной с программным обеспечением, такой как: Стратегия тестирования, План тестирования и спецификации требований. 
</li>
<li>Пошаговое руководство. Автор рабочего продукта объясняет продукт своей команде. Участники могут задавать вопросы, если таковые имеются. Встреча проводится автором. 
</li>
<li>Инспекция: Основная цель - найти дефекты, а встречу проводит обученный модератор. Этот обзор является формальным типом обзора, где следует строгий процесс поиска дефектов. У рецензентов есть контрольный список для проверки рабочих продуктов. Они фиксируют дефект и информируют участников об устранении этих ошибок. 
</li>
<li>Code Walk Through: Это неформальный анализ исходного кода программы для выявления дефектов и проверки методов кодирования.
</li>
</ul>
<h2>Что вы знаете о Data Flow testing?</h2>
Тестирование потока данных - это еще один набор методов / стратегий белого ящика, который связан с анализом потока управления, но с точки зрения жизненного цикла переменной. Переменные определяются, используются и уничтожаются, когда в них больше нет необходимости. Аномалии в этом процессе, такие как использование переменной без ее определения или после ее уничтожения, могут привести к ошибке. Существуют условные обозначения, которые могут помочь в описании последовательных во времени пар в жизненном цикле переменной: 
<ul>
<li>~ - переменная еще не существует или предыдущий этап был последним 
</li>
<li>d - определено, создано, инициализировано 
</li>
<li>k - не определено, убито 
</li>
<li>u - используется (c - использование вычислений; p - использование предикатов) 
</li>
</ul>
Таким образом, ~ d, du, kd, ud, uk, uu, k ~, u ~ являются вполне допустимыми комбинациями, когда ~ u, ~ k, dd, dk, kk, ku, d ~ являются аномалиями, потенциальными или явными ошибками. В настоящее время практически все они эффективно обнаруживаются компиляторами или, по крайней мере, IDE, и нам редко требуется выполнять статический анализ для обнаружения этих аномалий. То же самое относится и к динамическому анализу, который сфокусирован на исследовании / выполнении du пар - современные языки программирования снижают вероятность возникновения проблем, связанных с du. Так что в настоящее время такая проверка в основном не стоит усилий.
<h2>Что вы знаете о Control Flow testing?</h2>
Тестирование потоков управления (Control Flow Testing) - это одна из двух техник тестирования белого ящика, основанная на определении путей выполнения кода программного модуля и создания выполняемых тест кейсов для покрытия этих путей.
Фундаментом для тестирования потоков управления является построение графов потоков управления (Control Flow Graph), основными блоками которых являются:
<ul>
<li>блок процесса - одна точка входа и одна точка выхода
</li>
<li>точка альтернативы - одна точка входа, две и более точки выхода
</li>
<li>точка соединения - две и более точек входа, одна точка выхода
</li>
</ul>
При тестировании потока управления определяются различные уровни покрытия тестами. Под «покрытием» мы подразумеваем процент кода, который был протестирован, по сравнению с тем, который есть для тестирования. В тестировании потока управления мы определяем покрытие на нескольких различных уровнях. (Обратите внимание, что эти уровни охвата представлены не по порядку. Это связано с тем, что в некоторых случаях проще определить более высокий уровень охвата, а затем определить более низкий уровень охвата с точки зрения более высокого.):

<table>
<tr>
<td>Уровень
</td><td>Название
</td><td>Краткое описание
</td></tr>
<tr>
<td>Уровень 0
</td><td>--
</td><td>"Тестируй все что протестируешь, пользователи протестируют остальное" На английском языке это звучит намного элегантнее: "Test whatever you test, users will test the rest"
</td></tr>
<tr>
<td>Уровень 1
</td><td>Покрытие операторов
</td><td>Каждый оператор должен быть выполнен как минимум один раз.
</td></tr>
<tr>
<td>Уровень 2
</td><td>Покрытие альтернатив / Покрытие ветвей
</td><td>Каждый узел с ветвлением (альтернатива) выполнен как минимум один раз.
</td></tr>
<tr>
<td>Уровень 3
</td><td>Покрытие условий
</td><td>Каждое условие, имеющее TRUE и FALSE на выходе, выполнено как минимум один раз.
</td></tr>
<tr>
<td>Уровень 4
</td><td>Покрытие условий альтернатив
</td><td>Тестовые случаи создаются для каждого условия и альтернативы
</td></tr>
<tr>
<td>Уровень 5
</td><td>Покрытие множественных условий
</td><td>Достигается покрытие альтернатив, условий и условий альтернатив (Уровни 2, 3 и 4)
</td></tr>
<tr>
<td>Уровень 6
</td><td>"Покрытие бесконечного числа путей"
</td><td>Если, в случае зацикливания, количество путей становится бесконечным, допускается существенное их сокращение, ограничивая количество циклов выполнения, для уменьшения числа тестовых случаев.
</td></tr>
<tr>
<td>Уровень 7
</td><td>Покрытие путей
</td><td>Все пути должны быть проверены
</td></tr>
</table>

Подробный разбор с примерами доступен в источнике:
flylib.com/books/en/2.156.1/control_flow_testing.html
<h2>Что такое Loop coverage?</h2>
Loop testing определяется как тип тестирования программного обеспечения методом белого ящика, который полностью фокусируется на валидности конструкций цикла. Это одна из частей тестирования структуры управления (Control Structure testing): тестирование пути, проверка данных, тестирование условий (path testing, data validation testing, condition testing). 
Этот показатель сообщает, выполняли ли вы каждое тело цикла ноль раз, ровно один раз и более одного раза (последовательно). Для циклов do-while покрытие цикла сообщает, выполняли ли вы тело ровно один раз и более одного раза. Ценным аспектом этой метрики является определение того, выполняются ли циклы while и for более одного раза, т.к. эта информация не сообщается другими метриками. 
<img src="https://lh6.googleusercontent.com/jrZUePNsJu_L0YEInoPlwq9bcWqP1V0mDQSAx97y90qg4VMSRT8fzXwDYswLgZULSpr64kNlXPHlrd0h1fqYbPK8Ao3aAQ3fUIsDDRQ9teyp2OaOBy-IVkGEGMAj4EGDVaVKPUyj">
<h2>Что такое Race coverage?</h2>
Этот показатель показывает, выполняет ли несколько потоков один и тот же код одновременно. Это помогает обнаружить сбой при синхронизации доступа к ресурсам. Это полезно для тестирования многопоточных программ, например, в операционной системе.
<h2>Тестирование пути и тестирование базового пути? (Path testing & Basis Path testing)</h2>
Path testing - это метод структурного тестирования, который включает использование исходного кода программы для нахождения каждого возможного исполняемого пути. Это помогает определить все ошибки, лежащие в части кода. Здесь Test case выполняются таким образом, что каждый путь проходится по крайней мере один раз. Все возможные control paths, включая все loop paths. Test case подготавливаются на основе логической сложности. При таком типе тестирования каждый оператор в программе гарантированно выполняется как минимум один раз. Flow Graph, Cyclomatic Complexity и Graph Metrics используются для достижения basis path.
Любая программа включает в себя несколько точек входа и выхода. Тестирование каждого из этих пунктов является сложным и трудоемким. Для сокращения избыточных тестов и достижения максимального охвата тестов используется Basis Path testing. Basis Path testing такое же, но оно основано на методе White Box testing и определяет Test case на основе потоков или логического пути, которые могут быть пройдены через программу. В программной инженерии Basis Path testing включает в себя выполнение всех возможных блоков в программе и достижение максимального охвата пути с наименьшим количеством Test case. Это гибрид branch testing и path testing. Цель Basis Path testing состоит в том, что оно определяет количество независимых путей, таким образом, число необходимых Test case может быть определено явно (максимизирует охват каждого тестового случая).
Тесты критического пути (Critical path tests) запускаются для проверки функциональности, используемой обычными пользователями во время их повседневной деятельности. Многие пользователи обычно используют определенный набор функций приложения, который необходимо проверить, как только фаза smoke будет успешно завершена. Здесь метрический предел немного ниже, чем при smoke, и он соответствует 70-80-90% в зависимости от цели проекта при ста процентах у smoke. Чаще всего на практике, на данном уровне тестирования проверяется основная масса требований к продукту. Пример: выбор шрифта, возможность набора текста, вставки картинок и т. д. 

<img src="https://lh3.googleusercontent.com/ajhl7AreCw6oZrj4sOzSc0Yi3745bDWS_hrtMoMWtfb4CBx_cw6nsKPPKu6-miB1QRam6pfq1SrZ72g73lZf6FHfZmbr7jChLZ2Ls5uYeKbulEBJcuBuyH77Kifk4NmOWoT2nSQD">

<h2>Что вы знаете о Statement coverage?</h2>
Охват операторов - это метод проектирования теста белого ящика, который включает в себя выполнение всех исполняемых операторов (if, for и switch) в исходном коде как минимум один раз. Он используется для вычисления и измерения количества операторов в исходном коде, которые могут быть выполнены с учетом требований. Другими словами, тестировщик будет концентрироваться на внутренней работе исходного кода, касающегося control flow graphs или flow charts. Как правило, в любом программном обеспечении, если мы посмотрим на исходный код, будет множество элементов, таких как операторы, функции, циклы, обработчики исключений и т. д. В зависимости от входных данных программы некоторые части кода могут не выполняться. Цель покрытия Statement - охватить все возможные пути, строки и операторы в коде. Тестируются операторы потока управления, такие как. 
Покрытие операторов позволяет найти: 
<ul>
<li>Неиспользованные выражения (Unused Statements) 
</li>
<li>Мертвый код (Dead Code)
</li>
<li>Неиспользуемые ветви (Unused Branches) 
</li>
<li>Недостающие операторы (Missing Statements)
</li>
</ul>

<img src="https://lh3.googleusercontent.com/jdaV-ql5_cSd63nzi3alwtbXVJzCz3Lh0ROOws3y5tBG8XNmYGv2qBl8jJgcGcv5zlIEJAFlW7yFQqPj6PASJ2zAKl-V_pd90xuocQtV-ighRiXTbdjTbeZrWFMXgo8-ZbGNeGpz">
<h2>Что вы знаете о Decision coverage?</h2>
«Решение» - это программная точка, в которой control flow имеет два или более альтернативных маршрута. control flow- это последовательность событий (paths) при выполнении через компонент или систему. Таким образом, если быть точным, «решение» - это узел потока управления (например, оператор if, оператор цикла или оператор case), который имеет две или более ссылок на отдельные ветви выполнения. 100% покрытие решений означает, что все возможные результаты решения были выполнены по крайней мере один раз. Для утверждений if это правда или ложь. 
Иногда этот метод называют Branch testing.
<h2>Что вы знаете о Branch coverage?</h2>
В покрытии ветвей проверяется каждый результат из модуля кода. Например, если результаты являются бинарными, вам необходимо протестировать как истинные, так и ложные результаты. Это помогает вам гарантировать, что каждая возможная ветвь из каждого условия решения выполняется по крайней мере один раз. Используя метод покрытия Branch, вы также можете измерить долю независимых сегментов кода. Это также поможет вам узнать, какие разделы кода не имеют ветвей.

Если тесты имеют полный branch coverage, то мы можем сказать, что они также имеют полный statement coverage, но не наоборот. Причина заключается в том, что в branch coverage, кроме выполнения всех statements, мы также должны проверить, выполняют ли тесты все ветви, что можно интерпретировать как охват всех ребер в control flow branch.

<img src="https://lh5.googleusercontent.com/oFvBmLitKzTlWNP3sQSXYRvoVMIH9rT4J3OEEi9CrH5igqcSX2e5TUyhbiRzCD5-bAh4HLL2NPvcyAx2zPOy-fKDZQ_GA2dqjYhnn17T4iJkvwDp-0cdOZXlD-c8dsIDBSwbQdE4">
<h2>Что вы знаете о Condition coverage?</h2>
Покрытие условий (Condition/Toggle Coverage) - рассматриваются только выражения с логическими операндами, например, AND, OR, XOR. Условное покрытие обеспечивает лучшую чувствительность к control flow, чем decision coverage. Condition Coverage не дает гарантии о полном decision coverage.
Multiple Condition Coverage: Множественное покрытие условий сообщает, встречается ли каждая возможная комбинация условий. Test Case, необходимые для полного охвата решения несколькими условиями, приведены в таблице истинности логического оператора для решения. Как и в случае покрытия условий, покрытие нескольких условий не включает покрытие решений.
<h2>Что вы знаете о FSM coverage?</h2>
Покрытие FSM (FSM Coverage) - Покрытие конечного автомата, безусловно, является наиболее сложным методом покрытия кода. В этом методе покрытия вам нужно посмотреть, как много было переходов/посещений определенных по времени состояний (time-specific states). Оно также проверяет, сколько последовательностей включено в конечный автомат.
<h2>Что такое Function coverage?</h2>
Этот показатель показывает, вызывали ли вы каждую функцию или процедуру. Во время предварительного тестирования полезно обеспечить хотя бы некоторое покрытие во всех областях программного обеспечения. Широкое неглубокое тестирование быстро обнаруживает серьезные недостатки в наборе тестов.
<h2>Что такое Call coverage?</h2>
Этот показатель показывает, выполняли ли вы каждый вызов функции. Гипотеза состоит в том, что ошибки обычно возникают в интерфейсах между модулями. Также известен как покрытие пары вызовов (call pair coverage).
<h2>Что означает LCSAJ coverage?</h2>
LCSAJ (linear code sequence and jump) «линейная последовательность кода и переход». Эта вариация path coverage учитывает только подпути, которые могут быть легко представлены в исходном коде программы, не требуя flow graph. LCSAJ - это последовательность строк исходного кода, выполняемых последовательно. Эта «линейная» последовательность может содержать decisions, пока control flow фактически продолжается от одной строки к следующей во время выполнения. Подпути создаются путем объединения LCSAJ. Исследователи ссылаются на коэффициент покрытия путей длиной n LCSAJ как на коэффициент эффективности теста (TER) n + 2.
Его основное применение при динамическом анализе программного обеспечения, чтобы помочь ответить на вопрос «Сколько тестирования достаточно?». Динамический анализ программного обеспечения используются для измерения качества и эффективности тестовых данных программного обеспечения, где количественное определение выполняются в терминах структурных единиц кода при тестировании. В более узком смысле, LCSAJ является хорошо определенным линейным участком коды программы. При использовании в этом смысле, LCSAJ также называют JJ-путь, стоя для скачка к скачку-пути. 100% LCSAJ означает 100% Statement Coverage, 100% Branch Coverage, 100% procedure или Function call Coverage, 100% Multiple condition Coverage.
<h2>Сравнение некоторых метрик</h2>
Вы можете сравнить «относительные силы»? (relative strengths), когда более сильная метрика включает более слабую метрику. 
<ul>
<li>Decision coverage включает в statement coverage, поскольку выполнение каждой ветви должно приводить к выполнению каждого statement. Эта связь сохраняется только тогда, когда control flows непрерывно до конца всех основных блоков. Например, функция C / C ++ может никогда не вернуться для завершения вызывающего базового блока, потому что она использует throw, abort, семейство exec, exit или longjmp. 
</li>
<li>Path coverage включает в себя Decision coverage. 
</li>
<li>Predicate coverage включает в себя Path coverage и multiple condition coverage, а также большинство других метрик. 
</li>
</ul>
Показатели покрытия нельзя сравнивать количественно.
<h2>Что такое Equivalence Partitioning?</h2>
Хорошо известная техника и одна из самых используемых. Часто вы можете найти такое объяснение: Например, у вас есть диапазон допустимых значений от 1 до 10, поэтому вам просто нужно проверить одно значение из диапазона - «5» и одно вне диапазона - «0». Это очень простое и понятное объяснение, но оно может дать узкий взгляд на эту технику. Что если у нас нет диапазона чисел? Концепция разделения эквивалентности возникла из математики и понимания того, что такое класс эквивалентности и отношение эквивалентности, что может быть трудно быстро понять без математического бекграунда. Но для целей тестирования, я думаю, это можно упростить, определив его следующим образом: эквивалентное разделение - это подмножество элементов из определенного набора, которые обрабатываются Системой (тестируются) одинаково. Таким образом, вам не нужно выполнять тесты для каждого элемента подмножества, и достаточно одной проверки, чтобы охватить все подмножество. Следовательно, методика может быть описана как разделение всего набора данных ввода / вывода на такие разделы. И если у вас есть, например, набор данных, содержащий около 100 элементов, которые можно разделить на 5 разделов, вы можете уменьшить количество кейсов до 5. Хитрость заключается в том, чтобы увидеть и идентифицировать разделы. Их можно найти в наборах без номеров (например, листья деревьев, разделенные по цвету - желтый, зеленый и т. д.), или даже один элемент может быть классом эквивалентности (например, лифт обычно более полон на первом этаже, чем на других этажах). По мере того, как люди выходят из здания, поднимается лифт, поэтому первый этаж - это отдельный класс эквивалентности). Очень эффективная, экономящая время техника.
<h2>Что такое Boundary Value Analysis?</h2>
Анализ Граничных Значений (Boundary Value Analysis - BVA). Второй известный метод, который часто используется в паре с предыдущим. Идея этого метода заключается в проверке граничных значений для разделов эквивалентности, когда результат изменяется с действительного на недействительный (для этого раздела). Test case, основанные на этих значениях, чувствительны к ошибкам и имеют высокую вероятность обнаружения ошибок при использовании логических операторов (> вместо >=, < вместо >, || вместо && и т. l.).
Это описание немного неоднозначно. Для проверки границ мы должны проверять допустимые значения границ диапазона, плюс одно значение ниже и одно значение вне диапазона. Таким образом, для диапазона больше 1 и меньше или равного 10, это 1, 2 и 10, 11.
<h2>Что такое Error Guessing?</h2>
Предугадывание ошибки (Error Guessing - EG). Это когда тест аналитик использует свои знания системы и способность к интерпретации спецификации на предмет того, чтобы "предугадать" при каких входных условиях система может выдать ошибку. Например, спецификация говорит: "пользователь должен ввести код". Тест аналитик, будет думать: "Что, если я не введу код?", "Что, если я введу неправильный код? ", и так далее. Это и есть предугадывание ошибки.
<h2>Что такое Cause/Effect?</h2>
Причина / Следствие (Cause/Effect - CE). Это, как правило, ввод комбинаций условий (причин), для получения ответа от системы (Следствие), то есть Простая проверка базовых действий и их результата. Например, если нажать крестик в правом верхнем углу окна (причина), оно закроется (следствие). Или вы проверяете возможность добавлять клиента, используя определенную экранную форму. Для этого вам необходимо будет ввести несколько полей, таких как "Имя", "Адрес", "Номер Телефона" а затем, нажать кнопку "Добавить" - это "Причина". После нажатия кнопки "Добавить", система добавляет клиента в базу данных и показывает его номер на экране - это "Следствие".
Граф причинно-следственных связей похож на Decision Table и также использует идею объединения условий. И иногда они описываются как один метод. Но если между условиями существует много логических зависимостей, может быть проще их визуализировать на cause-effect graph. Здесь можно выделить три этапа: 
<ul>
<li>Определить условия и последствия 
</li>
<li>Нарисовать график со всеми логическими зависимостями и ограничениями 
</li>
<li>Преобразовать график в Decision Table, отслеживая каждую комбинацию причин, которые приводят к эффекту от эффекта (tracing each combination of causes that lead to an effect from the effect).
</li>
</ul>
<h2>Что такое Exhaustive testing?</h2>
Исчерпывающее тестирование (Exhaustive testing - ET) - это крайний случай. В пределах этой техники вы должны проверить все возможные комбинации входных значений, и в принципе, это должно найти все проблемы. На практике применение этого метода не представляется возможным, из-за огромного количества входных значений.
<h2>Какие вы знаете комбинаторные техники тест-дизайна?</h2>
Или, скорее, стоит рассматривать их как комбинаторные стратегии. Их основное назначение - создавать комбинации входных параметров на основе одного из приведенных ниже алгоритмов.
Все комбинации (All combinations): как видно из названия, этот алгоритм подразумевает генерацию всех возможных комбинаций. Это означает исчерпывающее тестирование и имеет смысл только при разумном количестве комбинаций. Например, 3 переменные с 3 значениями для каждой дают нам матрицу параметров 3х3 с 27 возможными комбинациями.
Попарное тестирование (Pairwise testing) — это техника формирования наборов тестовых данных. Сформулировать суть можно, например, вот так: формирование таких наборов данных, в которых каждое тестируемое значение каждого из проверяемых параметров хотя бы единожды сочетается с каждым тестируемым значением всех остальных проверяемых параметров. Смысл метода не в том, чтобы перебрать все возможные пары параметров, а в том, чтобы подобрать пары, обеспечивающие максимально эффективную проверку при минимальном количестве выполняемых тестов. С этой задачей помогают справиться математические методы, называемые ортогональными таблицами (OAT). Также существует ряд инструментов, которые помогают автоматизировать этот процесс.

Тестирование каждого выбора (Each choice testing): эта стратегия означает, что каждое значение каждого конкретного параметра должно использоваться как минимум один раз в тестовом наборе. Таким образом, полученное количество случаев будет равно количеству значений параметра с наибольшим диапазоном. Каждый выбор - это минимальная стратегия покрытия.

<table>
<tr>
<td>param1
</td><td>param2
</td><td>param3
</td></tr>
<tr>
<td>a
</td><td>1
</td><td>X
</td></tr>
<tr>
<td>b
</td><td>2
</td><td>Y
</td></tr>
<tr>
<td>c
</td><td>3
</td><td>
</td></tr>
<tr>
<td>
</td><td>4
</td><td>
</td></tr>
<tr>
<td>
</td><td>5
</td><td>
</td></tr>
<tr>
<td>Test Case
</td><td>param1
</td><td>param2
</td><td>param3
</td></tr>
<tr>
<td>1
</td><td>a
</td><td>1
</td><td>X
</td></tr>
<tr>
<td>2
</td><td>b
</td><td>2
</td><td>Y
</td></tr>
<tr>
<td>3
</td><td>c
</td><td>3
</td><td>X
</td></tr>
<tr>
<td>4
</td><td>a
</td><td>4
</td><td>Y
</td></tr>
<tr>
<td>5
</td><td>b
</td><td>5
</td><td>X
</td></tr>
</table>


Тестирование базового выбора (Base choice testing): для этой стратегии мы должны определить наши базовые значения для каждого параметра. Это могут быть самые распространенные, самые маленькие / самые большие, самые простые или значения по умолчанию. После того, как мы сделали наш базовый выбор, мы должны изменять значение каждого параметра по одному, сохраняя при этом значения других параметров фиксированными при базовом выборе. Пусть a, 2 и Y будут нашим базовым выбором. Тогда кейсы будут:

<table>
<tr>
<td>param1
</td><td>param2
</td><td>param3
</td></tr>
<tr>
<td>a
</td><td>1
</td><td>X
</td></tr>
<tr>
<td>b
</td><td>2
</td><td>Y
</td></tr>
<tr>
<td>c
</td><td>3
</td><td>Z
</td></tr>
</table>

<table>
<tr>
<td>Test Case
</td><td>param1
</td><td>param2
</td><td>param3
</td></tr>
<tr>
<td>1
</td><td>a
</td><td>2
</td><td>Y
</td></tr>
<tr>
<td>2
</td><td>b
</td><td>2
</td><td>Y
</td></tr>
<tr>
<td>3
</td><td>c
</td><td>2
</td><td>Y
</td></tr>
<tr>
<td>4
</td><td>a
</td><td>1
</td><td>Y
</td></tr>
<tr>
<td>5
</td><td>a
</td><td>3
</td><td>Y
</td></tr>
<tr>
<td>6
</td><td>a
</td><td>2
</td><td>X
</td></tr>
<tr>
<td>7
</td><td>a
</td><td>2
</td><td>Z
</td></tr>
</table>

Доп. материал:
<a href="https://habr.com/ru/company/tinkoff/blog/516132/">Меньше, чем пара. Еще один способ сокращения количества тестов</a>

<h2>Что такое тестирование ортогональных массивов? (OAT - Orthogonal Array testing)</h2>
Оно является техникой тестирования, которая использует ортогональные массивы для создания Test case. Это особенно полезно, когда тестируемая система имеет огромные входные данные. Например, когда необходимо проверить билет на поезд, необходимо проверить такие факторы, как - количество пассажиров, номер билета, номера мест и номера поездов. Один за другим проверка каждого фактора / ввода является громоздкой. Это более эффективно, когда инженер QA объединяет больше входных данных и проводит тестирование. В таких случаях мы можем использовать метод тестирования Orthogonal Array. Этот тип сопряжения или объединения входов и тестирования системы для экономии времени называется попарным тестированием (pairwise testing). Метод OATS используется для попарного тестирования. Сформулировать суть pairwise можно, например, вот так: формирование таких наборов данных, в которых каждое тестируемое значение каждого из проверяемых параметров хотя бы единожды сочетается с каждым тестируемым значением всех остальных проверяемых параметров.

В реальном мире у тестировщиков не будет свободного времени для выполнения всех возможных Test case, чтобы выявить дефекты, поскольку существуют другие процессы, такие как документация, предложения и обратная связь с заказчиком, которые необходимо учитывать на этапе тестирования. Следовательно, test managers хотели оптимизировать количество и качество Test case, чтобы обеспечить максимальное покрытие тестами с минимальными усилиями. Это усилие называется Test case Optimisation.
<ul>
<li>Систематический и статистический способ тестирования парных взаимодействий 
</li>
<li>Точки взаимодействия и интеграции являются основным источником дефектов. 
</li>
<li>Выполните четко определенные, краткие Test case, которые могут выявить большинство ошибок. 
</li>
<li>Ортогональный подход гарантирует попарное покрытие всех переменных.
</li>
</ul>
Формула для расчета ОАТ: 
<img src="https://lh3.googleusercontent.com/gD1NuYX818654itN9YgYgA3-mnuMyTC0qolFIb5LFibtj-nKqMjgMnyqs6shfj0DIIgvwsPpNt_wNY_gwHjKb4Bc3ouZ0T_WBnzoX9j9UVT7FO9jOLWsyO1Cq39qon5bTUE1Az2-">
Runs (N) - количество строк в массиве, что выражается в количестве тестовых случаев, которые будут сгенерированы. Factors (K) - Количество столбцов в массиве, что выражается в максимальном количестве переменных, которые могут быть обработаны. Levels (V) - максимальное количество значений, которые могут быть приняты для любого отдельного фактора. Один фактор имеет от 2 до 3 входов для тестирования. Это максимальное количество входов определяет уровни.
<h2>Что такое Domain analysis/testing?</h2>
Доменный анализ: Это тип функционального тестирования, направленный на разбиение диапазона возможных значений переменной (или переменных) на поддиапазоны (или домены), с последующим выбором одного или нескольких значений из каждого домена для тестирования, то есть на анализ показательных значений и взаимосвязи элементов. Основная цель Domain testing: предоставить стратегию по выбору минимального набора показательных тестов. Кроме того, оно проверяет, что система не должна принимать входные данные, условия и индексы за пределами указанного или действительного диапазона. Во многом доменное тестирование пересекается с известными нам техниками разбиения на классы эквивалентности и анализа граничных значений. Но доменное тестирование не ограничивается перечисленными техниками. Оно включает в себя как анализ зависимостей между переменными, так и поиск тех значений переменных, которые несут в себе большой риск (не только на границах).
<img src="https://lh4.googleusercontent.com/AK8Lzev0tHf3CY5qPl9RwTVyc6skY7OwPeOc3VNUbqhGOhGN0_Vox8gn6n_eznKucdjiq8lc8kKtIDAmqB4HbGCrka5Pze4hnstqy42vgJdmp8lH3jbZZfAetq9iMpkzXp4ZXI2W">


Доп. материал:
<ul>
<li><a href="https://bbst.courses/wp-content/uploads/2018/01/Kaner-Intro-to-Domain-Testing-2018.pdf">Introduction to Domain Testing</a>
</li>
<li><a href="https://www.developsense.com/articles/2006-10-MasterOfYourDomain.pdf">Master of Your Domain</a>
</li>
</ul>
<h2>Что такое Cyclomatic Complexity в тестировании ПО? </h2>
Это метрика ПО, используемая для измерения сложности программы. Это количественная мера независимых путей в исходном коде программы. Независимый путь определяется как путь, имеющий хотя бы одно ребро, которое ранее не проходило ни в одном другом пути. Цикломатическая сложность может быть рассчитана относительно функций, модулей, методов или классов в программе. Эта метрика основана на представлении программы как control flow. Поток управления изображает программу в виде графа, который состоит из вершин и ребер. На графе вершины представляют обработку задачи, а ребра представляют поток управления между вершинами.
Тестирование базового пути является одним из методов «белого ящика» и гарантирует выполнение хотя бы одного оператора во время тестирования. Он проверяет каждый линейно независимый путь в программе, что означает, что число тестовых примеров будет эквивалентно цикломатической сложности программы. <img src="https://lh3.googleusercontent.com/M36zomzoDi0nJxl7lwtoFrZQf1nHai5AP0pkauN8Yrsl5_b1T_BwM5YmxQxzs0Rg15BEqRFDNd38TQAhR49D_E5STDm90-VbbTzlLSrxEa7pG_9OsO4Rq4Kqpbk4J1JG6lrfhy0d">

V(G) = E - N + 2 где E – количество ребер, N –количество вершин
или
V(G) = P + 1 где P - Количество предикатных узлов (узел, содержащий условие)

<img src="https://lh3.googleusercontent.com/07MfQh-QsMF1wzGPUld6zCRjcclnmNlEpGiqINBMKEOaAeIoEUMaaDj1MSSEmcTzMS254HdiijyJZSWl_raGAijnd-4ASaufU5MiUqohZHLMMISUGy6UCcdU0FJWAeDbwO7Ty4B1">
Сложность 1-10 говорит о хорошо написанном коде, легкой тестируемости и экономичности. 10-20 и 20-30 говорят об усложненном коде и трудностях с тестированием такого кода вкупе с высокими затратами. Сложность больше 40 практически не поддается проверке и стоит очень дорого. Подсчитывается вручную в случае небольшого ПО или с помощью автоматизированного ПО для крупного.
Цикломатическая Сложность может оказаться очень полезной:
<ul>
<li>Помогает разработчикам и тестировщикам определять независимые пути выполнения 
</li>
<li>Разработчики могут быть уверены, что все пути были протестированы хотя бы раз 
</li>
<li>Помогает нам больше сосредоточиться на открытых (uncovered) путях 
</li>
<li>Улучшение покрытия кода 
</li>
<li>Оценка рисков 
</li>
<li>Использование этих метрик в начале цикла снижает риски
</li>
</ul>
<h2>Что такое State Transition testing?</h2>
Тестирование переходов между состояниями определяется как метод тестирования ПО, при котором изменения входных условий вызывают изменения состояния в тестируемом приложении (AUT). Это метод тестирования черного ящика, в котором тестировщик анализирует поведение тестируемого приложения для различных входных условий в последовательности. В этом методе тестировщик предоставляет как положительные, так и негативные входные значения теста и записывает поведение системы. Это модель, на которой основаны система и тесты. Любая система, в которой вы получаете разные выходные данные для одного и того же ввода, в зависимости от того, что произошло раньше, является системой конечных состояний. Техника тестирования переходов между состояниями полезна, когда вам нужно протестировать различные системные переходы. Этот подход лучше всего подходит там, где есть возможность рассматривать всю систему как конечный автомат
<ul>
<li>Состояние (state, представленное в виде круга на диаграмме) – это состояние приложения, в котором оно ожидает одно или более событий. Состояние помнит входные данные, полученные до этого, и показывает, как приложение будет реагировать на полученные события. События могут вызывать смену состояния и/или инициировать действия.
</li>
<li>Переход (transition, представлено в виде стрелки на диаграмме) – это преобразование одного состояния в другое, происходящее по событию.
</li>
<li>Событие (event, представленное ярлыком над стрелкой) – это что-то, что заставляет приложение поменять свое состояние. События могут поступать извне приложения, через интерфейс самого приложения. Само приложение также может генерировать события (например, событие «истек таймер»). Когда происходит событие, приложение может поменять (или не поменять) состояние и выполнить (или не выполнить) действие. События могут иметь параметры (например, событие «Оплата» может иметь параметры «Наличные деньги», «Чек», «Приходная карта» или «Кредитная карта»).
</li>
<li>Действие (action, представлено после «/» в ярлыке над переходом) инициируется сменой состояния («напечатать билет», «показать на экране» и др.). Обычно действия создают что-то, что является выходными/возвращаемыми данными системы. Действия возникают при переходах, сами по себе состояния пассивны.
</li>
<li>Точка входа обозначается черным кружком.
</li>
<li>Точка выхода показывается на диаграмме в виде мишени.
</li>
</ul>

 <img src="https://lh4.googleusercontent.com/phWpxnCHLiZETao25say3M3ZHuZVBuNwHpwxoF-gsIOxbC7vmTcUXBEGqOf8FUw54SUZblk1KdXwyiDjaNo9KuXgUhciHDld8tFHTIki6tEoa1UtFzlMxNVM-rZh03Eyou36AtnG">
Для наглядности возьмем классический пример покупки авиабилетов. Все начинается с точки входа. Мы (клиенты) предоставляем авиакомпании информацию для бронирования. Служащий авиакомпании является интерфейсом между нами и системой бронирования авиабилетов. Он использует предоставленную нами информацию для создания бронирования. После этого наше бронирование находится в состоянии «Создано». После создания бронирования система также запускает таймер. Если время таймера истекает, а забронированный билет еще не оплачен, то система автоматически снимает бронь.
Каждое действие, выполненное над билетом, и соответствующее состояние (отмена бронирования пользователем, оплата билета, получение билета на руки, и т. д.) отображаются в блок-схеме. На основании полученной схемы составляется набор тестов, в котором хотя бы раз проверяются все переходы.
Некоторым исследователям представляется более удобным свести весь процесс в таблицу состояний и переходов. Конечно, таблица не так наглядна, как схема, но зато она получается более полной и систематизированной, так как определяет все возможные State-Transition варианты, а не только валидные.

Еще пример с банкоматом. После того, как мы визуализировали все переходы, мы просто выполняем определенные пути из диаграммы в качестве Test case:
<img src="https://lh4.googleusercontent.com/2TD5SS9vTwd62HdQqjvlVqiYnN2-d1zaHww6eBBqoVjy7FkyJAI5lQ2b6O2jnYhumaCpnRRhRbXBzqImhnR_0zFyXSaQBSvH1xlT21qtReaM8POn6hzKypqyJLfvg7kdL5ApJxUV">
<h2>Что такое Scenario (use case) testing?</h2>
Use Case описывает сценарий взаимодействия двух и более участников (как правило – пользователя и системы). Пользователем может выступать как человек, так и другая система. Юзкейсы могут быть позитивными (Sunny day use case) – в приоритете, и негативными (Rainy day use case).
Целью этого тестирования является нахождение дефектов, которые трудно найти при тестировании частей/модулей отдельно. Но нужно понимать, что это не аналог приемочного тестирования (но может быть его частью) и оно не охватывает все возможные варианты путей.
Как правило, Test case представлен очень небольшим количеством действий и одним результатом. Сценарий, с другой стороны, представляет собой последовательность действий (с промежуточными результатами), которые приводят к достижению какой-то конкретной цели. Сценарии могут быть частью документации разработчика (scenario diagrams). Довольно часто они задокументированы в требованиях как «use cases» - сценарии, которые обычно описывают взаимодействие пользователя с Системой. Но часто эти сценарии не очень подробны. Кроме того, прежде чем использовать их для создания Test case, их необходимо подробно описать с помощью шаблона. Шаблоны могут варьироваться от проекта к проекту. Но среди таких обычных полей, как имя, цель, предварительные условия, актер (ы) и т. д., всегда есть основной успешный сценарий и так называемые расширения (плюс иногда подвариации). Расширения - это условия, которые влияют на основной сценарий успеха. А подвариации - это условия, которые не влияют на основной flow, но все же должны быть рассмотрены. После того, как шаблон заполнен данными, мы создаем конкретные Test case, используя методы эквивалентного разделения и граничных значений. Для минимального охвата нам нужен как минимум один тестовый сценарий для основного сценария успеха и как минимум один Test case для каждого расширения. Опять же, этот метод соответствует общей формуле «получите условия, которые меняют наш результат, и проверьте комбинации». Но способ получить это - проанализировать поведение Системы с помощью сценариев.
Пример: Рассмотрим сценарий, когда пользователь покупает товар с сайта онлайн-покупок. Пользователь сначала войдет в систему и начнет поиск. Пользователь выберет один или несколько товаров, отображаемых в результатах поиска, и добавит их в корзину. После всего этого он проверит. Так что это пример логически связанного ряда шагов, которые пользователь выполнит в системе для выполнения задачи. В этом тестировании проверяется поток транзакций во всей системе от конца до конца. Варианты использования - это, как правило, путь, который пользователи чаще всего используют для достижения конкретной задачи. Таким образом, это упрощает использование прецедентов при обнаружении дефектов, поскольку включает в себя путь, с которым пользователи чаще всего сталкиваются при первом использовании приложения.

Как создать хорошие сценарии (Сэм Канер):
<ol>
<li>Напишите истории жизни для объектов в системе.
</li>
<li>Перечислите возможных пользователей, проанализируйте их интересы и цели.
</li>
<li>Подумайте об отрицательных пользователях: как они хотят злоупотреблять вашей системой?
</li>
<li>Перечислите «системные события». Как система справляется с ними?
</li>
<li>Перечислите «особые события». Какие приспособления система делает для них?
</li>
<li>Перечислите преимущества и создайте сквозные задачи, чтобы проверить их.
</li>
<li>Интервью пользователей об известных проблемах и сбоях старой системы.
</li>
<li>Работайте вместе с пользователями, чтобы увидеть, как они работают и что они делают.
</li>
<li>Читайте о том, что должны делать подобные системы.
</li>
<li>Изучите жалобы на предшественника этой системы или ее конкурентов.
</li>
<li>Создать фиктивный бизнес. Относитесь к нему как к реальному и обрабатывайте его данные.
</li>
<li>Попробуйте преобразовать реальные данные из конкурирующего или предшествующего приложения.
</li>
</ol>
<h2>Что такое Decision Table testing?</h2>
Этот простой метод заключается в документировании бизнес-логики в таблице как наборов условий и действий. Например, если у вас есть набор переменных, которые трудно запомнить и управлять ими, таблица решений поможет упорядочить их, чтобы упростить идентификацию правильных случаев. 

Пример: если пользователь вводит правильное имя пользователя и пароль, он будет перенаправлен на домашнюю страницу. Если какой-либо из вводимых данных неправильный, появится сообщение об ошибке. 
<img src="https://lh5.googleusercontent.com/8t8si1_DAntjoadGKRGpIYaXc1q0BzajHy6ysedXazE18ETU-bs-ss6NLOU_JUEgTmrUguNhP0pW-qKZ70K6oHSE1Vq5NidyEcVhipjJT6yL6agmP7m8HyqvK_bmylfMcPwKfbcd">
<table>
<tr>
<td>Условие
</td><td>1
</td><td>2
</td><td>3
</td><td>4
</td></tr>
<tr>
<td>Имя пользователя (+/-)
</td><td>-
</td><td>+
</td><td>-
</td><td>+
</td></tr>
<tr>
<td>Пароль (+/-)
</td><td>-
</td><td>-
</td><td>+
</td><td>+
</td></tr>
<tr>
<td>Итог (E/H)
</td><td>E
</td><td>E
</td><td>E
</td><td>H
</td></tr>
</table>
Условные обозначения: «+» - правильное имя пользователя / пароль «-» - Неверное имя пользователя / пароль E - Сообщение об ошибке отображается H - отображается главный экран 
<ul>
<li>Случай 1 - имя пользователя и пароль были неверны. Пользователю показывается сообщение об ошибке.
</li>
<li> Случай 2 - Имя пользователя было правильным, но пароль был неправильным. Пользователю показывается сообщение об ошибке. 
</li>
<li>Случай 3 - Имя пользователя было неверным, но пароль был правильным. Пользователю показывается сообщение об ошибке. 
</li>
<li>Случай 4 - имя пользователя и пароль были правильными, и пользователь перешел на домашнюю страницу Преобразуя это в тестовый пример, мы можем создать 2 сценария: 
</li>
<ol>
<li>Введите правильное имя пользователя и правильный пароль и нажмите на кнопку входа, и ожидаемый результат будет пользователь должен перейти на домашнюю страницу 
</li>
<li>И один из сценария ниже: 
</li>
<ol>
<li>Введите неправильное имя пользователя и неправильный пароль и нажмите на кнопку входа, и ожидаемый результат будет, пользователь должен получить сообщение об ошибке 
</li>
<li>Введите правильное имя пользователя и неправильный пароль и нажмите на кнопку входа, и ожидаемый результат будет, пользователь должен получить сообщение об ошибке 
</li>
<li>Введите неправильное имя пользователя и правильный пароль и нажмите на кнопку входа, и ожидаемый результат будет, пользователь должен получить сообщение об ошибке
</li>
</ol>
</ol>
</ul>

<h2>Что такое Random testing?</h2>
Техника функционального тестирования (Black box), также известный как тестирование с произвольным вводом, это, вероятно, самый недооцененный метод, основная идея которого заключается в выборе случайных входных данных из возможных значений для определенной функциональности. Так что нет никакой системы в выборе входных данных. Этот метод также называется monkey testing, и если мы говорим о ручном тестировании, он может быть менее эффективным, чем другие методы черного ящика. Но если мы добавим автоматизацию, она станет мощным инструментом. Просто представьте, что Test case (с различными наборами входных данных) генерируются, выполняются и оцениваются автоматически в непрерывном цикле, что позволяет вам запускать тысячи и миллионы случаев в течение разумного времени. Создание «Случайного тестера» - довольно интересная тема, но также довольно сложная и требует более глубокого изучения. Здесь я опишу это только концептуально. 
В Monkey testing тестировщиком (иногда и разработчиком) считается «Обезьяна». Если обезьяна использует компьютер, она будет произвольно выполнять любую задачу в системе из своего понимания. Точно так же, как тестировщик будет применять случайные Test case в тестируемой системе, чтобы находить bugs/errors без предварительного определения тестового примера. В некоторых случаях Monkey testing также посвящен модульному тестированию или GUI-тестированию. Основная задача: попытаться сломать систему. 
Gorilla testing - это метод тестирования ПО, при котором модуль программы многократно тестируется, чтобы убедиться, что он работает правильно и в этом модуле нет ошибок. Модуль может быть проверен более ста раз одним и тем же способом. Gorilla testing также известен как «раздражающее тестирование».

<table>
<tr>
<td>Monkey testing
</td><td>Gorilla testing
</td></tr>
<tr>
<td>Тестирование выполняется случайным образом без каких-либо заранее определенных Test case
</td><td>Тоже
</td></tr>
<tr>
<td>Тестирование выполняется на всей системе может иметь несколько Test case
</td><td>Тестирование выполняется на нескольких отдельных модулях с небольшим количеством Test case.
</td></tr>
<tr>
<td>Целью Monkey testing является проверка на сбой системы
</td><td>Целью тестирования Gorilla является проверка правильности работы модуля.
</td></tr>
</table>


<table>
<tr>
<td>Monkey testing
</td><td>Ad-hoc testing
</td></tr>
<tr>
<td>Тестирование выполняется случайным образом без каких-либо заранее определенных Test case
</td><td>Тестирование выполняется без планирования и документации (контрольные примеры и SRS)
</td></tr>
<tr>
<td>В Monkey testing тестировщики могут не знать, что за ПО и для чего оно предназначено.
</td><td>В Ad-hoc testing тестировщик должен понять ПО перед выполнением тестирования
</td></tr>
<tr>
<td>Целью Monkey testing является проверка на сбой системы
</td><td>Целью специального тестирования является случайное разделение системы на части и проверка их функциональности.
</td></tr>
</table>
Типы Обезьян:
<ul>
<li>Тупая обезьяна: тестировщики не имеют представления о системе и ее функциональных возможностях, а также не имеют никаких гарантий относительно достоверности Test case. 
</li>
<li>Умная обезьяна: тестировщик имеет четкое представление о системе, ее назначении и функциональности. Тестировщик перемещается по системе и предоставляет действительные данные для выполнения тестирования. 
</li>
<li>Выдающаяся обезьяна: тестировщики выполняют тестирование в соответствии с поведением пользователя и могут указать некоторые вероятности возникновения ошибок.
</li>
</ul>
<h2>Что такое Syntax testing?</h2>
Синтаксическое тестирование - это метод проверки «черного ящика». Этот метод помогает при разработке Test case для входных форматов. Конечно, если наши правила синтаксиса звучат как «должны быть только цифры или буквы», нам не нужен этот метод. Но если у нас есть какой-то сложный формат (например, почтовый индекс, телефон, конкретный адрес электронной почты), это может быть удобно. Прежде всего, мы должны определить наш формат и описать его формально, используя форму Бэкуса-Наура (или расширенный BNF). Это очень важный момент, поэтому я бы посоветовал вам ознакомиться с BNF, прежде чем читать дальше. После того, как мы создали определение BNF для нашего формата, пришло время генерировать положительные и отрицательные кейсы: 
Для положительных случаев мы находим возможные варианты значений, допускаемые отдельными элементами определения BNF, а затем разрабатываем варианты, чтобы просто охватить эти варианты. 
Для случаев с недопустимым синтаксисом мы определяем и применяем возможные мутации (например, отсутствующий элемент, нежелательный дополнительный элемент, недопустимое значение для элемента и т. д.) к отдельным элементам определения BNF. Затем мы разрабатываем наши кейсы, применяя мутации, которые могут давать отличительные результаты (случаи, которые приводят к действительным комбинациям, исключаются).
<img src="https://lh4.googleusercontent.com/rFO5p5QbSo8mBKETsZ5cRbAzkuVwKkCOvvoS4koDBWXe0YFwLwnoF6KTiaL9m2EgOpNKCS02oQRFLOvVicH_3SVA49I0rtASYDl2haM1BvcNiDFl61xvMMIHVlReWVWATyI-X2R1">
<h2>Что вы знаете о Classification tree method?</h2>
Большинство ресурсов выделяют два основных шага для этой техники: 
<ul>
<li>Определение относящихся к тесту аспектов (аспектов, которые влияют на функциональность - так называемые классификации) и их соответствующих значений (называемых классами, это могут быть точные значения или классы эквивалентности). 
</li>
<li>Объединение разных классов из всех классификаций в Test case.
</li>
</ul>
Оба эти шага справедливы для большинства методов тестирования и могут быть перефразированы следующим образом: - определить параметры ввода / вывода, а затем объединить их, чтобы получить ваши кейсы. 
Теперь давайте добавим некоторые детали. Классификационное дерево - это графический метод, который помогает нам визуализировать относящиеся к тесту аспекты (аспекты, которые влияют на поведение тестового объекта во время теста) в форме иерархического дерева.
Как вырастить это дерево? Это похоже на интеллектуальные карты с небольшими отличиями, если это вам о чем-то говорит. У нас есть тестовый объект (целое приложение, определенная функция, абстрактная идея и т. д.) вверху как корень. Мы рисуем ответвления от корня как классификации (проверяем соответствующие аспекты, которые мы определили). Затем, используя распределение по эквивалентности и анализ граничных значений, мы определяем наши листья как классы из диапазона всех возможных значений для конкретной классификации. И если некоторые из классов могут быть классифицированы далее, мы рисуем под-ветку / классификацию с собственными листьями / классами. Когда наше дерево завершено, мы делаем проекции листьев на горизонтальной линии (Test case), используя одну из комбинаторных стратегий (все комбинации, каждый выбор и т. д.), и создаем все необходимые комбинации.
<img src="https://lh3.googleusercontent.com/HFPlp7_pJrF7S-mmqNcgMCPbUTkU8YgS3hpMcQrIaHdO-3phJSJxtbbaqHbXIdDRigrIx6Xqr-NRvK9VCb9MZcY5WnUJOR0s_zZQfHEQPI-Sq7-5uo5rkADcR1luaVFxc63Wpucu">
В приведенном выше примере использовалась комбинаторная стратегия «Каждый выбор». Наиболее очевидные преимущества здесь - это большая наглядность и ясность объема тестового объекта и идей Test case. Если у вас есть сложные, иерархически структурированные данные, и вы можете позволить себе тратить время на создание и поддержку дерева, этот метод будет чрезвычайно удобен. И для эффективного применения метода вы можете, например, рассмотреть возможность использования специального инструмента, такого как Classification Tree Editor.
<h2>Как мы узнаем, что код соответствует спецификациям? </h2>
Матрица прослеживаемости - это интуитивно понятный инструмент, который обеспечивает соответствие требований тестовым примерам. Когда выполнение всех Test case заканчивается успешно, это указывает на то, что код соответствует требованиям. 
<h2>Что включает в себя матрица отслеживания требований? (RTM - Requirement Traceability Matrix)</h2>
Матрица прослеживаемости - это документ, который связывает любые два базовых документа, которые требуют отношения «многие ко многим» для проверки полноты отношений. В случае тестирования это матрица покрытия функциональных требований тест-кейсами.
Есть даже такое понятие как Requirement based testing, которое имеет место быть, когда есть требования к продукту, на их основе составляются тест-сценарии и выполняется тестирование.
Зачем нужна эта матрица?
Например, для того чтобы:
- при разработке тестов четко ориентироваться какие из требований уже покрыты тестами, а какие еще нет;
- при выполнении тестирования ориентироваться какие из требований прошли все написанные для них тесты успешно, а какие - еще нет.
Матрица трассировки может служить одновременно в качестве матрицы покрытия. Наличие такой матрицы позволяет объективно оценить, какая часть продукта покрыта тестами, а какая нет. Это необходимое условие, чтобы оценить, какой объем работы мы уже выполнили и что еще осталось сделать - и по части создания, и по части выполнения тестов.
Еще одно преимущество traceability matrix – ее наглядность. Если она поддерживается в актуальном состоянии, то можно сразу увидеть "белые пятна" и сосредоточиться на них.
Traceability matrix также позволяет сравнивать тесты между собой по критерию количества требований, которые они покрывают. Одни тесты могут покрывать несколько требований, другие – только одно.
<h2>В чем разница между Test matrix и Traceability matrix?</h2>
Тестовая матрица: тестовая матрица используется для определения фактического качества, усилий, плана, ресурсов и времени, необходимых для охвата всех этапов тестирования программного обеспечения. 
Матрица прослеживаемости: сопоставление между Test case и требованиями.
<h2>Что такое анализ GAP? </h2>
Анализ пробелов выявляет любые отклонения между функциями, доступными для тестирования, и восприятием их клиентом. Матрица прослеживаемости - это инструмент тестирования, который тестировщики могут использовать для отслеживания пробелов. 
<h2>Что такое граф причинно-следственных связей? (Cause Effect Graph)</h2>
Это графическое представление входных данных и связанных с ними выходных эффектов, которые помогают в разработке Test case. 
<h2>В чем разница между предугадыванием ошибок и посевом? (Error guessing and error seeding)</h2>
Предугадывание -  методика разработки Test Suite, в которой тестировщики должны предполагать возможные дефекты и писать тестовые наборы для их представления. 
Seeding. Это процесс добавления известных ошибок в программу для отслеживания скорости обнаружения и удаления. Это также помогает оценить количество неисправностей, оставшихся в программе.
<h2>Стили тестов?</h2>
*источник утерян, аналогов не нашел
<ul>
<li>Output based verification (смотрим что возвращает)
</li>
<li>State based verification (смотрим состояние)
</li>
<li>Communication based verification (общение и зависимости)
</li>
</ul>
<h2>Техники тестирования требований?</h2>
<ul>
<li>Взаимный просмотр:
</li>
<ul>
<li>беглый просмотр — автор показывает свою работу коллегам, они в свою очередь дают свои рекомендации, высказывают свои вопросы и замечания;
</li>
<li>технический просмотр — выполняется группой специалистов;
</li>
<li>формальная инспекция — привлекается большое количество специалистов, представляет собой структурированный, систематизированный и документированный подход. Минус такого варианта — тратится много времени.
</li>
</ul>
<li>Вопросы — если возникают вопросы, то можно спрашивать у представителей заказчика, более опытных коллег.
</li>
<li>Тест-кейсы и чек-листы — хорошее требование должно быть проверяемым, чтобы это определить можно использовать чек-листы или полноценные тест-кейсы. Если можно быстро придумать несколько пунктов чек-листа — это уже хороший знак.  
</li>
<li>Исследование поведения системы — необходимо мысленно смоделировать процесс работы пользователя с системой, созданной по тестируемым требованиям, после этого определить неоднозначные варианты определения системы.
</li>
<li>Рисунки — графическое представление дает наглядное представление приложения, на рисунке проще увидеть, что какие-то элементы не стыкуются, где-то чего-то не хватает и т. д. 
</li>
<li>Прототипирование — сделав наброски пользовательского интерфейса, легко оценить применение тех или иных пользовательских решений
</li>
</ul>
<h2>Что такое эвристики?</h2>
Эвристики – это быстрые, недорогие способы решения проблемы или принятия решения. Эвристики подвержены ошибкам, то есть они могут как сработать, так и не сработать. Эвристики недостаточно абстрактны, они могут перекрываться и пересекаться друг с другом. Также эвристики зависят от контекста
Процесс тестирования на основе эвристик – это такая технология тестирования алгоритмов, приложений и программ, при использовании которой стратегия тестирования основывается на предыдущем опыте и данных о вероятности наступления различных событий.
<ul>
<li>Эвристика «Время вышло!» мы останавливаем тестирование, когда заканчивается выделенное на него время.
</li>
<li>Эвристика <a href="http://ru.wikipedia.org/wiki/%D0%9F%D0%B8%D0%BD%D1%8C%D1%8F%D1%82%D0%B0">пиньяты</a> (The Piñata Heuristic). Мы прекращаем ломать программу, когда начинают выпадать конфеты – мы останавливаем тестирование, когда видим первую достаточно серьезную проблему.
</li>
<li>Эвристика «мертвой лошади». В программе слишком много ошибок, так что продолжение тестирования не имеет смысла. Мы знаем, что все изменится настолько, что сведет на нет результаты текущего тестирования.
</li>
<li>Эвристика «Задание выполнено» останавливаем тестирование, когда найдены ответы на все поставленные вопросы.
</li>
<li>Эвристика «Отмена задания» Наш клиент сказал нам: «пожалуйста, прекратите тестирование». Это может произойти по причине перерасхода бюджета, или вследствие отмены проекта, и по любой другой причине. Какова бы ни была причина, нам поручили остановить тестирование. (На самом деле эвристика «Время вышло!» может быть частным случаем более общей «Отмены задания», в том случае, если предпочтительнее, чтобы не мы сами, а заказчик принял решение о том, что время вышло.)
</li>
<li>Эвристика «Я зашел в тупик!» По какой бы то ни было причине мы останавливаемся, поскольку обнаруживаем некое препятствие. У нас нет информации, которая нам требуется (например, многие люди заявляют, что не могут тестировать без достаточного количества спецификаций). Имеется блокирующая ошибка, и таким образом мы не можем перейти в ту область продукта, которую необходимо протестировать, у нас нет необходимого оборудования или инструментария, у команды нет квалификации, требуемой для выполнения некоторых специальных тестов.
</li>
<li>Эвристика «освежающей паузы» Вместо прекращения тестирования мы приостанавливаем его на некоторое время. Мы можем остановить тестирование и сделать перерыв, когда мы устали, когда нам стало скучно или пропало вдохновение. Мы можем сделать паузу на то, чтобы выполнить некоторые исследования, разработать планы, поразмыслить над тем, что мы делали в прошлом и понять, что делать дальше. Идея заключается в том, что нам требуется определенный перерыв, после которого мы сможем вернуться к продукту со свежим взглядом или свежими мыслями. Также есть и другой вид паузы: мы можем остановить тестирование какой-либо функции, поскольку в настоящий момент другая имеет более высокий приоритет.
</li>
<li>Эвристика «Отсутствие продвижения» Что бы мы ни делали, мы получаем тот же самый результат. Это может происходить в случае, когда программа падает определенным способом или перестает отвечать, но также мы можем не продвигаться, когда программа в основном ведет себя стабильно: "выглядит хорошо!"
</li>
<li>Эвристика Привычного завершения. Мы останавливаем тестирование тогда, когда мы обычно останавливаем тестирование. Имеется протокол, задающий определенное количество идей для тестирования, или тест-кейсов, или циклов тестирования, или как вариант – имеется определенный объем работ по тестированию, который мы выполняем и после этого останавливаемся. Agile-команды, например, часто применяют такой подход: «когда выполнены все приемочные тесты, мы знаем, что продукт готов к поставке. Отличие от эвристики «Время вышло!» в том, что временные ограничения могут изменяться более гибко, чем некоторые другие. 
</li>
<li>Больше нет интересных вопросов В этот момент мы решаем, что не осталось вопросов, ответы на которые были бы достаточно ценными, чтобы оправдать стоимость продолжения тестирования, и поэтому мы останавливаемся. Эта эвристика используется в основном как дополнение к другим эвристикам, помогая принять решение о том, есть ли какие-то вопросы или риски, которые отменяют действие этих эвристик (примеры таких вопросов я привожу после каждой эвристики). Кроме того, если одна эвристика советует нам прекратить тестирование, следует проверить, нет ли интересных вопросов или серьезных рисков в других областях, и если они есть, то мы скорее продолжим тестирование, чем остановимся.
</li>
<li>Эвристика уклонения/безразличия. Иногда людей не интересует дополнительная информация, либо они не хотят знать, что происходит в программе. Тестируемое приложение может быть первой версией, которую, как мы знаем, скоро заменят. Некоторые люди прекращают тестирование по причине лени, злого умысла или отсутствия мотивации. Иногда бизнес-критичность выпуска нового релиза настолько высока, что никакая мыслимая проблема не остановит выход программы, и поэтому никакие новые результаты тестирования не будут иметь значения.
</li>
</ul>
Дополнение: Кем Канер (Cem Kaner) предложил еще одну эвристику: «Отказ от выполнения задания» (Mission Rejected), в которой тестировщик сам отказывается от продолжения тестирования. Подробнее читайте здесь.
Процесс тестирования на основе эвристик – это такая технология тестирования алгоритмов, приложений и программ, при использовании которой стратегия тестирования основывается на предыдущем опыте и данных о вероятности наступления различных событий.

Мнемоника – это набор правил и приемов, которые помогают эффективно запоминать необходимые сведения (информацию).
Большинство экспертов с мировым именем в сфере тестирования настоятельно рекомендуют использовать проверенную схему SFDPOT, автором которой является Джеймс Бах. По их словам, это самый качественный и правильный инструмент для быстрой генерации тестовых идей и наработок.
Итак, что такое SFDPOT?
SFDPOT – Structures, Functions, Data, Platforms, Operations, Times:
<ul>
<li>Structures – архитектура приложения (продукта), которая проверяется по частям. На этом этапе создаются тестовые идеи и шаги, неразрывно связанные со структурой веб-продукта;
</li>
<li>Function – производительность приложения (продукта). Проверка того, что может выполнять приложение (продукт). На этом этапе проводится функциональное тестирование ПО;
</li>
<li>Data – взаимодействие с данными. Проверка приложения на взаимодействие с данными. QA специалисты должны определить по какой логике продукт взаимодействует с данными, как проходит их получение, тип обработки и виды информации;
</li>
<li>Platform – экосистема, платформа. Выполнение проверки того, как именно приложение (продукт) потенциально взаимодействует с платформой, на которой оно создано и запущенно. Тестировщик должен определить, на каких именно платформах и внутри каких систем необходимо провести процедуру ручного и автоматизированного тестирования;
</li>
<li>Operations – проверка созданных сценариев для разработанного приложения. На этом этапе перед тестировщиками постает задача по выяснению потенциального круга будущих пользователей, которые будут взаимодействовать с создаваемым продуктом;
</li>
<li>Time – период времени, проверка того, как продукт ведет себя в зависимости от наступления или завершения каких-либо временных промежутков.
</li>
</ul>

Что же касается CRUCSPIC STMP, то этот метод может рассматриваться как составная часть Operations внутри методики SFDPOT.
Если вкратце сказать о функциональности CRUCSPIC STMP, то можно отметить, что это своего рода атрибуты системы. Наработки CRUCSPIC STMP позволяют выделить основные объекты тестирования, его целей, а также построить карту эффективности взаимодействия между собой.

<img src="https://lh5.googleusercontent.com/cF5kpa8lvcZc7iPbcOBtyeb2f4VRsJEHErLQPMNNaiZmidqJi2Mjnmvb8LQN74fCZbW9KzzrLc0ffaIF_iRrk97dc6Nty3eIa3phvTawt9MlKLtM1-_qW-ugzg65BFUiYUIW0Oxs">
