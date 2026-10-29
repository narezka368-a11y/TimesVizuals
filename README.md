# TimesVizuals

Клиентский мод для Minecraft **1.21.4** (Fabric). Свой ClickGui, HUD-эдитор, менеджер аккаунтов, кастомное главное меню и 38 модулей.

## Возможности

- **ClickGui** — тёмное стекло, акцентный градиент, поиск, раскрывающиеся настройки, тултипы (RShift)
- **HUD-эдитор** — перетаскивание всех элементов с сеткой 2 px (RCtrl)
- **Alt Manager** — список ников, создание/удаление/Random, переключение сессии
- **Главное меню** — своя анимированная замена ванильному титульнику
- **Метки клиента** — бейдж ⟦TV⟧ в табе и чате
- **Модули**: render (13), hud (11), player (5), combat (4), client (4), movement (1)

## Установка

1. Fabric Loader для 1.21.4 + Java 21
2. Положить `timesvizuals-1.0-1.21.4.jar` и **Fabric API** в папку `mods`
3. `RShift` — меню, `RCtrl` — HUD-эдитор

## Сборка

```bash
gradlew build
# готовый jar: build/libs/timesvizuals-1.0-1.21.4.jar
```

## Сайт

Папка `site/` — готовая статическая страница:

```
site/
├── index.html                      # лендинг
├── 404.html                        # страница ошибки
├── README.md
├── assets/
│   ├── style.css
│   └── logo.svg
└── download/
    └── timesvizuals-1.0-1.21.4.jar # актуальная сборка
```

Открывается двойным кликом по `index.html` — без сервера и сборки.

### Публикация на GitHub Pages

**Вариант 1 — через веб-интерфейс (без установки программ):**

1. GitHub → **New repository** → имя `TimesVizuals`, Public.
2. **Add file → Upload files** → перетащить содержимое папки `site` (не саму папку).
3. **Commit changes**.
4. **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
5. Через минуту сайт будет на `https://<ник>.github.io/TimesVizuals/`.

**Вариант 2 — через git:**

```bash
cd site
git init
git add .
git commit -m "TimesVizuals site"
git branch -M main
git remote add origin https://github.com/<ник>/TimesVizuals.git
git push -u origin main
```

## Лицензия

Исходники распространяются как есть, без гарантий. Проект не связан с Mojang или Microsoft.
