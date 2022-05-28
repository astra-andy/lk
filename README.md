Личный кабинет абитуриента.

Создан макет дизайна с применением технологий HTML и CSS.
Кодировка файлов UTF8.
Шапка сайта помещена в отдельный файл _header.php
Подвал в _footer.php

index.php - Главная страница с формой авторизации.
Для входа необходимо ввести e-mail и пароль.

reg.php - Страница регистрации.
Поля: Ф.И.О., E-mail, Номер телефона, Паспортные данные (номер и кем выдан), пароль.
Все поля обязательны для заполнения. Проверяются на заполненность и валидность.
Если такой E-mail адрес уже есть в базе, то покажем ошибку.
Минимальная длина пароля 6 символов.
Сразу после регистрации возможна авторизация.

Авторизация.
После правильного ввода e-mail и пароля, происходит авторизация и переход на страницу lk.php
Выводится приветствие, дата регистрации и личные данные.
Ключ авторизации хранится в cookie, его время жизни 24 часа. Логин хранится 10 дней.
Если авторизованным зайти на главную, то произойдёт редирект на lk.php
Есть возможность редактировать личные данные.
Есть возможность выйти (завершить авторизацию).

list.php - Список всех зарегистрированных для администратора.
Видны все заполненные данные кроме пароля.
Есть возможность выключать/включать пользователей.
Если пользователь выключен, он не сможет авторизоваться.

core.sql - содержит команду MySQL для создания таблицы, которая
хранит информацию о зарегистрированных пользователях
