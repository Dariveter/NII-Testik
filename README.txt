WHOISWHO v4

ВАЖНО:
1. Загрузите ВСЁ содержимое этой папки в корень репозитория Dariveter/NII.
2. В GitHub Pages: Settings → Pages → Deploy from a branch → main → /(root).
3. Тест в Tilda вставлять iframe:
   <iframe
     src="https://dariveter.github.io/NII/"
     style="width:100%;height:100vh;border:0;display:block"
     allow="web-share; clipboard-write"
   ></iframe>

Главная кнопка шаринга:
— на поддерживаемом мобильном браузере вызывает Web Share API;
— передаёт чистую картинку результата + текст + https://ne-institute.com/whoiswho;
— если Web Share недоступен, открывает меню fallback-вариантов.

Telegram / Facebook / VK:
— используют result-specific страницы /share/<result>/;
— соцсеть получает чистую OG-картинку результата;
— при клике пользователь переходит на https://ne-institute.com/whoiswho.

Instagram:
— сайт копирует ссылку;
— затем отправляет чистую картинку через системный share sheet;
— если это невозможно, скачивает картинку.

Картинки в этой версии — именно пять файлов, загруженных пользователем в текущем чате.
