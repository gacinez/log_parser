# log_parser
Скрпит предназначен для парсинга файлов с раширением log, информацию которую он собирает и пердостаовляет в формате json:
- общее количество выполненных запросов
- количество запросов по типу: GET - 20, POST - 10 и т.п.
- топ 10 IP адресов, с которых были сделаны запросы
- топ 10 запросов, которые завершились клиентской ошибкой, должно быть видно метод, url, статус код, ip адрес
- топ 10 запросов, которые завершились ошибкой со стороны сервера, должно быть видно метод, url, статус код, ip адрес

Два возможных способа запуска скрипта:

1). Запуск с указание параметра пути, в таком случае в директории и вложенных директориях будут отпарсены все файлы с расширением log log_parser.py --path C:\Dev\log_parser\logs


2). Запуск с указанием непосредственно пути к файлу log_parser.py --file c:\Dev\log_parser\logs\new\1.log
