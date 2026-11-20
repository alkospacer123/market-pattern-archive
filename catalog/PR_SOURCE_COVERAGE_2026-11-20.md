# R7 — покрытие 10 исторических PR независимыми копиями

**Срез:** 20.11.2026. В `market-pattern-archive/main` после #3 лежит **11 исходных файлов**, а в отдельном Draft этой партии подготовлено ещё **8 файлов** из PR #557 и #564. После отдельного разрешения и Merge станет **19** файлов с проверенным Git blob SHA. **Ниже — стадия после возможного Merge #4, не текущий статус main.**

| Закрытый PR | Изменённых файловых записей в PR | Исходных файлов скопировано и сверено SHA (после #4) | Пока не скопировано (файловых записей, не уникальных объектов) |
|---|---:|---:|---:|
| [#540](https://github.com/alkospacer123/market-pattern-discovery/pull/540) | 89 | 1 | 88 |
| [#544](https://github.com/alkospacer123/market-pattern-discovery/pull/544) | 2 | 1 | 1 |
| [#557](https://github.com/alkospacer123/market-pattern-discovery/pull/557) | 44 | 5 | 39 |
| [#559](https://github.com/alkospacer123/market-pattern-discovery/pull/559) | 11 | 1 | 10 |
| [#560](https://github.com/alkospacer123/market-pattern-discovery/pull/560) | 65 | 1 | 64 |
| [#561](https://github.com/alkospacer123/market-pattern-discovery/pull/561) | 27 | 2 | 25 |
| [#562](https://github.com/alkospacer123/market-pattern-discovery/pull/562) | 56 | 1 | 55 |
| [#563](https://github.com/alkospacer123/market-pattern-discovery/pull/563) | 59 | 1 | 58 |
| [#564](https://github.com/alkospacer123/market-pattern-discovery/pull/564) | 68 | 5 | 63 |
| [#566](https://github.com/alkospacer123/market-pattern-discovery/pull/566) | 4 | 1 | 3 |
| **Всего** | **425** | **19** | **406** |

## Что именно означают числа

- **425** — сумма *записей изменённых путей* в десяти исторических GitHub PR; не число уникальных файлов во всей Git-истории и не количество отдельных исследований.
- **19** — прямые оригинальные текстовые/кодовые файлы с совпавшим Git blob SHA источника и архива, считая 8 staged в Draft PR #4. Для #557 и #564 первые два отчёта сохранены в укороченных архивных путях `historical-prs/pr-N/REPORT_RU.md`; оригинальные пути и blob SHA закреплены [в первом манифесте](FIRST_ARCHIVED_REPORTS_2026-11-20.md).
- **406** — арифметическая разница для покрытия записей, **не доказанное число уникальных недостающих первоисточников**. Часть исторического кода/результатов уже находится в `market-pattern-discovery/main`; часть является общими зависимостями, повторами или не подлежит публичному размещению.
- Существование копии отчёта **не** означает архивирование всех файлов его PR или воспроизведение исследования. Отдельный комплект Git refs, PR/Issues/CI, Binary originals и независимый restore ещё не подтверждён.

## Приоритеты, а не массовая копия

1. **Сначала методы и отрицательные результаты:** отчёты + preregistered PROTOCOL, implementation, synthetic tests, source manifests + сверка SHA. Настоящий PR дополняет #557/#564, но **не завершает** их воспроизводимость.
2. **Оставить в рабочем монорепозитории:** шесть защищённых каталогов, включая `TradingSystemLab.stage8_robot` и `IntradayLab.core`, используемые действующим V20; также другие пути до аудита dependency/CI.
3. **Проверять кандидатов:** есть ли точный blob уже в действующем `main`, нужен ли архивный дубликат; есть ли секреты, приватный FINAM/DPAPI, идентификаторы счетов, необезличенные SQLite и сообщения; при рисках — не загружать публично.
4. **Контрольный snapshot до очистки:** новый полный Git mirror текущего main, PR/Issues/CI, SHA и независимое хранение. Проверенный ZIP после #571 — не полный Git mirror и не отражает #578/#579.
5. **Удаление — исключительно после** copy → SHA/privacy verify → dependency/offline regressions → явное разрешение оператора на конкретный PR удаления. Для R5 Final Backup и R6 cold restore порядок прежний: после Kimi.

**R7 нельзя объявлять полным PASS по текущей выборке.** Kimi должен различать ARCHIVE/RESEARCH/MAIN/INSTALLED/LIVE/RECON.
