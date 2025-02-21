Чтение для понимания как запустить тесты и что они делают.

Этот туду-лист был написан на PHP и HTML (ну и немного джаваскрипта).  Он имеет простой функционал: можно добавлять задачи, смотреть список, отмечать выполненными, удалять и редактировать.

Что тестируется:

Тесты проверяют основные функции этого туду-листа. А именно:

1. **addTask:**  Проверяет, что задачи добавляются в список и пустые задачи не добавляются.
2. **listTasks:**  Проверяет, что список задач возвращается правильно и он изначально пустой.
3. **completeTask:** Проверяет, что задачи можно отметить как выполненные и что неверные индексы обрабатываются правильно.
4. **deleteTask:** Проверяет удаление задач по индексу и обработку неверных индексов.
5. **editTask:**  Проверяет редактирование задач и что нельзя установить пустой текст, а так же неверные индексы.
6. **countCompletedTasks:** Проверяет подсчет выполненных задач.

Как запустить тесты:

1. Убедитесь, что у вас установлен PHPUnit. Если нет, то запустите `composer require phpunit/phpunit --dev` в терминале в папке с туду-листом.
2. Откройте терминал в корневой папке проекта (там где `index.html`, `todo.php` и папка `tests`).
3. Запустите команду:  `./vendor/bin/phpunit tests/TodoTest.php` (или `vendor/bin/phpunit tests/TodoTest.php` для винды).
4. Посмотрите, чтобы все тесты прошли "ОК" (зелененьким таким). Если что-то "FAIL", значит где-то ошибка в коде или тесте.

Вроде все. 