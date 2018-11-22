# Консольный FTP-клиент

+ Версия: 1.1
+ Автор: [Дружинин Егор](http://github.com/hexlify/)

## Описание

Данный клиент предназначен для работы с серверами по протоколу FTP

Требование: `python3.6+`

## Консольный FTP-клиент

```
$ python client.py [-h] [--port PORT] [--login LOGIN] [--verbose]
                 host {put,get,ls} ...
```

### Ключи

+  `host` - указывает адрес хоста
+ `[-h]` - справка по клиенту
+  `--port PORT`, `-p PORT` - указывает порт для подключения
+  `--user USERNAME`, `-u USERNAME` - указывает имя пользователя
+ `--passwd PASSWD` - указывает пароль
+ `--debug` - режим debug

Консольный клиент поддерживает следующие команды, которые можно указать как ключи при запуске в терминале. После их выполнения клиент завершит работу

### Команды CLI:

+ `put (upload)` - скачивание файла (папки) с сервера
+ `get [-r] (download)` - загрузка файла (папки) на сервер
+ `ls` - вывод содержимого директории

Для получения более детальной справки по командам-ключам пользуйтесь данной конструкцией:

```
$ python client.py ... <command> --help
```

## Команды клиента:

+ `get` - скачивание файла (папки) с сервера
+ `put` - загрузка файла (папки) на сервер
+ `user` - вход с помощью логина и пароля
+ `pwd` - вывод текущей директории
+ `rm` - удаление папок/файлов
+ `ren` - переименование папок/файлов
+ `cd` - смена директории
+ `mkdir` - создание директории
+ `ls` - вывод содержимого директории
+ `size` - размер файла
+ `debug` - debug режим. Выводит на консоль отправляемые серверу команды
+ `mode` - переключение режима работы
+ `help` - получение справки
+ `exit` - завершение работы

Для получения более детальной справки по командам пользуйтесь данной конструкцией: `help <command>`
