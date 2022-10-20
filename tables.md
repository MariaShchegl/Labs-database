# Описание сущностей
(имя поля, тип, ограничения, связь с другими сущностями)
## Книга (User Book)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| book_id | pk | auto increment; not null; unique | первичный ключ |
| title | VARCHAR(100) | not null | название книги |
| publisher_id |  |  | издатель |
| year | int| not null | год издания |
| isbn | int | not null | уникалный номер книги |
| cost | float | not null | цена за книгу |
| discount_id |  |  | скидка книги |
## Автор (Auther)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| author_id | pk | auto increment; not null; unique | первичный ключ |
| nickname | VARCHAR(100) | not null | псевдоним автора |
| rating | int | not null | рейтинг автора |
## Издатель (Publisher)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| publisher_id | pk | auto increment; not null; unique | первичный ключ |
| name | VARCHAR(50) | not null | название издателя |
| adress | VARCHAR(30) | not null | адресс издательства |
## Жанр (Genre)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| genre_id | pk | auto increment; not null; unique | первичный ключ |
| genre | VARCHAR(50) | not null | жанр |
## Сотрудник (Employee)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| employe_id | pk | auto increment; not null; unique | первичный ключ |
| name_surname | VARCHAR(100) | not null | имя, фамилия сотрудника|
| passport_id |  |  |  |
| phone_number | int | not null | номер телефона |
| post_id | int | not null | внешний ключ на клиента |
## Покупатель (Buyer)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| buyer_id | pk | auto increment; not null; unique | первичный ключ |
| nick | VARCHAR(100) | not null | ник покупателя |
| discount_id |  |  |  |
## Должность сотрудника (Post)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| post_id | pk | auto increment; not null; unique | первичный ключ |
| name_of_post | VARCHAR(100) | not null | название должности |
| salary | int | not null | зп |
| discount_id |  |  |  |
## Паспорт (Passport)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| passport_id | pk | auto increment; not null; unique | первичный ключ |
| registration | VARCHAR(50) | not null | регистрация |
| serial_number | int | not null | серийный номер |
| date_of_birth | date | not null | дата рождения |
## Скидка (discount)
|имя поля | тип | ограничения | описание |
|:---:|:---:|:---:|:---:|
| discount_id | pk | auto increment; not null; unique | первичный ключ |
| discount | int | not null | скидка |
