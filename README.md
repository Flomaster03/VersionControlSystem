Описание
Система контроля версий — это программное обеспечение, которое может отслеживать изменения, внесенные в программу. Существует несколько популярных систем контроля версий (например, Git, SVN или Mercurial). У каждого из них есть свои плюсы и минусы. Их объединяет одна общая идея. Система контроля версий запоминает, кто изменил файл, когда это было сделано и почему . Это также позволяет вам вернуться к предыдущим версиям.

В этом проекте вам необходимо реализовать простую систему контроля версий. Это будет ваш собственный Git. Кстати, если вы хотите научиться работать с Git, загляните в Git How To .

Взгляните на команды, которые вам нужно будет реализовать в этом проекте:

configустанавливает или выводит имя автора коммита;
--helpраспечатывает страницу справки;
addдобавляет файл в список отслеживаемых файлов или выводит этот список;
logпоказывает все коммиты;
commitсохраняет изменения файла и имя автора;
checkoutпозволяет переключаться между коммитами и восстанавливать предыдущее состояние файла.
На этом этапе ваша программа должна иметь возможность принимать один аргумент и, в зависимости от аргумента, печатать справочную информацию.

Цели
На этом этапе ваша программа должна:

Возьмите один аргумент как команду.
Если аргумент отсутствует или есть --help, распечатайте всю страницу справки.
Если команда существует, программа должна вывести описание команды.
Если команда неверна, выведите'[passed argument]' is not a SVCS command.
В отличие от многих других проектов, программа не работает в бесконечном цикле. Программа начинается с аргументов, которые передаются в основную функцию и должны что-то сделать, затем снова начинается с нуля с другими аргументами и должна делать что-то еще.
Примеры
Символ «больше», за которым следует пробел ( > ), представляет ввод пользователя. Обратите внимание, что это не часть ввода. Система проверки игнорирует все пробелы, но мы предлагаем попытаться создать хороший результат.

Пример 1 : аргумент--help

These are SVCS commands:
config     Get and set a username.
add        Add a file to the index.
log        Show commit logs.
commit     Save changes.
checkout   Restore a file.
Пример 2 : нет аргументов

These are SVCS commands:
config     Get and set a username.
add        Add a file to the index.
log        Show commit logs.
commit     Save changes.
checkout   Restore a file.
Пример 3 : аргументconfig

Get and set a username.
Пример 4 : аргументwrong

'wrong' is not a SVCS command.

