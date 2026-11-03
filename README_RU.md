# Delete Nearest Marker to Cursor

[English](README.md) · **Русский**

Удаляет ближайший к курсору редактирования маркер, определяя расстояние по временной шкале. Регионы игнорируются.

## Работа скрипта

- Перебирает все маркеры проекта и вычисляет абсолютное расстояние до курсора.
- Удаляет ближайший маркер независимо от его положения слева или справа.
- Записывает удаление в историю отмены REAPER.
- Если в проекте нет маркеров, ничего не изменяет.

## Установка

### Через ReaPack

Добавьте [каталог Patch34 ReaPack](https://raw.githubusercontent.com/patch-34/patch34-reapack/main/index.xml) через **Extensions → ReaPack → Import repositories…**. В **Extensions → ReaPack → Browse packages** найдите пакет **Delete Nearest Marker to Cursor**, установите его и синхронизируйте пакеты.

### Вручную

1. Скопируйте `Delete_Nearest_Marker_To_Cursor.lua` в каталог `Scripts` ресурсов REAPER (см. **Options → Show REAPER resource path**).
2. Откройте **Actions → Show action list → New action → Load ReaScript** и выберите Lua-файл.
3. Запустите действие или назначьте сочетание клавиш.

При ручном обновлении заменяйте файл по прежнему пути. При изменении имени файла действие может потребоваться зарегистрировать заново.

## Лицензия и авторство

Распространяется по [лицензии MIT](LICENSE).

Автор: [Aleksei Vorobev / Patch34](https://github.com/patch-34).
