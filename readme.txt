Гайдлайн НаПоправку — отдельный сайт

Как выложить:
1. app.netlify.com → Add new site → Deploy manually
2. перетащить эту папку целиком (не содержимое, а папку)
3. Site configuration → Change site name → napopravku-guide
   Адрес: https://napopravku-guide.netlify.app

Как обновлять: заменить index.html и перезалить папку.

Что внутри:
  index.html      страница целиком: разметка, стили и скрипт
  css/style.css   стили Webflow, на которых держится вёрстка блоков логотипа
  images/         картинки шапок, логотипы, фото для примеров
  documents/      пакет презентаций для скачивания
  _headers        разрешение CORS, нужно для шрифтов и файлов
