# Исторические Draft PR — архивный индекс (20.11.2026)

**Статус:** `ARCHIVE_SOURCE_INDEX_PASS / CODE_COPY_NOT_STARTED / RESTORE_NOT_TESTED`. Десять PR ниже проверены в GitHub: **CLOSED / NOT MERGED**. Исходные ветки и разговоры находятся в `market-pattern-discovery`, не в этом архивном репозитории.

| Исторический PR | HEAD commit SHA-1 | Ветка в исходном репозитории | Категория, НЕ LIVE |
|---|---|---|---|
| [#540](https://github.com/alkospacer123/market-pattern-discovery/pull/540) | `71207fe07c2728ebf81bdfb0c34fac8e2ae0ab25` | `feature/intraday-m15-robot-offline-foundation-20261016` | IntradayLab M15 — исторический самостоятельный offline робот |
| [#544](https://github.com/alkospacer123/market-pattern-discovery/pull/544) | `7f7bc38ef3aa4d0978dae6b1347e0e1e8706abb5` | `cc03-b2-repair-native-file-replace-fixture-20261017` | CC-03 / Windows File.Replace — исторический native fixture |
| [#557](https://github.com/alkospacer123/market-pattern-discovery/pull/557) | `5836971e7ff8e472d8128c675c4f837b40a036ef` | `research/t3-h1-m15-partial-tp-2r-50-20261019` | T3/H1/M15 — частичное закрытие +2R 50% |
| [#559](https://github.com/alkospacer123/market-pattern-discovery/pull/559) | `650e6f5a6940daa1f8b02ab79d11858cbf8d5484` | `codex/cc03-550-independent-source-feasibility` | CC-03/H1 — отрицательное заключение NO_SAFE_SOURCE |
| [#560](https://github.com/alkospacer123/market-pattern-discovery/pull/560) | `90a0a552c05f9ae280f4f2350fd013ea507ea00f` | `research/t3-initial-stop-forensics-v1-20261020` | T3/H1/M15 — initial stop forensics |
| [#561](https://github.com/alkospacer123/market-pattern-discovery/pull/561) | `b2c2aa31a4a4b3f186ddc4b990e8b058dd2989e5` | `cc03-finam-readonly-offline-candidate` | CC-03/H1 — эксперимент FINAM READONLY |
| [#562](https://github.com/alkospacer123/market-pattern-discovery/pull/562) | `40b59a495936adc8110a60f8c25028bbbc9c2e8d` | `research/t3-entry-diagnostics-v1-20261020` | T3/H1/M15 — диагностика качества входов |
| [#563](https://github.com/alkospacer123/market-pattern-discovery/pull/563) | `91b36991ea9b559cb318993948b061e154710e2c` | `research/t3-m15-stretched-confirmation-v1-20261020` | T3/M15 — stretched confirmation experiment |
| [#564](https://github.com/alkospacer123/market-pattern-discovery/pull/564) | `258d13df775f68149875d02a00c2289480e40666` | `research/t3-m15-be1-after-1r-v1-20261020` | T3/M15 — отрицательный BE1 after +1R |
| [#566](https://github.com/alkospacer123/market-pattern-discovery/pull/566) | `01d04ac2bd5c567940defe1d57be3f67b84469f2` | `codex/v20-04-three-robots-offline-bootstrap` | V20-04 — ранний offline bootstrap, не R088 |

## Сохранённое происхождение

- Первоисточник: [market-pattern-discovery](https://github.com/alkospacer123/market-pattern-discovery), включая 10 исходных PR, обсуждения, commit history и ссылки на CI.
- Восстановленный локальный Git mirror от 09.11: 10 HEAD из таблицы присутствовали и получили операторские архивные ссылки `refs/archive/pre-r7-20261120/pr-NNN` с `update-ref=0`; отдельно закреплён тогдашний main `0881d1e08b51a564fb54bb7d334d1578fc130400`.
- Проверенный архив `git-mirror-20261109.zip`: SHA256 `9e5d490410f7fbe3ddab983d557b981eb96146f2e5c023e42b2a1d0ee9fd0754`, прежняя копия SSD была подтверждена. Это **не** зеркало нового `main` от 20.11. Данные реестра SHA — Git SHA-1 коммитов, не SHA256 файлов.
- [Реестр 425 файловых записей и различия с main](https://github.com/alkospacer123/market-pattern-discovery/blob/main/recovery/HISTORICAL_DRAFT_REGISTER_2026-11-20.md), [R0 CC](https://github.com/alkospacer123/market-pattern-discovery/blob/main/recovery/R0_CC_DRAFT_BLOB_AUDIT_2026-11-20.md), [R0 T3](https://github.com/alkospacer123/market-pattern-discovery/blob/main/recovery/R0_T3_RESEARCH_DRAFT_BLOB_AUDIT_2026-11-20.md), [R0 ранние V20/M15](https://github.com/alkospacer123/market-pattern-discovery/blob/main/recovery/R0_V20_M15_DRAFT_BLOB_AUDIT_2026-11-20.md).
- Приоритет принятого действующего кода: `market-pattern-discovery` `main`, паспорт R088, CC-07 и TRL closeout; исторические PR не внедрять.

## Ограничения и следующий gate

Этот документ **только индексирует источники**; не утверждает, что коммиты, ветки, артефакты CI, исходные ZIP/XLSX или результаты восстановлены в самом `market-pattern-archive`. Независимая побайтовая копия каждого исторического файла и экспорт PR/Issues/CI остаются отдельными будущими задачами. Нельзя удалять исходные ветки и исторические папки из рабочего репозитория только потому, что ссылки собраны здесь.

Перед физическим переносом исходника: точный path + blob SHA, проверка секретов и лицензий, независимая копия, офлайн-прогоны V20/CC/TRL на прежнем и обновлённом дереве и разрешение оператора на необратимое удаление. Действующий V20 импортирует `TradingSystemLab.stage8_robot` и `IntradayLab.core` — **эти зависимости сохранять в основном репозитории**.
