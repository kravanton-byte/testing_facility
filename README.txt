Медиакот 2027: новогоднее поздравление и игра UM · MediaFuturism
Адрес: https://hny2027.mediafuturism.ru/

ЧТО В ПАПКЕ
  index.html                      страница целиком: поздравление, игра (HTML, CSS, JavaScript, Canvas)
  assets/um-logo.webp             логотип UM в красном круге
  assets/mediafuturism-logo.webp  логотип MediaFuturism
  assets/fonts/*.woff2            шрифты Rubik и Unbounded (лицензия SIL Open Font License, тексты лицензий рядом)
  README.txt                      этот файл

ЧЕМ СОБРАНО
  Без фреймворков и без сборщика. Это готовая папка: её можно скопировать на хостинг как есть.
  Все пути относительные. Внешних запросов нет: шрифты и картинки лежат в папке.
  Сервер не нужен. Аналитики, форм, cookies и Service Worker нет.
  В localStorage браузера хранятся только личный рекорд (mk_best) и выбранный котик (mk_cat).
  Favicon не добавлен, его подключаете вы.

КАК ПРОВЕРИТЬ ЛОКАЛЬНО
  В этой папке выполнить:  python3 -m http.server 8000
  и открыть http://localhost:8000

ИСХОДНИКИ
  Архив hny2027-sources.zip: index.html (общий исходник для сайта и для тестовой версии в Claude),
  assets/ и tools/build_site.py. Сборщик убирает тестовую таблицу лидеров и подключает локальные шрифты:
    python tools/build_site.py <папка для результата>
  Нужен только Python 3, без дополнительных пакетов.

ГРАФИКА
  Котики, ёлка, медиаслоты и бонусы рисуются кодом на Canvas, отдельных файлов картинок для них нет.
