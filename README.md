# InPrincipio

Desktop app (macOS) for working on text or code in parallel: one prompt, several
AI models answer side by side, so you can compare and pick the best.

*Русская версия — ниже.*

## Features

- Three built-in project profiles — Manuscript, Development, Free project —
  each with its own connected folder/file and agent roles.
- One click fans a prompt out to Claude, Codex, Cursor, and OpenCode in
  parallel.
- Orchestrator modes: plain fan-out with configurable per-engine roles,
  side-by-side comparison, read-only Plan, Propose-changes with a file diff
  preview, Apply with a per-file journal and rollback, and a Full-access mode
  where an agent can read/write files and delegate to the other CLIs itself.
- Full writing editor (Editor mode): real project documents, markdown,
  images, spell-check, disk-persisted version history (autosave backups +
  named snapshots).
- Readiness indicator per engine, Codex usage-limit display; sign-in/out for
  every engine in Settings → Agents.
- Settings: interface language (en/ru/uk/cs), appearance (Normal/Night/Book),
  per-profile project path.
- Auto-update: the app checks for and installs new versions itself.

## Requirements

Each engine needs its CLI installed and signed in, on its own subscription:

- [`claude`](https://claude.com/claude-code) (Claude Code)
- `codex` (ChatGPT)
- `cursor-agent` (Cursor)
- `opencode` (OpenCode)

## Development

```bash
pnpm install
pnpm tauri dev
```

Build:

```bash
pnpm tauri build
```

## Stack

Tauri v2 (Rust) + React + TypeScript.

## Also from InPrincipio: Grey Ash: Invasion

**Grey Ash: Invasion™** («Серый пепел. Вторжение») is a survival role-playing
game set in a modern city, now in active, intensive development.

On a quiet Friday in June, grey ash begins to fall over the city. Ilya, a
draughtsman, is locked inside his late grandfather's flat on the eighth floor
of a panel block: no keys, the phone network failing, and people outside
starting to change. The game is told in the first person and is played through
illustrated rooms with clickable objects, a notebook and a floor plan that grows
as he explores.

Where it stands now:

- A playable prologue: a few days inside the flat, from an ordinary morning to
  the way out — down a rope of knotted bedsheets to the balcony below.
- Body and mind (hunger, thirst, fatigue, nerves, wounds and ailments), skills
  that grow with use, an inventory, day-by-day news from TV, radio and forums.
- Turn-based close combat with dice rolls and body parts.
- Four languages: Russian (original), Ukrainian, English, Czech.
- macOS first (Electron + TypeScript). The source is private for now.

Made by KDV.

## Licence

Source is published so it can be read and checked; released builds are free to
use, including for paid work. Redistribution, modified versions and resale are
not granted yet — see [LICENSE](LICENSE), which says plainly what is and isn't
allowed and how to ask for the rest. Third-party components keep their own,
more permissive terms ([THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)).

---

# InPrincipio (Русский)

Настольное приложение (macOS) для параллельной работы с текстом или кодом:
один запрос — сразу несколько вариантов от разных ИИ-моделей, чтобы сравнивать
и выбирать лучший.

## Возможности

- Три встроенных профиля проекта — Рукопись, Разработка, Свободный проект —
  у каждого свой подключаемый файл/папка и свой набор ролей агентов.
- Один клик — параллельный запрос к Claude, Codex, Cursor и OpenCode.
- Режимы Оркестратора: обычный фан-аут с настраиваемыми ролями агентов,
  сравнение результатов, режим «План» (только чтение), «Предложение
  изменений» с превью diff по файлам, «Применение» с журналом по файлам и
  откатом, режим «Полный доступ», где агент сам читает/пишет файлы и может
  делегировать подзадачи другим CLI.
- Полноценный текстовый редактор (режим «Редактор»): реальные документы
  проекта, markdown, картинки, проверка орфографии, история версий на диске
  (автосохранения и именованные снимки).
- Лампочка готовности по каждому движку, индикатор лимита Codex; вход/выход
  для каждого движка — в Настройки → Агенты.
- Настройки: язык интерфейса (en/ru/uk/cs), оформление (Светлое/Тёмное/
  Сепия), путь к проекту на каждый профиль.
- Автообновление: приложение само проверяет новые версии и обновляется.

## Требования

Для каждого движка нужен установленный и авторизованный CLI, каждый на своей
подписке:

- [`claude`](https://claude.com/claude-code) (Claude Code)
- `codex` (ChatGPT)
- `cursor-agent` (Cursor)
- `opencode` (OpenCode)

## Разработка

```bash
pnpm install
pnpm tauri dev
```

Сборка:

```bash
pnpm tauri build
```

## Стек

Tauri v2 (Rust) + React + TypeScript.

## Также в InPrincipio: «Серый пепел. Вторжение»

**«Серый пепел. Вторжение»™** (Grey Ash: Invasion) — ролевая игра о выживании
в современном городе. Сейчас в активной, интенсивной разработке.

Тихой июньской пятницей на город начинает падать серый пепел. Чертёжник Илья
заперт в квартире покойного деда на восьмом этаже панельного дома: ключей нет,
связь пропадает, а люди снаружи начинают меняться. Игра ведётся от первого
лица: иллюстрированные комнаты с предметами, которые можно трогать, блокнот и
план квартиры, который дорисовывается по ходу.

Что есть сейчас:

- Проходимый пролог: несколько дней в квартире — от обычного утра до выхода по
  верёвке из простыней на балкон этажом ниже.
- Тело и нервы (голод, жажда, усталость, раны и хвори), навыки, которые растут
  от дела, инвентарь, вести по дням из телевизора, радио и форумов.
- Пошаговый ближний бой с бросками кубика и частями тела.
- Четыре языка: русский (исходный), украинский, английский, чешский.
- Сначала macOS (Electron + TypeScript). Исходники пока закрыты.

Делает KDV.

## Лицензия

Исходники опубликованы, чтобы их можно было прочитать и проверить; собранными
релизами можно пользоваться свободно, в том числе в платной работе.
Перепубликация, изменённые версии и перепродажа пока не разрешены — [LICENSE](LICENSE)
говорит прямо, что можно и чего нельзя, и как спросить про остальное. Чужие
части сохраняют свои, более свободные условия ([THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)).
