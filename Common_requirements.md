# Протокол сбора требований к проекту "Робот и точка" со стейкхолдеров

**Дата**: 16.05.2024  
**Начало**: 20:00  
**Окончание**: 22:00  
**Общее время совещания**: 120 минут  

## Стейкхолдеры

| № | ФИО                       | Роль/Должность                |
|:--|:--------------------------|:------------------------------|
| 1 | Иванов Олег Николаевич    | Генеральный директор          |
| 2 | Сафин Максим Алексеевич   | Менеджер продукта             |
| 3 | Елизарова Анна Михайловна | Технолог                      |
| 4 | Назарец Никита Олегович   | СТО (Chief Technical Officer) |


### Выявление требований генерального директора

|№|Вопрос|Требование|Тип|Комментарий|
|-|-|-|-|-|
| 1|Какая цель данного проекта?|Внедрение данного проекта должно сократить операционные расходы на 30% в течение одного года|Бизнес|Один пилотный проект.Сокращение операционных расходов/людей, при условии прежней или даже лучшей производительности.|
|2|Какие сроки реализации пилотного проекта?|Пилотный проект должен быть реализован за год|Бизнес|После года будет приниматься решением по распространению данного функционала на остальные рестораны сети|
|3|Какое финансирование проекта?|Проект должен уложиться в 100 млн рублей собственных средств|Бизнес| |

### Выявление требований менеджера продукта

|№|Вопрос|Требование|Тип|Комментарий|
|-|-|-|-|-|
| 1|Что из себя должен составлять MVP?|Через год должен быть работающий ресторан, где автоматизированы технологические процессы с помощью внедрения роботов|Бизнес|Часть персонала остается|
|2|Какие процессы необходимо автоматизировать?|В рамках реализации проекта необходимо автоматизировать процесс приготовления, комплектации и выдачи блюд, также требуется разработка и внедрение тачпоинта в ресторане, мобильного приложения и табло заказов.|Бизнес| |
|3|Какие роботы должны применяться и в каком количестве?|В проекте должно использоваться по два робота для каждой из следующих функций: приготовления/жарки булочек; для гриля/фри; для напитков; нарезка в холодном цехе/салаты; заправщик/сборщик каждого блюда; комплектовщик заказов|Бизнес|Роботы уже закуплены со всеми документами. Робот-комплектовщик собирает заказ в зависимости от того какой был заказ (с собой или здесь), люди сами подходят, когда, например, на табло загорается их номер заказа.|
|4|Какая концепция данного ресторана?|Ресторан должен соответствовать концепции ресторана быстрого питания|Бизнес|Бургеры, картошка фри, напитки, готовые десерты|
|5|Какое время работы ресторана?|Система в ресторане должна работать круглосуточно|Функциональные|Допускаются технические перерывы для обслуживания роботов|
|6|Кто составляет целевую аудиторию ресторана?|Ресторан должен быть ориентироваться на целевую аудиторию - студенты/учащиеся, работающие люди, которые хотят быстро перекусить.|Бизнес| |
|7|Каким предполагается процесс процесс обработки заказа роботами?|После того, как посетитель оставляет заказ, он должен распределиться по блюдам, далее на еще более составные части. Далее роботы, распределенные по обязанностям должны подготовить свои блюда и направить к роботу-заправщику, который собирает бургеры и другие блюда. После чего готовые блюда едут к роботу-комплектовщику, который должен выдать заказ посетителю.|Бизнес|Приготовление одного блюда - именно взаимодействие роботов в рамках данной задачи - уже реализовано на стороне роботов. То есть, напиток готовит один робот, ставит на ленту, котлету жарит другой, салат и булочку готовят еще другие роботы.|
|8|Нужны ли отчеты, дашборды? Если да, то как часто?|Система должна предоставлять все возможные отчеты. Основные - сколько блюд заказано, в разрезе дня/заказов, средние суммы заказов, проценты потерь, скорость обработки блюда и подобное.|Функциональные|Хочется видеть все отчеты.Все, что успеем сделать в рамках MVP - необходимо сделать.|
|9|Необходим ли мониторинг в режиме реального времени?|Требуется реализация выгрузки отчетов по клику в любой момент времени. Мониторинг состояния роботов должен собираться и обрабатываться в режиме реального времени.|Функциональные|Выгрузка по заказам в режиме реального времени не интересует. За состоянием роботов будет следить технолог, который будет находиться с ними в одной комнате.|
|10|Кого из персонала планируется оставить?|В рамках проекта должны остаться следующие должности, которые заняты людьми: технолог – следит за роботами, мониторит состояние, время прожарки и подобное; главный технолог – может менять рецептуру блюда, граммовки, состав; менеджер по гостеприимству - решает  конфликты, может помочь сделать заказ, отменить заказ, сделать возврат и подобное|Функциональные|технологи возможно работают сменами, админы зала тоже. У менеджера по гостеприимству скорее всего должен быть свой интерфейс. Возможно, охранник и кассир|
|11|Есть ли документация к ПО роботов?|Работа с роботами осуществляется с помощью API, документация которого приложена к самим роботам.|Функциональные| |
|12|Какие приоритеты у основных функций, которые надо автоматизировать?|При разработке проекта должны соблюдаться следующие приоритеты автоматизации процессов: процесс приготовления; заказ с помощью тачпоинта в ресторане и табло выдачи заказа; мобильное приложение для заказа|Функциональные| с существующими системами необходимо только интегрироваться|
|13|Какие платежные системы необходимо поддержать?|В проекте должна быть поддержка оплаты с помощью СБП|Функциональные|Рассматривается вариант оставить кассира для заказа и оплаты наличными|

