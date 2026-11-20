# R7 — полный исторический комплект STOP/TICK GRID, 12.10.2026

**Source MAIN, зафиксирован для копирования:** `alkospacer123/market-pattern-discovery@f15d565755b996252081ed49ed5a094ee1e8d820`.

**Архивная ветка / статус:** `COPY_STAGED / GIT_BLOB_SHA_MATCH_16_OF_16 / DO_NOT_DELETE_SOURCE / NO_OFFLINE_RUN`.

**Что за комплект:** изолированный исторический audit-only `audit_only/stop_tick_grid_20261012/`, относящийся к исследованию STOP/TICK GRID. Исходный [README](https://github.com/alkospacer123/market-pattern-discovery/blob/f15d565755b996252081ed49ed5a094ee1e8d820/audit_only/stop_tick_grid_20261012/README.md) утверждает, что эти файлы **не импортируются роботом**, `PRODUCTION_CHANGES=NONE`. Это **утверждение первоисточника**, а не доказательство полной отсутствия зависимостей во всех проектах. Историческое исследование может быть полезно TRL или реконструкции H1. В текущем рабочем `main` оригиналы сохранены.

**Назначение копии:** `historical-tree/audit_only/stop_tick_grid_20261012/`. Архив содержит все 16 файлов директории: README, отчёт, `audit.py`, `supplemental.py`, `run_existing_tests.py`, JSON и 8 CSV с результатами/сигнальными диагностическими доказательствами. Относительные ссылки внутри директории сохранены. Для запуска воспроизводимых проверок **необходим отдельно восстановленный исходный checkout и фиксированные внешние данные**, одного архива недостаточно.

## Реестр побайтовой сверки

У всех 16 элементов Git blob SHA-1 равен SHA той же оригинальной записи в рабочем источнике. Ни один исходный файл не удалён, Git history не переписывалась.

| Исходный относительный путь | Проверенный Git blob SHA-1 оригинала = архивной копии | Размер в байтах (из Git tree) |
|---|---|---:|
| `audit_only/stop_tick_grid_20261012/audit.py` | `26e22c720f32bd867d3195064842bc635cf308c1` | 22035 |
| `audit_only/stop_tick_grid_20261012/authority_reconciliation.csv` | `64108a79505c810a48e8098865e543af17f98cb3` | 31051 |
| `audit_only/stop_tick_grid_20261012/full_available_admitted_entries.csv` | `c85a22ca8ad0057c8b841510c895ef1006a820af` | 136771 |
| `audit_only/stop_tick_grid_20261012/full_available_raw_signals.csv` | `2f6cfbbd941a2a89bfbd9e3d28154dbe9bc7b132` | 442663 |
| `audit_only/stop_tick_grid_20261012/lifecycle_admitted_entries.csv` | `66eb53d8c8b9e47af4fda9c65e981125f7c8f49e` | 139943 |
| `audit_only/stop_tick_grid_20261012/lifecycle_raw_signals.csv` | `f01244de3817422bf85ea25d4b48bcd966d4aece` | 449371 |
| `audit_only/stop_tick_grid_20261012/outward_rounding_math_only.csv` | `dc5a392638c29c5e4f27925893e0073f3906246e` | 54288 |
| `audit_only/stop_tick_grid_20261012/production_reconciliation.csv` | `64108a79505c810a48e8098865e543af17f98cb3` | 31051 |
| `audit_only/stop_tick_grid_20261012/README.md` | `19ba6396b513acce86b753a28a46944013e26528` | 2702 |
| `audit_only/stop_tick_grid_20261012/REPORT_RU.md` | `dc04c2c99b41c3a6f1f167d04c73f701191aa4f8` | 30670 |
| `audit_only/stop_tick_grid_20261012/results.json` | `226eb9c7acf576a60203bcf8c78dbd41629b8041` | 51904 |
| `audit_only/stop_tick_grid_20261012/run_existing_tests.py` | `d64da460e2e2355b55e29450ec6a29747e25747f` | 1219 |
| `audit_only/stop_tick_grid_20261012/runtime_matrix.csv` | `94b45bd26c2ec77544c2f5dfd4bd764a35e14481` | 2772 |
| `audit_only/stop_tick_grid_20261012/supplemental_results.json` | `c563f31124c22361a3293c4cedacc58e92ad79a6` | 16906 |
| `audit_only/stop_tick_grid_20261012/supplemental.py` | `ffd2177f27bf24ecbaeab831431a55bbbb1ef4cb` | 6936 |
| `audit_only/stop_tick_grid_20261012/verification.json` | `a993802c64f872491dfcd0c7df7e970cbc6ed7dd` | 4826 |

## Границы доказательств и безопасность

- **COPY_GIT_BLOB_MATCH=PASS_16_OF_16**: содержимое каждого сохранённого Git blob совпало. Это **не** означает `OFFLINE_REPRODUCTION_PASS`, `CURRENT_LIVE_PASS`, `ARCHIVE_INDEPENDENT_RESTORE_PASS` или `CAN_DELETE_SOURCE`.
- Документированный исходный контур — read-only диагностика старого STOP/TICK GRID, а не действующий V20 release. Нет разрешений изменять риск, сигналы, SLTP, FINAM, запускать H1/M15 или проводить сделки.
- До архивирования сканировались очевидные шаблоны GitHub-токенов, приватных ключей, e-mail, пользовательских Windows-путей и полей номеров торговых счетов. В 16 файлах совпадений по применённым шаблонам не найдено. Исходные CSV описаны исходным README как **производные исследовательские сигналы, не брокерские заявки**. Это ограниченный эвристический просмотр, не полный privacy audit. Публичность архива не меняет статуса этих файлов как исторических материалов.
- Данные оригинального исследования и воспроизведение: исходный README ссылается на code `688560ec2e8a71c1085bec255a9660783b51e122` и data `50f1fd2178c18b7ab3bd969be82ad01f47a34745`; эти точные исторические срезы **не воспроизводились** в рамках R7, номера не заменяют действующий `main`.
- **Запрещено** перемещать или удалять эту папку из `market-pattern-discovery` до нового независимого полного Git mirror/PR-issues-CI экспорта, статических dependency checks, offline regressions и **отдельного разрешения оператора на точный список удалений**.
- `TradingSystemLab/` и `IntradayLab/` сохраняем целиком; `src/`, `tests/`, `config/`, `schemas/`, `BBW/`, `bbw_system/`, `results/` не удалять по аналогии: их связи с действующей/исследовательской базой проверяются отдельно.
- Recovery R5 и restore R6 по утверждённому Roadmap выполняются в конце **после Kimi**. Перед любым необратимым R7 действием нужен защитный checkpoint, который ещё `NOT_VERIFIED`.

**Вывод для Kimi:** архивный SNAPSHOT является источником исторических исследований и не заменяет актуальные `V20-08/LIVE_RELEASE_R088_20261120_RU.md`, действующий Control Center и TRL. Git Merge не равен LIVE.
