# Delete Nearest Marker to Cursor

[English](README.md) · **Русский**

Удаляет маркер, ближайший к курсору редактирования по абсолютному расстоянию на временной шкале. Регионы игнорируются — учитываются только маркеры.

## Установка

### Через ReaPack

Добавьте [каталог Patch34 ReaPack](https://raw.githubusercontent.com/patch-34/patch34-reapack/main/index.xml) через **Extensions → ReaPack → Import repositories…**. Найдите **Delete Nearest Marker to Cursor** в **Extensions → ReaPack → Browse packages**, установите пакет и выполните синхронизацию.

### Вручную

1. В REAPER откройте **Actions → Show action list…**.
2. Выберите **New action → Load ReaScript…**.
3. Укажите файл `Delete_Nearest_Marker_To_Cursor.lua`.
4. При необходимости назначьте сочетание клавиш.

## Принцип работы

Скрипт перебирает все маркеры проекта, для каждого вычисляет расстояние до курсора редактирования по формуле `abs(marker_pos - cursor_pos)` и удаляет ближайший. Маркер может находиться справа или слева от курсора. Операция полностью поддерживает Undo.

## Примечания

- Регионы полностью исключены из поиска.
- Если в проекте нет маркеров (есть только регионы или нет ни тех, ни других), скрипт завершается без сообщения и без изменений.

## Лицензия и авторство

Распространяется по [лицензии MIT](LICENSE).

Автор: [Aleksei Vorobev / Patch34](https://github.com/patch-34).
