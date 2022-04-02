# Пользовательские истории (User stories)

_Пользовательская история (user story): Высокоуровневое пользовательское или бизнес-требование, обычно использующееся в гибких методологиях разработки программного обеспечения. Обычно состоит из одного или нескольких предложений на разговорном или формальном языке, описывающих функциональность, необходимую пользователю, любые нефункциональные требования и включающих в себя критерии приемки. (ISTQB)_

В индустрии разработки ПО слово «требование» определяет нашу цель, что именно нужно клиентам и что заставит нашу компанию развивать свой бизнес. Будь то продуктовая компания, которая производит программные продукты, или сервисная компания, которая предлагает услуги в различных областях программного обеспечения, основной базой для всех из них является требование, а успех определяется тем, насколько хорошо эти требования выполняются. Термин «требование» имеет разные названия в разных методологиях проекта. В Waterfall это называется Requirement/Specification Document, в Agile или SCRUM требования документируются в виде «Epic» и «User Story». В модели Waterfall документы с требованиями представляют собой огромные документы на сотни страниц, поскольку весь продукт реализуется за один этап. Но это не относится к Agile / SCRUM, потому что в этих случаях требования предъявляются к небольшим функциям или фичам, поскольку продукт готовится поэтапно.

Пользовательская история определяет требования к любой функциональности или фиче, в то время как критерии приемки (Acceptance Criteria) определяют критерии готовности (Definition of done) для пользовательской истории или требования.

![https://www.softwaretestinghelp.com/wp-content/qa/uploads/2018/02/User-Story-and-Acceptance-Criterion.jpg](https://www.softwaretestinghelp.com/wp-content/qa/uploads/2018/02/User-Story-and-Acceptance-Criterion.jpg)

**Пользовательская история** - это требование для любой функциональности или фичи, которое записано в 1-2 строки. Пользовательская история обычно является самым простым из возможных требований и касается одной-единственной функции/фичи.

**Формат**:

Как /_роль пользователя или клиента_/, я хочу /_цель, которую нужно достичь_/, чтобы я мог /_причина цели_/.

Например, “Как _пользователь WhatsApp_, я хочу, чтобы _значок камеры в поле ввода чата позволял захватывать и отправлять изображения_, чтобы я мог _щелкнуть и поделиться своими фотографиями одновременно со всеми своими друзьями_.”

Это стандартный формат, но далеко не обязательный или единственно-возможный. Главное  в пользовательской истории -  это ценность, которую пользователь получит от функции, т.е. User Story -  это приём записи требований, который помогает команде разработки понять нужду клиента и после обсуждения выбрать, описать и утвердить то решение, которое удовлетворит эту нужду.

**Job Stories**

В целом Job Stories - схожая с US техника. Можно назвать их приёмом-субститутом, ведь обычно они не используются вместе и выполняют максимально похожую функцию. Job Stories представляют требование в виде действия, которое выполняет пользователь. Они не описывают саму функцию, а лишь концентрируют внимание команды на потребности. Job Stories концентрируются на психологической части фичи, на эмоциях, тревогах и прочем, что может возникнуть во время использования функции.

“Тело” JS делится на три части:

* Situation: дает контекст обо всей JS, который помогает dev-команде придумать возможное решение;
* Motivation: описывает невидимую руку, которая ведет юзера к использованию данной функции;
* Expected Outcome: описывает, что получит юзер после использования функции.

Job Stories могут писаться по двум форматам:

* В одну строку: When X I want to Y so I can Z" или "When X, actor is Y so that Z;
* В три строки:
  * When X
  * I want to Y
  * So I can Z.

Пример: When I want to withdraw money from my bank account, I want to know I have enough money in my account to withdraw some now so that I can go out to dinner with my friends.

Источники:

* [What Is User Story And Acceptance Criteria (Examples)](https://www.softwaretestinghelp.com/user-story-acceptance-criteria/)
* [Гайд по User Stories](https://habr.com/ru/post/577420/)

Доп. материал:

* [User Stories Full Study: внутри и снаружи](https://www.youtube.com/watch?v=E07TXH\_QpY0)
* [10 советов для написания хороших пользовательских историй](https://habr.com/ru/company/otus/blog/546518/)
* [Гайд по Job Stories в помощь к написанию user stories](https://dkapaev.medium.com/%D0%B3%D0%B0%D0%B9%D0%B4-%D0%BF%D0%BE-job-stories-c7d513f72e8f)
* [Юзер-стори идеальная, а багов 100500? Как мы тестируем документацию](https://habr.com/ru/company/testit-tms/blog/564666/)
* [Job Stories Offer a Viable Alternative to User Stories](https://www.mountaingoatsoftware.com/blog/job-stories-offer-a-viable-alternative-to-user-stories)
* [25 sample user stories](https://www.yodiz.com/help/agile-user-stories-and-groomed-product-backlog/)
* [User Stories](https://www.agilealliance.org/glossary/user-stories/#q=\~\(infinite\~false\~filters\~\(postType\~\(\~'page\~'post\~'aa\_book\~'aa\_event\_session\~'aa\_experience\_report\~'aa\_glossary\~'aa\_research\_paper\~'aa\_video\)\~tags\~\(\~'user\*20stories\)\)\~searchTerm\~'\~sort\~false\~sortDirection\~'asc\~page\~1\))
* [User stories to acceptance criterias examples](https://i.pinimg.com/originals/35/4c/32/354c320f1bf9722791a7ccdbb40476cd.png)
* [The User Story Value Hypothesis](https://qablog.practitest.com/the-user-story-value-hypothesis/)
* [Use case или User story? Хватит выбирать - даешь все и сразу](https://www.youtube.com/watch?v=KNsznqqcUgI)
