# Требования к проекту 
## Для компании iShev-Soft Solutions

Версия 1.0  
Подготовлено Егором Шинкаревичем

Содержание
=================
* 1 [Введение](#1-введение)
* 2 [Требования пользователя](#2-требования-пользователя)
  * 2.1 [Программные интерфейсы](#21-программные-интерфейсы)
  * 2.2 [Интерфейс пользователя](#22-интерфейс-пользователя)
  * 2.3 [Характеристики пользователей](#23-характеристики-пользователей)
* 3 [Системные требования](#3-системные-требования)
  * 3.1 [Функциональные требования](#31-функциональные-требования)
  * 3.2 [Нефункциональные требования](#32-нефункциональные-требования)
* 4 [Внешний вид приложения](#3-внешний-вид-приложения)


## 1. Введение
> Название продукта - CODELANG.
Продукт является полноценным клиент-серверным приложением и представляет собой аналог социальной сети для программистов, в которой разработчики могут делиться своим кодом, просматривать код других пользователей, оценивать и комментировать.

Проект позволяет зарегистрированным пользователям создавать сниппеты(фрагменты кода). Под созданным сниппетом другие пользователи могут делиться своим мнением, оставив комментарий. Должна быть предоставлена хорошая система оценивания. Зарегистрированный пользователь должен иметь возможность оценить сниппеты других пользователей, поставить лайк или дизлайк.

## 2. Требования пользователя

### 2.1 Программные интерфейсы
Для осуществления всех возможностей продукт будет активно взаимодействовать с Firebase для использования хранилища с целью хранения картинок пользователей.

### 2.2 Интерфейс пользователя
Проект включает в себя как клиентскую, так и серверную части.
Клиент должен быть реализован с использованием современных фронтенд технологий, в частности такого фреймворка как Nuxt.js, который построен на Vue.js и позволяет осуществлять Server Side Rendering.
Серверная часть проекта должна быть реализована с использованием современного JavaScript бэкенд фреймворка Nest.js, базы данных PostgresQL. Также сервер должен иметь хорошую документацию для упрощения работы фронтенд разработчика. Документация должна быть сделана с помощью Swagger для Nest.js.
Пользователь должен иметь возможность поменять язык приложения. Должны быть представлены два языка - Русский и Английский.

### 2.3 Характеристики пользователей
Пользователи разбиваются на 3 группы:
1. Администраторы
2. Обычные пользователи
3. Гости

Гость это пользователь, который использует приложение без регистрации. Такие Пользователи могут просматривать сниппеты, лайки, комментарии и профили других пользователей. У них нет возможности для создания чего-либо. Они могут только смотреть.
Обычный пользователь это пользователь, который зарегистрировался и зашёл в свой аккаунт. Эти пользователи могут всё что и гости, но при этом у них есть возможность создавать сниппеты, оценивать, комментировать. Также они могут удалить свои сниппеты и комментарии, отменять лайки и дизлайки, удалять свой профиль, выйти из профиля.
Администратор это самый привелигерованный пользователь. У него есть такие же права как и у типов пользователей перечисленных выше. Также Администратор может удалять профили пользователей, комментарии пользователей, удалять сниппеты других пользователей. 

## 3. Системные требования

### 3.1 Функциональные требования
Должны быть реализованы следующие возможности:
1. Регистрация пользователей
2. Авторизация пользователей
3. Создание сниппетов
4. Просмотр сниппетов других пользователей
5. Комментирования сниппетов
6. Оценка сниппетов

### 3.2 Нефункциональные требования
1. Версия Node.js 16.0.
2. Версия Nest.js 9.0.
3. Само приложение на Nuxt.js + Nest.js.
4. Для хранения данных пользователей PostgresQl версии 9.0.
5. Для хранения всех фото и файлов, используется Firebase Storage.
6. Во время разработки рекомендуется использовать Docker.

## 4 Внешний вид приложения

## 4.1 Главная страница
![image](https://user-images.githubusercontent.com/72657584/194246619-fe543928-41db-46aa-9bc6-cc63c12c4b52.png)

## 4.2 Страница входа
![image](https://user-images.githubusercontent.com/72657584/194247014-8d59d469-98e4-470c-9fa6-43dc0a372149.png)

## 4.3 Страница регистрации
![image](https://user-images.githubusercontent.com/72657584/194247079-3ef33efa-171e-423f-a61c-270bdbae52de.png)

## 4.4 Страница профиля пользователя
![image](https://user-images.githubusercontent.com/72657584/194247216-a72e6ed4-3029-4e54-b06f-384383840732.png)

## 4.5 Страница создания сниппета
![image](https://user-images.githubusercontent.com/72657584/194247267-65f2cd61-a026-4cac-a232-a070a7eaa65d.png)



