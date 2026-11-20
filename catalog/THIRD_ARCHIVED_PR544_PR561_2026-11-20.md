# Архивная партия #3 — исторические PR #544 и #561

**Срез:** 20.11.2026. **Статус:** `DRAFT / GIT_BLOB_MATCH_3_OF_3 / SOURCE_UNCHANGED / NO_MERGE`. Копии взяты из закрытых без Merge исторических PR основного репозитория.

| Исторический источник | Путь в PR и проверенный HEAD SHA | Git blob SHA-1 (источник = архив) | Статус |
|---|---|---|---|
| [#544](https://github.com/alkospacer123/market-pattern-discovery/pull/544) | [`ControlCenter/tests/test_cc03_b2_replace_native_fixture.py`](../historical-prs/pr-544/ControlCenter/tests/test_cc03_b2_replace_native_fixture.py); `7f7bc38ef3aa4d0978dae6b1347e0e1e8706abb5` | `87a9de1e1b4b1e2045b099109efe6420a3151ce8` | Старый native Windows File.Replace fixture, не текущий CC-07 |
| [#561](https://github.com/alkospacer123/market-pattern-discovery/pull/561) | [`ControlCenter/docs/CC03_BROKER_SNAPSHOT_RELEASE.md`](../historical-prs/pr-561/ControlCenter/docs/CC03_BROKER_SNAPSHOT_RELEASE.md); `b2c2aa31a4a4b3f186ddc4b990e8b058dd2989e5` | `3c5191b607c5421d06075e19e18366bf3677a6a8` | Старый draft readonly snapshot, не действующая FINAM/CC интеграция |
| [#561](https://github.com/alkospacer123/market-pattern-discovery/pull/561) | [`ControlCenter/docs/CC03_FINAM_READONLY_ONE_SHOT_DESIGN.md`](../historical-prs/pr-561/ControlCenter/docs/CC03_FINAM_READONLY_ONE_SHOT_DESIGN.md); `b2c2aa31a4a4b3f186ddc4b990e8b058dd2989e5` | `cd492583193d3724c252053da18c1f01d2ceac5d` | Старый offline-design, НЕ брокерский источник |

## Безопасность и полнота

При повторной проверке обе версии каждого из трёх текстовых файлов имеют идентичные Git blob SHA. Выполнен ограниченный поиск очевидных токенов/секретов, email, путей профилей Windows и номеров счёта; совпадений нет. Это не общий аудит всего PR. **Не запускать** ни broker readonly, ни Windows fixture на Intel; не загружать частные логи, FINAM/DPAPI и исходные токены в публичный архив.

**После принятия архивного PR #3** архив будет иметь 11 отдельных оригинальных файлов, по крайней мере один от каждого из всех десяти исторических PR. **Это всё ещё не полная независимая копия всех 425 файловых записей, обсуждений, веток, CI, ZIP/XLSX или Git-истории.** Сохранять исходные PR и ветки.

Не удалять ничего из `market-pattern-discovery` до отдельной проверки V20/CC/TRL dependencies, тестов и разрешения владельца. Архивный PR #3 не даёт полномочий на установку, LIVE, Merge другого PR или удаление веток.
