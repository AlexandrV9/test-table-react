<h1 align="center">Тестовое задание от компании Каналсервис</h1>


<h3 align="center">ТЗ (техническое задание):</h3>

Находится по следующей ссылке: https://kanalservis.notion.site/kanalservis/React-e07c83de444142dc8e743a2712934113



<h3 align="center">Список используемых технологий:</h3>

1) **React** - фреймворк для разработки пользовательских интерфейсов;
2) **MySQL** - система управления базами данных (СУБД);
3) **Axios** - JavaScript-библиотека для выполнения либо HTTP-запросов в Node.js.

<h3 align="center">Особенность данного проекта</h3>

Данный проект предназначени для фильтрации данных, пришедших от сервера.

Его особенность заключается в том, что прежде чем выполнять запрос к БД через сервер, отправится запрос на получения количества элементов удолетворяющих условиям фильтра. Если ничего не найдётся, то основной запрос на получения данных не отправится на сервер. Если же есть какие-то данные, то отправится основной второй запрос на получения массива данных, требующий дополнительного времени обработки.

Причём в приложении не загружаются сразу все данные (т.к. в БД их может быть очень много), а заграужаются малыми порциями. Т.к. в проекте есть пагинация, то одна страница - это один запрос на получение 7 элементов, вторая страница - это запрос на получение следующих 7 элементов.

Засчёт всего вышеперечисленного приложение работает очень быстро.



<h3 align="center">Алгоритм запуска приложения:</h3>

1. Для работы приложения, вам необходимо установить следующие инструменты:
    - [MySQL Workbench](https://dev.mysql.com/downloads/workbench/) - приложение для визуального проектирования баз данных;
    - [MySQL Community Server](https://dev.mysql.com/downloads/mysql/) - сервер для работы с SQL запросами;
2. Запустить MySQL Community Server;
3. Открыть MySQL Workbench:
    - Создать БД с названием TABLEDataBase;
    - Создать в этой БД таблицу с названием travel;
    - Добавить в эту схему следующие поля:
      * id - INT AI PK;
      * name - TEXT;
      * date - TEXT;
      * number - FLOAT;
      * distance - FLOAT;
    - После этого необходимо добавить в эту таблицу тестовые данные, любым удобным для вас способом (желательно, чтобы их было больше 60)
4. Далее производим установку и запуск сервер, который находится в другом репозитории. Скоро тут появится ссылка на него;
5. После этого скачиваем код данного репозитория;
6. Устанавливаем библиотеки с помощью команды: `npm i`;
7. Далее запускаем проект с помощью команды: `npm run start`;
8. Проект запущен ! :)

Автор данного проекта - Alexandr Vashchekin


