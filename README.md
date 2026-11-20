# Market Pattern Archive — исторические материалы и проверяемое происхождение

**Дата основания каталога:** 20.11.2026. **Статус:** `ARCHIVE_PARTIAL_ORIGINALS / 11_SOURCE_BLOBS_WITH_PROVENANCE / NOT_FULL_RECOVERY`. Это **публичный** исторический репозиторий и НЕ рабочая среда для торговли.

## Рабочая архитектура — читать прежде архивов

**Единый рабочий репозиторий:** [alkospacer123/market-pattern-discovery](https://github.com/alkospacer123/market-pattern-discovery) содержит:
- `V20_TradingSystem_M15/` — **ACTIVE**, текущая V20 R088.
- `ControlCenter/` — **ACTIVE**, операторская панель V20.
- `TradingResearchLab/` — **RESEARCH**, исследования и Journal.
- `recovery/` — **KNOWLEDGE**, общая проверяемая база GPT/Kimi.
- `TradingSystemLab/` — **LEGACY H1 + DEPENDENCY** (модули `TradingSystemLab.stage8_robot` используются V20).
- `IntradayLab/` — **LEGACY M15 + DEPENDENCY** (модули `IntradayLab.core` используются V20).

**Текущий релизный паспорт и ограничения для Kimi:** [карта границ](https://github.com/alkospacer123/market-pattern-discovery/blob/main/recovery/KIMI_REPOSITORY_BOUNDARIES_2026-11-20.md), [V20 R088](https://github.com/alkospacer123/market-pattern-discovery/blob/main/V20_TradingSystem_M15/V20-08/LIVE_RELEASE_R088_20261120_RU.md), [TRL November closeout](https://github.com/alkospacer123/market-pattern-discovery/blob/main/TradingResearchLab/reports/TRL-NOV-2026-FINAL-CLOSEOUT.md).

**Отдельный репозиторий данных:** [alkospacer123/market-pattern-data](https://github.com/alkospacer123/market-pattern-data). Не переносить данные в этот публичный архив без проверки источников и разрешений.

## Что допускается сюда переносить

Только подтверждённые исторические самостоятельные реализации, неиспользуемые эксперименты, результаты с проверенными источниками, включая отрицательные гипотезы. Каждый перенос должен сохранять оригинальный путь, исходный commit SHA и Git blob SHA / SHA256, статус принятия, ссылки на PR/Issues/CI и подтверждение отсутствия чувствительного содержимого.

Исторические H1/M15 **не удалять целиком** из рабочего репозитория: V20 использует отдельные модули. До переноса отдельных файлов: dependency/import check → offline regression V20/CC/TRL → immutable source hash → архивная копия → проверка копии → отдельное разрешение на удаление оригинала.

## Что пока содержит этот архив

После архивных Squash Merge #1/#2 и подготовки #3 здесь сохранены **11 оригинальных файлов с идентичными Git blob SHA из 10 исторических PR** (после Merge #3). До него в `main` только 8 файлов из #1/#2. Это **не полные копии PR**, не Git mirror и не резервный комплект для восстановления. История исходных PR/коммитов пока хранится в `market-pattern-discovery`, а архивный Git mirror от 09.11 отдельно проверялся на Intel/SSD. Исходный `market-pattern-discovery` не удалять и его Git-историю не переписывать.

[Реестр десяти PR](catalog/HISTORICAL_DRAFT_PR_INDEX_2026-11-20.md), [первая партия](catalog/FIRST_ARCHIVED_REPORTS_2026-11-20.md), [вторая партия](catalog/SECOND_ARCHIVED_REPORTS_2026-11-20.md), [третья партия (Draft #3)](catalog/THIRD_ARCHIVED_PR544_PR561_2026-11-20.md).

Старые PR, закрытые без Merge: #540, #544, #557, #559, #560, #561, #562, #563, #564, #566. Их ветки сохранены в исходном GitHub. В архиве они индексируются **не как действующий код**.

## Безопасность и запреты

- Не публиковать FINAM/DPAPI, реальные счета, доступы, токены, необезличенные SQLite, приватные журналы и сырые чаты.
- Не восстанавливать или запускать H1/M15 LIVE; не смешивать архивный CC-03/H1 с действующим CC-07/V20.
- Не выполнять Merge, удаление исходников, переписывание Git history, установку, заявки/отмены FINAM, перезапуск LIVE без разрешения оператора.
- Различать `MAIN`, `INSTALLED`, `LIVE`, `RESEARCH`, `ARCHIVE`, `RECON`; отсутствие данных отмечать `NOT_VERIFIED`.
- Два ИИ GPT/Codex и Kimi AI/Kimi Code — равные партнёры с отдельными авторизациями и общими проверяемыми источниками. Этот архив не заменяет три отдельные логические базы Kimi.

## Recovery

ZIP `market-pattern-discovery` после PR #571 проверен владельцем на внешнем SSD: `SHA256=36D387EB106F13E2EC6CA7DF6F3D2BA59204DDEAC3216A46CCFABFEB8F48C329`, `ssd_copy_verified=pass`. После следующего документационного PR #578 этот файловый ZIP **не соответствует новому `main`**. Он не содержит полную Git-историю, PR/Issues/CI и не доказывает cold restore. Финальный Recovery и R6 isolated restore тесты остаются после адаптации Kimi.
