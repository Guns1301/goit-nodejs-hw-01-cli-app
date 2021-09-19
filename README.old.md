# goit-nodejs-hw-01-cli-app

Шаг 1
Инициализируй npm в проекте npm init -y
В корне проекта создай файл index.js
Поставь пакет nodemon как зависимость разработки (devDependencies) - npm i nodemon -D
В файле package.json добавь "скрипты" для запуска index.js
Скрипт start который запускает index.js с помощью node
Скрипт start:dev который запускает index.js с помощью nodemon

"start": "node index.js",
"start:dev": "nodemon index.js",

Шаг 2
В корне проекта создай папку db. Для хранения контактов скачай и используй файл contacts.json, положив его в папку db.

В корне проекта создай файл contacts.js.

Сделай импорт модулей fs и path для работы с файловой системой
Создай переменную contactsPath и запиши в нее путь к файлу contacts.json.
Для составления пути ипользуй методы модуля path.
Добавь функции для работы с коллекцией контактов. В функциях используй модуль fs и его методы readFile() и writeFile()
Сделай экспорт созданных функций через module.exports

Шаг 3
Сделай импорт модуля contacts.js в файле index.js и проверь работоспособность функций для работы с контактами.

Шаг 4
В файле index.js импортируется пакет commander для парсинга аргументов командной строки.

npm i commander

Шаг 5
Запусти команды в терминале и сделай отдельный скриншот результата выполнения каждой команды.

# Получаем и выводим весь список контактов в виде таблицы (console.table)

node index.js --action list

# Получаем контакт по id

node index.js --action get --id 5

# Добавялем контакт

node index.js --action add --name Mango --email mango@gmail.com --phone 322-22-22

# Удаляем контакт

node index.js --action remove --id=3
