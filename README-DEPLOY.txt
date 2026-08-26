WHOISWHO v6 — STATIC SOCIAL SHARE

ЭТА СБОРКА СДЕЛАНА СТРОГО ПО СХЕМЕ С ОТДЕЛЬНЫМИ SHARE-СТРАНИЦАМИ.

ВАЖНО: ZIP НЕЛЬЗЯ ПРОСТО ЗАГРУЗИТЬ В GITHUB КАК ZIP.
Его нужно РАСПАКОВАТЬ и загрузить содержимое в КОРЕНЬ репозитория.

После загрузки в репозитории ОБЯЗАТЕЛЬНО должна быть структура:

index.html
share-check.html
assets/
  alice-og.jpg
  alice-portrait.webp
  alice-share.jpg
  chatgpt-og.jpg
  ...
share/
  alice/index.html
  chatgpt/index.html
  gemini/index.html
  claude/index.html
  grok/index.html

ПРОВЕРКА:
https://dariveter.github.io/NII/share-check.html

Должны открываться:
https://dariveter.github.io/NII/share/alice/?v=6
https://dariveter.github.io/NII/share/chatgpt/?v=6
https://dariveter.github.io/NII/share/gemini/?v=6
https://dariveter.github.io/NII/share/claude/?v=6
https://dariveter.github.io/NII/share/grok/?v=6

Каждая share-страница содержит СТАТИЧЕСКИЕ OG-теги и абсолютный URL картинки.
Социальный бот читает OG. Обычный пользователь выполняет JS и попадает на:
https://ne-institute.com/whoiswho

Кэш:
Share-кнопки используют ?v=6, чтобы соцсети воспринимали URL как новый.
Если в будущем меняются картинки или OG-тексты, увеличить SHARE_VERSION.
