# Оглавления
<!--ts-->
* [Оглавления](#оглавления)
* [Описание](#описание)
* [Вопросы](#вопросы)
   * [Вопросы на собеседовании по Node.JS базового уровня](#вопросы-на-собеседовании-по-nodejs-базового-уровня)
   * [Вопросы для собеседования по Node JS продвинутого уровня](#вопросы-для-собеседования-по-node-js-продвинутого-уровня)
* [Задачи](#задачи)
   * [Node.js](#nodejs)
      * [Лёгкий:](#лёгкий)
         * [1. Node.js (Асинхронная работа с файлами):](#1-nodejs-асинхронная-работа-с-файлами)
         * [2. Node.js (Асинхронная работа с файлами):](#2-nodejs-асинхронная-работа-с-файлами)
         * [3. Node.js (Работа с объектами):](#3-nodejs-работа-с-объектами)
         * [4. Node.js (Чтение и запись файлов):](#4-nodejs-чтение-и-запись-файлов)
         * [5. Node.js (Удаление дубликатов из массива):](#5-nodejs-удаление-дубликатов-из-массива)
      * [Средний:](#средний)
         * [1. Node.js (Асинхронная обработка нескольких API-запросов)](#1-nodejs-асинхронная-обработка-нескольких-api-запросов)
         * [2. Node.js (Работа с массивами и объектами):](#2-nodejs-работа-с-массивами-и-объектами)
         * [3. Node.js (Банкомат):](#3-nodejs-банкомат)
      * [Сложный:](#сложный)
         * [1. Node.js (Асинхронность и управление потоками данных):](#1-nodejs-асинхронность-и-управление-потоками-данных)
         * [2. Node.js (Модификация строк и объектов):](#2-nodejs-модификация-строк-и-объектов)
   * [SQL](#sql)
      * [Лёгкий:](#лёгкий-1)
         * [1. SQL (Простая выборка):](#1-sql-простая-выборка)
         * [2. SQL (Выборка с сортировкой):](#2-sql-выборка-с-сортировкой)
      * [Средний:](#средний-1)
         * [1. SQL (Объединение таблиц):](#1-sql-объединение-таблиц)
         * [2. SQL (Агрегация данных):](#2-sql-агрегация-данных)
      * [Сложный:](#сложный-1)
         * [1. SQL (Сложные агрегации):](#1-sql-сложные-агрегации)
         * [2. SQL (Подсчёт уникальных записей и фильтрация):](#2-sql-подсчёт-уникальных-записей-и-фильтрация)

<!-- Created by https://github.com/ekalinin/github-markdown-toc -->
<!-- Added by: runner, at: Wed Nov 27 10:14:46 UTC 2024 -->

<!--te-->
# Описание
В данном файле есть вопросы кондидату и задачи по Node.js и SQL.
Задачи в первую очереь расчитаны на Junior Node.js разработчиков.
Все задачки разбиты на 3 уровня сложности: (лёгкий, средний и сложный)

# Вопросы

## Вопросы на собеседовании по Node.JS базового уровня
1. *Как работает Node JS?* <br>
Node JS работает с однопоточным циклом событий и неблокирующим вводом-выводом, оба из которых обеспечивают высокую скорость, поскольку они могут обрабатывать больше одновременных запросов. Node JS также может работать на любом автономном веб-сервере, используя модуль «HTTP».

2. *Почему Node JS однопоточный?*<br>
Чтобы разрешить асинхронную обработку, Node JS использует однопоточную парадигму. Приложение может работать более эффективно и лучше масштабироваться при использовании асинхронной обработки. Таким образом, в отличие от обычной реализации на основе потоков, Node JS использует подход однопоточной модели.

3. *Объясните асинхронность и неблокировку*<br>
Асинхронный: Асинхронный означает отсутствие синхронности. Эта функция позволяет нам отправлять асинхронные HTTP-запросы, которые не ждут ответа от сервера. Эти операции отвечают на запрос, на который уже получен ответ сервера.
Неблокирующие функции: операции ввода-вывода обрабатываются с помощью неблокирующих функций. Они сразу же отвечают любыми доступными данными и продолжают функционировать в соответствии с требованиями. Если ответ получить не удалось, API сразу возвращает ошибку.

4. *Что такое REPL?*<br>
Read, Eval, Print и Loop называются REPL в Node JS. REPL представляет собой компьютерную среду, в которой можно ввести любую команду, а машина может ответить выводом, например оконной консолью или оболочкой Unix/Linux. Среда REPL по умолчанию предустановлена с Node JS. Следующие задачи могут быть выполнены с помощью REPL: <br><br>
Чтение: считывает ввод пользователя, анализирует ввод в структуру данных JavaScript и сохраняет его в памяти.
Eval: получает и оценивает структуру данных.
Print: распечатывает окончательный результат.
Loop: повторяет указанную команду до тех пор, пока не будет дважды нажата клавиша CTRL+C.
Укажите шаги, с помощью которых «Поток управления» управляет вызовами функций в Node JS? <br><br>
Вот шаги:
- Контролировать порядок выполнения
- Собирать данные
- Ограничение параллелизма
- Вызов следующего шага в программе

5. *Что такое LTS-релизы Node JS?*<br>
Версия Node JS LTS, что означает долгосрочную поддержку Node JS, получает все необходимые обновления безопасности, обновления производительности и исправления ошибок. Эти версии, в которых приоритет отдается стабильности и безопасности, поддерживаются не менее 18 месяцев. В LTS-версиях вносятся только исправления ошибок, обновления безопасности, обновления npm и документации, улучшения производительности и другие изменения.

6. *Объясните промежуточное ПО в Node JS?*<br>
Промежуточное ПО — это функция, которая принимает объекты Request и Response. Эти функции имеют доступ к нескольким объектам запроса и ответа, а также к последующей функции цикла во время цикла запрос-ответ приложения. Следующая функция промежуточного программного обеспечения выражается с помощью переменной, которая называется «следующий». Наиболее часто выполняемые функции промежуточного программного обеспечения:

- Выполнение любого типа кода
- Обновите запрос и объекты ответа
- Завершить цикл запрос-ответ
- Вызвать следующее промежуточное ПО в стеке

7. *Что такое ESLint?*<br>
ESLint — это проект с открытым исходным кодом, созданный Николасом С. Закасом в 2013 году с целью предложить инструмент проверки JavaScript через подключаемый модуль. Линтеры — это полезные инструменты для поиска определенных классов ошибок в Node JS, особенно тех, которые связаны с областью видимости переменных.

8. *Почему Google использует движок V8 для Node JS?*<br>
V8 — это движок выполнения Chrome, который переводит код JavaScript в собственный машинный код, и Google использует его.

9. *Объясните заглушку в Node JS.*<br>
Заглушки — это, по сути, приложения или методы, используемые в Node JS для стимулирования действий модуля или компонента. Заглушки предлагают предварительно запрограммированные ответы для функций во время любых тестовых сценариев.

10. *Объясните класс буфера в Node JS?*<br>
В Node JS класс буфера хранит необработанные данные способом, сравнимым с массивом целых чисел. Однако это относится к необработанному выделению памяти за пределами кучи V8. Без импорта модуля буфера приложение может использовать этот глобальный класс, к которому легко получить доступ.

## Вопросы для собеседования по Node JS продвинутого уровня

1. *Каковы атрибуты package.json?*<br>
Имя, версия, сводка, домашняя страница, автор, участники, список зависимостей, тип репозитория и URL-адрес, основная точка входа пакета и ключевые слова.

2. *Что такое обратный вызов с ошибкой в Node JS?*<br>
Мы должны подтвердить, что код был выполнен без ошибок, если мы хотим убедиться, что он работает правильно. В этой ситуации используются обратные вызовы Error-First, которые сначала передают ошибку, а затем любые соответствующие данные после этого.

3. *Что такое npm?*<br>
npm расшифровывается как Node Package Manager. Вот две основные функции npm:
Онлайн-репозитории для пакетов/модулей Node JS, которые доступны для поиска на search.Nodejs.org.
Управление версиями, утилита командной строки для установки пакетов и управление зависимостями пакетов Node JS.

4. *Какая польза от модуля crypto в Node JS?*<br>
Чтобы предложить пользователям криптографические функции, Node JS использует модуль crypto. Эта функция предоставляет пользователям доступ к широкому спектру оболочек для выполнения различных операций, включая шифрование, расшифровку, подпись и хеширование.

5. *Что такое паспорт в Node JS?*<br>
Node JS включает в себя часто используемое ПО промежуточного слоя Passport. Он может быть встроен в любое веб-приложение на основе Express.js и обычно используется для аутентификации.

6. *Как работает функция поиска DNS в Node JS?*<br>
Запись IPv4 или IPv6 возвращается методом поиска DNS с использованием веб-адреса в качестве входных данных.<br><br>
Дополнительные параметры, такие как выбор, определяют, является ли ввод объектом или целым числом. Учитываются как IPv4, так и IPv6, если здесь ничего не указано. Третий параметр функции обратного вызова предназначен для этой функции.<br><br>
Вот пример синтаксиса:
dns.lookup(адрес, параметры, обратный вызов)

7. *Что такое module.exports в Node JS?*<br>
Две функции становятся доступными и помещаются в практический контекст с помощью функции «module.exports». Объект, используемый для хранения относительного кода в одном фрагменте, называется модулем. Вы можете думать об этом как об операции по объединению всех функций в один файл.



# Задачи


## Node.js


### Лёгкий:

#### 1. Node.js (Асинхронная работа с файлами):
Напишите функцию, которая читает данные из файла и возвращает количество строк в файле. Используйте асинхронные функции `fs.promises`.
```node.js
const fs = require('fs').promises;

async function countLines(filePath) {
    // Ваш код
}

countLines('file.txt').then(console.log);
```

#### 2. Node.js (Асинхронная работа с файлами):
Напишите асинхронную функцию, которая получает список всех файлов и папок в текущей директории и возвращает их имена. Используйте `fs.promises` для работы с файловой системой.
```node.js
const fs = require('fs').promises;

async function getFilesInDirectory(dirPath) {
    // Ваш код
}

getFilesInDirectory('.').then(files => console.log(files)).catch(console.error);
```

#### 3. Node.js (Работа с объектами): 
Напишите функцию, которая принимает объект с данными о человеке (имя, возраст, пол) и возвращает строку с форматированным выводом этих данных.
```node.js
function formatPerson(person) {
    // Ваш код
}

const person = { name: "Иван", age: 25, gender: "мужчина" };
console.log(formatPerson(person)); // Пример вывода: "Иван, 25 лет, мужчина"
```

#### 4. Node.js (Чтение и запись файлов):
Тебе нужно прочитать данные из файла file1.txt, после прочтения полученные данные надо записать в файл file2.txt. Реализовать это надо 3 разными способами, для каждого способа своя функция: 
- readAndWriteCallbackHell() - в данной функции ты должен использовать только передачу коллбека в ассинхронную функцию. 
- readAndWritePromises() - в данной функции ты должен использовать промисы и then. 
- readAndWriteAsyncAwait() - в данной функции можно использовать async await.
```node.js
const fs = require("fs");

const readAndWriteCallbackHell = () => {};

const readAndWritePromises = () => {};

const readAndWriteAsyncAwait = async () => {};
```

#### 5. Node.js (Удаление дубликатов из массива):
Вам нужно написать функцию, которая принимает в качестве аргумента массив чисел и удаляет все повторяющиеся значения.
Напишите функцию двумя разными спомобами:
1. Используя два цикла, без использования стандартных функций JS.
2. Используя любые средства JS
```node.js
function removeRepsOne(array) {}

function removeRepsTwo(array) {}

console.log(removeRepsOne([1, 1, 2, 4, 5, 6, 6, 8, 9, 11])); // [1,2,4,5,6,8,9,11]
console.log(removeRepsTwo([1, 1, 2, 4, 5, 6, 6, 8, 9, 11])); // [1,2,4,5,6,8,9,11]
```


### Средний:

#### 1. Node.js (Асинхронная обработка нескольких API-запросов)
Напишите функцию, которая принимает массив URL-ов и делает параллельные HTTP-запросы к каждому URL, используя `axios`. Возвращайте массив результатов запросов, но если один из запросов завершился неудачей, продолжайте выполнение остальных.
```node.js
const axios = require('axios');

async function fetchAll(urls) {
    // Ваш код
}

const urls = ['https://api1.com', 'https://api2.com'];
fetchAll(urls).then(console.log);
```

#### 2. Node.js (Работа с массивами и объектами): 
Напишите функцию, которая принимает массив объектов (товары с полями `name` и `price`) и возвращает новый массив, где каждому товару добавлено новое поле `discountedPrice` с ценой, уменьшенной на 10%.
```node.js
function applyDiscount(products) {
    // Ваш код
}

const products = [
    { name: "Товар 1", price: 100 },
    { name: "Товар 2", price: 200 }
];
console.log(applyDiscount(products));

```

#### 3. Node.js (Банкомат): 
Создайте функцию, которая имитирует базовое функционирование банкомата. Функция должна принимать сумму и возвращать объект с распределением купюр в формате: {номинал_купюры: количество_купюр}.<br>
Требования к функции:
- Если запрошенная сумма не может быть выдана банкоматом, функция должна возвращать ошибку 'Недопустимая сумма'.
- Размен денег должен производиться максимально рационально (например, вместо пяти купюр по 1000, должна выдаваться одна купюра номиналом 5000).
- За одну операцию банкомат может выдать не более 20 купюр, в противном случае выводится сообщение об ошибке 'Превышен лимит купюр'.

```node.js
function cashMachine(amount) {
  const denominations = [5000, 2000, 1000, 500, 200, 100, 50];
}

cashMachine(8350); // {5000: 1, 2000: 1, 1000: 1, 200: 1, 100: 1, 50: 1}
cashMachine(2570); // Недопустимая сумма
cashMachine(100050); // Превышен лимит купюр
```



### Сложный:

#### 1. Node.js (Асинхронность и управление потоками данных):
Реализуйте простую очередь задач с использованием событийного механизма. Создайте функцию, которая добавляет задачи в очередь, а затем по очереди их обрабатывает с использованием `setTimeout`. Очередь должна поддерживать асинхронные задачи и параллельное выполнение не более 2 задач одновременно.
```node.js
const EventEmitter = require('events');

class TaskQueue extends EventEmitter {
    constructor() {
        super();
        // Ваш код
    }

    addTask(task) {
        // Ваш код
    }
}

// Пример использования
const queue = new TaskQueue();
queue.addTask(() => /* Ваша задача */);
```

#### 2. Node.js (Модификация строк и объектов):
Напишите функцию, которая принимает строку с JSON и удаляет все ключи, значения которых являются пустыми строками, `null`, `undefined` или `NaN`. Верните модифицированный объект.
```node.js
function cleanObject(jsonStr) {
    // Ваш код
}

const jsonStr = '{"name":"Иван", "age": null, "email":"", "phone": "12345"}';
console.log(cleanObject(jsonStr)); // Пример вывода: { name: 'Иван', phone: '12345' }
```

#### 3. Node.js (Регулярные выражения - "Проверка формата строки и извлечение данных"):
Тебе нужно написать функцию на JavaScript, которая принимает строку и проверяет, соответствует ли она определенному формату. Если строка соответствует формату, функция должна вернуть объект с извлеченными данными, иначе — null.

```node.js
function parseTransaction(str) {
    // Ваш код
}

const str = "Дата: 2024-05-15 Заказ: order-12345 Сумма: 1500 рублей Примечание: Оплата за услуги"
console.log(parseTransaction(str));
/*
Пример вывода:
{
  date: '2024-05-15',
  order: 'order-12345',
  amount: 1500,
  note: 'Оплата за услуги'
}
*/ 
```






## SQL

### Лёгкий: 

#### 1. SQL (Простая выборка):
У вас есть таблица пользователей `users` с полями `id`, `name`, и `age`. Напишите SQL-запрос, который возвращает всех пользователей старше 18 лет.

*Решение:*
```SQL
SELECT * FROM users WHERE age > 18;
```

#### 2. SQL (Выборка с сортировкой): 
У вас есть таблица товаров `products` с полями `id`, `name`, `price`. Напишите SQL-запрос, который возвращает все товары, отсортированные по цене по возрастанию.

*Решение:*
```SQL
SELECT * FROM products ORDER BY price ASC;
```







### Средний:

#### 1. SQL (Объединение таблиц): 
У вас есть две таблицы: `users` (поля `id`, `name`, `age`) и `orders` (поля `id`, `user_id`, `amount`). Напишите SQL-запрос, который возвращает имена пользователей и общую сумму их заказов.

*Решение:* 
```SQL
SELECT users.name, SUM(orders.amount) 
FROM users 
JOIN orders ON users.id = orders.user_id 
GROUP BY users.name;
```

#### 2. SQL (Агрегация данных): 
У вас есть таблица `orders` с полями `id`, `user_id`, `amount`. Напишите запрос, который возвращает общее количество заказов и среднюю сумму заказа.

*Решение:* 
```SQL
SELECT COUNT(*) AS total_orders, AVG(amount) AS avg_amount FROM orders;
```






### Сложный:

#### 1. SQL (Сложные агрегации): 
У вас есть таблица `transactions` (поля `id`, `user_id`, `amount`, `status`, где `status` может быть 'success' или 'failed'). Напишите запрос, который возвращает каждого пользователя с количеством успешных и неуспешных транзакций.

*Решение:*
```SQL
SELECT user_id, 
       SUM(CASE WHEN status = 'success' THEN 1 ELSE 0 END) AS successful_transactions, 
       SUM(CASE WHEN status = 'failed' THEN 1 ELSE 0 END) AS failed_transactions 
FROM transactions 
GROUP BY user_id;
```


#### 2. SQL (Подсчёт уникальных записей и фильтрация): 
У вас есть таблица пользователей `users` с полями `id`, `name`, `email`, `created_at`. Напишите запрос, который возвращает количество уникальных email-адресов, зарегистрированных за последний месяц.

*Решение:*
```SQL
SELECT COUNT(DISTINCT email) 
FROM users 
WHERE created_at >= DATE_SUB(CURDATE(), INTERVAL 1 MONTH);
```
