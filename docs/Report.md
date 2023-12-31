# Отчётные документы по итогам тестирования
## Краткое описание
Согласно [плану](Plan.md) было проведено автоматизированное тестирование веб-сервиса предлагающего купить тур.
+ В ходе тестирования были реализованы позитивные и негативные сценарии покупки тура, а также API сценарии с проверкой результатов выполнения операции в базе данных
+ Проверенна заявленная поддержка двух СУБД
    + MySQL;
    + PostgreSQL.

## Тест-кейсы

Общее колличество тест-кейсов:
+ Оплата через вкладку "Купить" - 45 (3 позитивных, 42 негативный)
+ Оплата через вкладку "Купить в кредит" - 45 (3 позитивных, 42 негативный)

## Общие рекомендации
По результатам тестирования необходимо:
+ Исправить найденные дефекты
1. [Не верное название вкладки](https://github.com/AnnaBorzenkowa/Diplom/issues/2)
2. [При вводе не верных данных владельца карты в полях "Купить в кредит" статус "Успешно"](https://github.com/AnnaBorzenkowa/Diplom/issues/4)
3. [При вводе не верных данных владельца карты в полях "Купить" статус "Успешно"](https://github.com/AnnaBorzenkowa/Diplom/issues/6)
4. [Неверные сообщения об ошибке, при отправки формы с пустыми полями во вкладках "Купить" и "Купить в кредит"](https://github.com/AnnaBorzenkowa/Diplom/issues/7)
5. [Сообщение об ошибке "Не верный формат", не исчезает при повторной отправке валидных данных во вкладках "Купить" и "Купить в кредит"](https://github.com/AnnaBorzenkowa/Diplom/issues/8)
6. [При вводе не валидных данных в поле "Месяц" операция завершается успешно](https://github.com/AnnaBorzenkowa/Diplom/issues/9)
7. [Проходит оплата по невалидной карте, во вкладках "Купить" и "Купить в кредит"](https://github.com/AnnaBorzenkowa/Diplom/issues/3)
8. [При вводе не валидных данных в поле CVC/CVV, статус операции Успешно](https://github.com/AnnaBorzenkowa/Diplom/issues/1)