### Выявление требований технолога

|№|Вопрос|Требование|Тип|Комментарий|
|-|-|-|-|-|
| 1|Какие основные требования точно должны быть?|В системе должна быть реализовано проверка наличия продуктов, чтобы можно было заказать только те блюда, которые можно приготовить с имеющимися продуктами.|Функциональные|В идеале не показывать блюда, продуктов на которые нам не хватает|
| 2|Как выполняется распределение заказов по роботам?|Заказы должны распределяться по очереди на свободных роботов по их “должностям”. Если один робот ломается, то второй робот должен брать работу на себя.|Функциональные|Эти моменты заложены в ПО роботов|
|3|Что должен делать технолог в приложении по настройке роботов?|Система должна иметь интерфейс для настройки параметров каждого робота.|Функциональные|У робота есть танкер, где он показывает сколько ингредиентов в него загружено|
|4|Каким образом будет передаваться заказ посетителю?|Выдача заказа посетителю должна осуществляться роботом-комплектовщиком после вывода номера заказа на табло.|Функциональные| |
|5|Какие есть уровни доступа пользователей в приложении по настройке роботов? |В приложении для управления роботами должны быть реализованы следующие роли: Обычный технолог – управляет параметрами; Старший технолог – может менять меню |Функциональные|Если не успеваем, то можно не делать ролевую модель|
|6|Производит ли компания полуфабрикаты?|Система должна уметь работать с уже закупленными полуфабрикатами, не ориентируясь на закупки и заготовки отдельных продуктов.|Функциональные| |
|7|Что делать в случае отключение электричества?|Система должна следовать следующему алгоритму в случае отключения электричества: Короткий старт – перезагрузка в течение 2 мин, ресторан не закрывается; Длинный старт – если был простой, то надо проверить все жидкости и все характеристики (вкл, проверка и нагрев оборудования). Это может занимать примерно 10 минут. В такой ситуации ресторан должен быть закрыт на время технического сбоя.|Функциональные| |
|8|Какое максимальное время простоя допустимо?|Если простой системы составляет менее 2 мин, то процесс готовки необходимо продолжить. Если простой был более 2-5 минут – то необходимо загрузить новые продукты и выполнить готовку блюда заново.|Функциональные| |
|9|Какое время ожидания заказа?|Система должна обеспечивать переход заказа на кухню с момента оплаты в течение 1 минуты. Время приготовления должно составлять не более 2 минут. Также система должна уметь “предсказывать” заказы и  заранее готовить.|Функциональные| |


### Выявление требований CTO

|№|Вопрос|Требование|Тип|Комментарий|
|-|-|-|-|-|
| 1|Нужно ли выполнять меры 152 ФЗ?|В рамках данного проекта не требуется хранить персональные данные|Функциональные|Скорее всего используем только телефон и имя (без фамилии и даты рождения). Возврат осуществляем только с паспортом. Для MVP не требуется хранение персональных данных|
|2|Как и куда должны приходить отчеты?|Отчеты от системы должны приходить письмом на email. Также должны быть возможна выгрузка из базы данных it - специалистом.|Функциональные| |
|3|Что происходит, если робот выключается по той или иной причине?|Система оркестрации роботов должна принимать решение по координации работы роботов.|Функциональные| |
|4|Как происходит идентификация клиентов|В системе должна быть реализована идентификация клиентов по номеру телефона и имени|Функциональные|Для MVP допускается максимальное урезанный по функционалу личный кабинет|



















































