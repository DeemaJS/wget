# wget

*** Тренируйтесь сперва на простых интернет-ресурсах.

 -r Ходим по ссылкам (рекурсивное скачивание)
 
-k Преобразовываем ссылки к локальному виду

-p Указывает на то, что нужно загрузить все файлы, которые требуются для отображения страниц (изображения, css и т.д.).

-l (level) позволяет указать насколько «глубоко» программа должна следовать по ссылкам; 0 — бесконечно глубоко, по умолчанию установлено 5

-nc При использовании этого параметра существующие файлы не будут перезаписаны. Это удобно, когда нужно продолжить загрузку сайта, прерванную в предыдущий раз

-np Не подниматься выше начального адреса при рекурсивной загрузке
—m Зеркалирование сайта. Удобно при обновлении ранее скачанного сайта. Вытаскивает только изменившиеся файлы
-i Загрузить URL-ы согласно локальному или внешнему файлу
-c Режим докачки. Указывает wget продолжать закачку файла. Если файл в текущей директории уже есть, на сервер будет отправлен запрос на продолжение закачки
-E Добавлять к загруженным файлам расширение .html
-P C:\Site Назначаем путь к файлам
—user-agent=»Mozilla/5.0″ Также, в ряде подобных (и не только) случаев, бывает весьма полезна опция представления wget — «User Agent». Некоторые серверы выдают требуемую информацию только для обозревателей, идентифицирующихся как «Mozilla» или Microsoft «Internet Explorer». Этот параметр позволяет обмануть такие серверы. —user-agent=»Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US; rv:1.8.1.6) Gecko/20070725 Firefox/2.0.0.6″ на всякий случай попросим wget прикинуться виндовым firefox’ом
—limit-rate=50k -w 3 Чтобы не создавать излишнюю нагрузку на сайт
-A.mp3 (скачать только mp3 файлы) Для этого применяется опция -A. После этой опции указывается список разрешенных для скачивания имен (точнее шаблонов имен файлов). Используется следующим образом:
-A ‘.jpg,.jpeg’ (скачать файлы с расширением jpg и jpeg)
-e robots=off Wget при рекуррентном скачивании учитывает Протокол Web-роботов, и пропускает часть файлов, запрещенных в файле robots.txt . Чтобы отключить эту функцию используется ключ «-e robots=off».
