Познакомимся с событиями!
У тебя есть файл input.txt примерно следующего содержания:
2 2 +
4 2 /
1234.12 4564 -
3 4 *
16 5 %
345 789 +

Два любых чила и операция (+, -, *, /, % - остаток от деления).

Создай класc Calculator, который имеет соответсвующие методы по сложению, вычитанию, и т.д. Каждый метод принимает только два аргумента.
При этом тебе нужно считать содержимое данного input.txt файла, чтобы после прочтения кажой из строк срабатывала нужная операция класса Calculator.
Напиши тесты на то, чтобы проверить, что каждый из методов класса Calculator был вызван ожидаемое количество раз (тестовый фреймворк - по желанию). sinon (https://www.npmjs.com/package/ts-sinon) тебе в помощь.

При чтении каждой строки не просто должен вызываться метод, должно срабатывать событие ('sum', 'divide', или как бы ты их не назвала😉), а уже это событие, когда оно имитировано, должно тригерить вызов метода. Здесь тебе EventEmitter в помощь:
https://nodejs.dev/en/learn/the-nodejs-event-emitter/

Для считывания содержимого файла используй вот такой подход:
https://geshan.com.np/blog/2021/10/nodejs-read-file-line-by-line/#readline