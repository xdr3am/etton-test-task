# Тестовое задание Эттон
*Тестовое задание на позицию "Frontend - разработчик" в компанию Эттон.*
____
#### Для работы использовать следующие инструменты:
- Vue 2 / Vue 3 или Nuxt на усмотрение разработчика
- HTML или PUG по желанию
- SCSS в качестве CSS-препроцессора 

#### Запрещено использовать:
- Любые UI киты с готовыми компонентами
- CSS фреймворки

## Техническое задание

Необходимо сверстать 3 страницы представленные в 
[макете](https://www.figma.com/file/pj92WWkh8aCpMhJwbrHuBK/test-etton-01)

Результат должен быть представлен ссылкой на задеплоенную версию тестового задания

## Общие требования по стилю

- Шрифт - Montserrat
- Расположение блоков и элементов - согласно макета
- Верстка должна быть адаптивной

## #header

- Содержит в себе логотип и 2 кнопки навигации
- Клик на логотип переводит на главную страницу
- Клик на кнопки навигации переводят на соответствующие страницы и визуально показывают текущий роут
- Кнопка "Каталог" имеет активный статус на странице "Каталог" и на странице выбранного продукта

## #footer

- Содержит в себе ФИО кандидата и ссылку на выполненную работу на гитхабе
- Клик по ссылке открывает гитхаб кандидата в новом окне
- Футер всегда прижат к низу страницы

## Главная страница

- Содержит в себе заголовок в центре страницы

## Каталог

- Содержит список товаров и фильтры
- Список товаров приложен в файлике cats.json в папке data в корне этого репозитория
- Его нужно добавить в свой проект и использовать для отображения товаров
- Карточка товара отображает:

1. Картинка товара - поле img, картинки может и не быть, вместо нее нужно показать плейсхолдер (любой)
2. Название товара - поле title, имеет ограничение в 2 строки, далее скрывается за многоточие(...)
3. Цена товара - поле price, если price === 0, тогда вместо цены вывести слово "Бесплатно". Так же цена должа быть разделена тысячными пробелами (14 900 Р)

- Фильтр имеет следующие поля:
1. Поле поиска - фильтрует список товаров по полю title
2. Селект выбора категорий - фильтрует список товаров по полю categories, товары могут содержать в себе несколько категорий
3. Список опций для селекта приложен в файлике select.json, id опций соответствуют категориям товаров
4. Селект должен выглядеть как на макете, так же должна быть доступность выбора с клавиатуры
5. Чекбокс "Бесплатно" - показывает только бесплатные товары
6. Чекбокс "Не бесплатно" - показывает только платные товары
7. Если оба чекбокса нажаты то показываются обе категории товаров, так же это правило работает если не нажат ни 1 чекбокс
8. Фильтры применяются по кнопке "Применить"
9. Фильтры сбрасываются по кнопке "Сброс"
10. Кнопка "Сброс" появляется только если есть значение в каком либо фильтре (не распространяются на сортировку)

- По умолчанию сортировки по цене у списка товаров нет, при клике по кнопке сортировки товары становится либо по убыванию цены либо по возрастанию
- В мобильной версии Фильтры скрываются и открываются по кнопке, при клике "Применить" или "Сброс" фильтры скрываются
- При переключении между страницами фильтры не обнуляются, обнуление происходит только при обновлении страницы или по кнопке "Сброс"

## Страница товара

- Содержит в себе товар который выбрали на странице каталога
- При обновлении окна браузера данные о товаре не должны пропасть со страницы

## Критерии успешного прохождения

1) Работа соответствует ТЗ.

2) Верстка корректно отображается в последней версии Google Chrome (без флага).

3) Валидный код, отсутствуют ошибки.

# Удачи!
