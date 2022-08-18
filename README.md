# Stress Testing local API
 
Нагружаем локальное API. Порядок действий для быстрой установки.
0. Скачиваем исходный код.
1. Устанавливаем менеджер пакетов NodeJS https://nodejs.org/en/download/ 
1. В папке где будет лежать наше api выполнить:
npm init -y
В результате получаем package.json
2. В этой же папке устанавливаем json-server:
npm install json-server
3. В package.json (созданный в первом пункте) добавляем скрипт для старта json-сервера:
"scripts":{
    "start": "json-server users.json"
  }
4. Сохраняем и запускаем в терминале:
npm start
5. Заходим на http://localhost:3000

В папке Report находится отчёт в формате docx(MS Office) с анализом нагрузочного тестирования.
В папке Jmeter Config - конфигурация Jmeter.
В папке apache-jmeter-5.5 - находится утилита для нагрузочного тестирования JMeter.
Так же файл базы данных users.json лежит в корне проекта.
