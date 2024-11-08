# UserStory Формирование заказа

## US 06: Я как Посетитель ХОЧУ просмотреть историю заказов ЧТОБЫ иметь возможность повторить заказ блюд, которые понравились
### Acceptance Criteria 
- Пользователь может просматривать список всех прошлых заказов с деталями (название блюда, дата, стоимость)
### Tasks
1. Добавить возможность просмотреть историю заказов
> Необходимо добавить кнопку "История заказов", чтобы пользователь мог просмотреть прошлые заказы и их состав.
### TestCase
- Просмотр списка всех прошлых заказов с деталями

## US 07: Я как Посетитель ХОЧУ повторить заказ ЧТОБЫ быстро сделать заказ из любимых блюд, не собирая корзину заново
### Acceptance Criteria 
- Каждый заказ должен содержать возможность «Повторить заказ», чтобы быстро добавить блюда в корзину.
- При повторении заказа корзина автоматически обновляется с новыми блюдами, включая актуальные цены.
### Tasks
1. Добавить функциональность «Повторить заказ»
> При нажатии на «Повторить заказ» добавлять все позиции из прошлого заказа в текущую корзину  с актуальными данными.
### TestCase
- Работа кнопки "Повторить заказ"
- Проверка актуальности цен при повторном заказе

## US 08: Я как Посетитель ХОЧУ видеть предложения по другим блюдам, которые будут сочетаться с моим выбранным блюдом ЧТОБЫ заказать максимально вкусный и гармоничный состав блюд
### Acceptance Criteria 
- При выборе блюда пользователю показываются рекомендации по дополнительным блюдам, которые хорошо сочетаются.
- Рекомендации отображаются на странице выбранного блюда и могут быть добавлены в корзину одним кликом.
### Tasks
1. Создать алгоритм рекомендаций сопутствующих блюд
> Настроить рекомендации на основе выбранного блюда (например, «Людям, заказавшим это, понравилось также...»). Отображать список рекомендуемых блюд на странице с подробной информацией о выбранном блюде.
2. Добавить возможность быстрого добавления рекомендованных блюд в корзину
> Реализовать кнопку «Добавить в корзину» возле каждого рекомендованного блюда.
### TestCase
- Проверка отображения рекомендаций
- Проверка добавления рекомендуемого блюда в корзину

## US 09: Я как Посетитель ХОЧУ воспользоваться поиском по названиям блюд ЧТОБЫ быстрее найти необходимое блюдо
### Acceptance Criteria 
- Пользователь может ввести название блюда в строку поиска и увидеть подходящие результаты.
- Результаты поиска обновляются в реальном времени при вводе запроса.
### Tasks
1. Добавить строку поиска на странице меню
> Разработать интерфейс для ввода текста и отображения результатов.
2. Реализовать функцию обновления результатов в реальном времени
> Поддерживать отображение подходящих результатов при каждом вводе символа.
### TestCase
- Проверка работы поиска блюда в режиме реального времени

