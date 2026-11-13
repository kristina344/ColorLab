# Публикация ColorLab на GitHub Pages

1. В пустом репозитории `kristina344/ColorLab` выберите **uploading an existing file**.
2. Перетащите всё содержимое этой папки в загрузчик GitHub с сохранением структуры: `photo_app.py`, `.github/workflows/pages.yml`, `public/data/...`, `public/assets/...`, `colorlab.css` и остальные файлы должны лежать в КОРНЕ репозитория, без дополнительной папки `ColorLab`.
3. При коммите выберите основную ветку `main`.
4. Откройте `Settings > Pages > Build and deployment > Source` и выберите **GitHub Actions**.
5. Откройте `Actions`, дождитесь завершения задания `Publish ColorLab to GitHub Pages` и проверьте ссылку из `Settings > Pages`.
6. Проверьте страницу в отдельном браузере и все интерактивные элементы. Запуск в WebAssembly пока НЕ проверен: возможны ограничения пакетов или файловых путей. При ошибке скопируйте лог Actions или сообщение браузера.

Браузерная версия лежит в `photo_app.py` и читает файлы из `public` через `mo.notebook_location()`. Для локального запуска исходный файл сохранён как `photo_app_local.py` (он ожидает папки `data` и `assets`).

В архиве также сохранён оригинальный ноутбук, а ссылка на Colab уже заменена на публичную ссылку пользователя.
