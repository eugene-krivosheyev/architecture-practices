Ключевые практики архитектора ПО 
=================================
3 дня

Для кого
=========
- [ ] **Системные архитекторы**
- [ ] **Разработчики с функцией системного проектирования**
- [ ] Системные аналитики
- [ ] Enterprise- и Solution-архитекторы
- [ ] Разработчики

<!--
На выходе
==========
Участники смогут
- [ ] 
и получат инструменты для использования на производстве
- [ ] Архитектурный документ
-->

Программа
=========
18 ак.ч.

Знакомство (1 час, из них 0.5 практики)
----------
- [ ] Формат: 10:00 – 15:00
- [ ] Перерывы: 10:50 – 11:05, 12:00 – 13:00, 13:50 – 14:05 
- [ ] Материалы
- [ ] Разбивка на команды по трое
- [ ] Знакомство и сбор проблем участников
- [ ] Обзор тренинга

Что такое архитектура (1/0.5)
---------------------
- [ ] Что такое архитектура?
- [ ] Какова цель архитектурной работы? 
- [ ] На какие вопросы должна отвечать архитектура?
- [ ] Начинаем «Шаблон архитектурного документа с примерами» by example
- ключевые решения,
- структурная декомпозиция,
- договоренности/правила/guidelines развития

Стейкхолдеры проекта/продукта (1/0.5)
------------------------------
- [ ] На всем жизненном цикле системы кого касаются архитектурные решения? Кто участвует в разработке, приемке и эксплуатации системы? Кто несет ответственность за какой-либо аспект системы?
- [ ] В чем их интересы?
- [ ] Как можно выразить интересы в форме рисков?
- [ ] Какие артефакты архитектор ждет от них?
- [ ] Какие артефакты они ожидают от архитектора?
- [ ] Продолжаем Шаблон архитектурного документа
- [стейкхолдеры](https://www.stakeholdermap.com/stakeholders-it-project.html)
- коммуникационные задачи архитектора

Жизненный цикл системы (1/0.5)
-------------------------------
- [ ] Какие этапы/вехи можете выделить в ЖЦ проекта/продукта?
- [ ] Каковы критерии приемки для этих этапов?
- [ ] Какие артефакты должны измениться на этих этапах?
- [ ] Как можно выразить этапы в терминах рисков?
- [ ] Какие требования следует добавить в начало ЖЦ?
- [ ] Связываем Шаблон архитектурного документа с вехами ЖЦ
- [ ] Вехи зависят от степени неопределнности: 
- каждый спринт независим и требует существенной архитектурной работы
- спринты образуют [RUP-like вехи](https://sceweb.uhcl.edu/helm/RationalUnifiedProcess/process/itrwkfls/iwf_iwfs.htm), архитектура постепенно стабилизируется
- последовательный процесс с изначально стабильной архитектурой
- [ ] Неочевидные фазы опытной, промышленной эксплуатации и вывода из эксплуатации, влияющие на требования к системе

Что определяет архитектурные решения (1/0.5)
-------------------------------------
- [ ] Ревью входных ограничений для архитектуры:
- Корпоративные архитектурные ограничения
- Проектные архитектурные ограничения
- IT-ландшафт, куда будет встраиваться система
- Функциональные и нефункциональные требования к системе
- Инфраструктура разработки, тестирования, эксплуатации
- [ ] Почему такая последовательность приоритетов?
- [ ] Но так же ограничения формируются _внутри_ команды _в процессе_ производства:
- Атрибуты внутренней модели качества (ПТП+Г)
- Архитектурные [гайдлайны/соглашения](https://www.mediawiki.org/wiki/Architecture_guidelines)
- [ ] Продолжаем Шаблон архитектурного документа
- обоснуйте добавленные архитектурные ограничения
- обоснуйте [добавленные атрибуты](http://www.sqale.org/?page_id=66) внутренней модели качества

Требования как архитектурно значимый артефакт (1/0.5)
----------------------------------------------
- [ ] Даны требования к системе:
- FR в формате [User Story](https://www.atlassian.com/ru/agile/project-management/user-stories) / [Job Story](https://jtbd.info/replacing-the-user-story-with-the-job-story-af7cdee10c27)
- NFR в формате [атрибутов качества](https://en.wikipedia.org/wiki/Non-functional_requirement)
- [Доменная модель в формате UML-диаграммы классов](https://homepage.cs.uiowa.edu/~tinelli/classes/022/Spring15/Notes/chap9.pdf)
- [ ] Какие ожидания архитектор предъявит к этим требованиям для снижения рисков реализации: 
- обеспечения корректности,
- борьбы со сложностью, 
- параллельности работ, 
- обеспечения гибкости и других внутренних атрибутов качества.
- [ ] Понятие типовых профилей требований
- типовые риски реализации
- [ ] Продолжаем Шаблон архитектурного документа
- отразить ожидания к требованиям
- отразить свои типовые профили «требования - риски»

Ключевая проблема инженерии #2: противоречивость требований (1/0.5)
------------------------------------------------------------
- [ ] Проблема #1 – неполнота, но это out of scope
- [ ] Основные конфликты и важность в – NFRs (Attribute Driven Design, ADD)
- [ ] Примеры конфликтов характеристик
- [ ] Суть инженерии как работа в условиях конфликта характеристик
- [ ] Trade-off как основная деятельность архитектора ([Architecture Tradeoff Analysis Method, ATAM](https://en.wikipedia.org/wiki/Architecture_tradeoff_analysis_method))
- [ ] Приоритизация требований как ключ к trade-offs
- [ ] Как можно по-другому решить?
- Принцип специализации
- Компромисс
- [ ] Продолжаем Шаблон архитектурного документа
- документирование trade-off и причин решений

Ключевая проблема инженерии #3: неопределённость реализации (1/0.5) 
------------------------------------------------------------
- [ ] В зависимости от степени [неопределенности](https://en.wikipedia.org/wiki/Cynefin_framework):
- готовое оптимальное решение (best practice)
- анализ + паттерны (good practices)
- покупка в проект внешней экспертизы
- гипотезы + прототипы
- чистое исследование
- [ ] Продолжаем Шаблон архитектурного документа
- документирование решения
- документирование архитектурных прототипов

Ключевая проблема инженерии #4: изменчивость реализации (1/0.5)
--------------------------------------------------------
- [ ] Как обеспечить гибкость и параллельную разработку? Инкапсуляция
- [ ] Модули/Функции vs Компоненты/Реализации
- [ ] Практики функционального анализа и проектирования:
- модули -> контракты -> инкапсуляция в компоненты
- [ ] Trade-off: Suite или Best of breed?
- [ ] Продолжаем Шаблон архитектурного документа
- [ ] Практики описания архитектурных решений
- Отход от документирования в коде в пользу [читаемости](https://www.oracle.com/java/technologies/javase/codeconventions-contents.html) и [понимаемости](https://martinfowler.com/books/dsl.html) дизайна
- Подход [Lean к документации архитектурных решений](http://agilemodeling.com/essays/agileDocumentation.htm)
- Включение в [DoD](https://www.scruminc.com/definition-of-done/) обязательных результатов по документированию
- Контракты модулей/функций в формате [BDD-сценариев](https://en.wikipedia.org/wiki/Behavior-driven_development)
- Описание структуры системы как [граф зависимостей](https://docs.gradle.org/current/userguide/viewing_debugging_dependencies.html) на [заглушки других сервисов или компонентов системы](https://www.baeldung.com/spring-boot-rest-client-swagger-codegen) в инструменте сборки 
- Описание структуры системы в форме [IaaC](https://habr.com/ru/company/dododev/blog/465137/) как конфигурация правил файрволов
- Описание структуры системы в форме IaaC как конфигурации в инструменте [Service Discovery](https://habr.com/ru/post/487706/)
- Описание структуры системы в форме IaaC как конфигурации [среды работы контейнеров](https://learnk8s.io/visualise-dependencies-kubernetes)
- Легковесная модель описания основных архитектурных точек зрения [С4](https://c4model.com)
- Описание [целостной архитектуры](https://sparxsystems.com/resources/tutorials/archimate/index.html) на языке [ArchiMate](https://en.wikipedia.org/wiki/ArchiMate) в различных [средах моделирования](https://certification.opengroup.org/register/archimate-tool)

Ключевая проблема инженерии #5: сложность реализации (3/0.5)
------------------------------------------------------
- [ ] Как снизить риски разработки больших и сложных систем?
- [ ] Декомпозиция
- [ ] Документация
- [ ] [PoV](https://upload.wikimedia.org/wikipedia/commons/5/5b/Conceptual_model_Architectural_description.png)
- почему структурная декомпозиция так важна?
- PoV: как увидеть решения за диаграммами 
- разбор [ключевых PoV](https://www.viewpoints-and-perspectives.info/home/viewpoints/) и скрытых в них атрибутов качества


References
==========
- [Архитектура](https://ru.wikipedia.org/wiki/Архитектура_системы)
- [Обзор подходов к описанию архитектуры](http://sewiki.ru/Категория:Архитектурные_подходы)
- [RUP](https://sceweb.uhcl.edu/helm/RationalUnifiedProcess/)
- [TOGAF](http://sewiki.ru/TOGAF)
- [ISO 42010](https://www.iso.org/ru/standard/50508.html)
- [SWEBoK](https://www.computer.org/education/bodies-of-knowledge/software-engineering)
- [SEMAT](http://semat.org/essence-user-guide)
- [Ardoq](https://www.ardoq.com)
- [Системная инженерия](http://sewiki.ru/Системная_инженерия)
- [RUP SWA document](https://sceweb.uhcl.edu/helm/RationalUnifiedProcess/process/artifact/ar_sadoc.htm)
