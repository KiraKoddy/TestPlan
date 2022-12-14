# Тест план
## Автоматизация тестирования формы записи на обучение профессии "Тестировщик ПО" на сайте Netology.ru

### Перечень автоматизируемых сценариев.
<strong>Переход на форму записи на обучение через "Каталог курсов" (хэддер вебстраницы)</strong>

1. Открыть главную страницу сайта "Нетология"
2. Перейти во вкладку "Каталог курсов" (хэддер)
3. Выбрать вкладку "Програмирование"
4. Выбрать профессию "Тестировщик ПО"

<strong>Переход на форму записи на обучение через виджет стартовой страницу</strong>

1. Открыть главную страницу сайта "Нетология"
2. Выбрать блок "Програмирование"
3. Выбрать профессию "Тестировщик ПО"
4. На странице присутствует форма записи на обучение

<strong>Переход на форму записи на обучение через "Выбрать курс"</strong>

1. Открыть главную страницу сайта "Нетология"
2. Перейти в каталог курсов через элемент страницы "Выбрать курс"
3. Выбрать профессию "Тестировщик ПО"
4. На странице присутствует форма записи на обучение

<strong>Переход на форму записи на обучение через "Каталог курсов" (футтер вебстраницы)</strong>

1. Открыть главную страницу сайта "Нетология"
2. Перейти во вкладку "Каталог курсов" (футтер)
3. Выбрать профессию "Тестировщик ПО"
4. На странице присутствует форма записи на обучение

<strong>Переход на форму записи на обучение через "Популярные курсы" (футтер вебстраницы)</strong>

1. Открыть главную страницу сайта "Нетология"
2. Перейти во вкладку "Популярные курсы" (хэддер)
3. Выбрать профессию "Тестировщик ПО"
4. На странице присутствует форма записи на обучение

<strong>Отправка формы на обучение (валидные данные)</strong>

1. Ввести валидные данные в поле "Имя" (например, Иван)
2. Ввести валидные данные в поле "Телефон" (одинадцать цифр)
3. Ввести валидные данные в поле "email" (например, test@test.ru)
4. Нажать на кнопку "Записаться"
5. Уведомление об успешной отправки формы

<strong>Отправка формы на обучение (не валидные данные, имя)</strong>

1. Ввести не валидные данные в поле "Имя" (например, Bdfy)
2. Ввести валидные данные в поле "Телефон" (одинадцать цифр)
3. Ввести валидные данные в поле "email" (например, test@test.ru)
4. Нажать на кнопку "Записаться"
5. Уведомление пользователя, что поле "Имя" в форме заполнено не корректно

<strong>Отправка формы на обучение (не валидные данные, телефон)</strong>

1. Ввести валидные данные в поле "Имя" (например, Иван)
2. Ввести не валидные данные в поле "Телефон" (десять/двенадцать цифр)
3. Ввести валидные данные в поле "email" (например, test@test.ru)
4. Нажать на кнопку "Записаться"
5. Уведомление пользователя, что поле "Телефон" в форме заполнено не корректно

<strong>Отправка формы на обучение (не валидные данные, email)</strong>

1. Ввести валидные данные в поле "Имя" (например, Иван)
2. Ввести валидные данные в поле "Телефон" (десять/двенадцать цифр)
3. Ввести не валидные данные в поле "email" (например, еуые""еуые.кг)
4. Нажать на кнопку "Записаться"
5. Уведомление пользователя, что поле "Email" в форме заполнено не корректно

<strong>Отправка формы на обучение (пустая)</strong>

1. Не вводить данные в поле "Имя", "Телефон", "Email"
2. Нажать на кнопку "Записаться"
3. Уведомление пользователя, что в форме имеются не заполненные поля

<strong>Тестирование API</strong>

1. POST запросы к API с валидными данными/не валидными данными/пустыми значениями
2. Корректное сохранение данных в базе данных

### Перечень используемых инструментов с обоснованием выбора.

- GitHub - хранение кода (доступность для команды)
- Selenide/Selenium - автоматизация тестирования, удобные инструменты тестирования Web-приложений
- IDEA - среда разработки, обширный набор инструментов для оптимизации кода
- Faker - удобная генерация случайных данных для атвотестов
- Postman - тестирование API, бесплатный, не требует предварительной сложной настройки
- Gradle - в качестве системы для автоматизации сборки приложений и сборе статистики, общая гибкость в настройках 
сборки

### Перечень необходимых разрешений, данных и доступов.

- Документация формы записи на обучение
- Разрешение на проведение автотестов, на доступ к базе данных (при необходимости), на тестирование API

### Перечень и описание возможных рисков при автоматизации.

- Изменение структуры страницы, актуализация автотестов - времязатраты
- При автотестах, данные могут случайно быть отправлены реальному менеджеру

### Перечень необходимых специалистов для автоматизации.

- QA Automation Enginee (Junior/Middle) для написания автотестов

### Интервальная оценка с учётом рисков в часах.
 - 4+ часа подготовка инструментов тестирвания, изучение документации, изучение прода/контура
 - 8-15 написание автотестов
 - 3+ подготовка отчетности 
 - 2+ поддержание актуальности тестов
 - регресс в установленные командой сроки (проверка актуальности тестов/изменение тестов/дописывание новых тестов)
