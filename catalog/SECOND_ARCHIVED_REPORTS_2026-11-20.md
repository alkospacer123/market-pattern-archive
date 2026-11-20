# Вторая партия исторических исходных отчётов — R7

**Дата:** 20.11.2026. **Статус:** `DRAFT / ORIGINAL_GIT_BLOB_MATCH_6_OF_6 / NOT_MERGED / NO_SOURCE_DELETE`.

Эти шесть документов скопированы из закрытых исторических PR основного репозитория `market-pattern-discovery` в отдельную ветку публичного `market-pattern-archive`, **не выполняя merge в архивный main** и не меняя исходные файлы. Их прямые Git blob SHA-1 совпадают у источника и у копии.

| PR | Содержимое, исходный путь | HEAD источника | Git blob SHA-1 = archived | Решение/роль |
|---|---|---|---|---|
| [#540](https://github.com/alkospacer123/market-pattern-discovery/pull/540) | [`IntradayLab/m15_robot/AUDIT_05_20261016.md`](../historical-prs/pr-540/IntradayLab/m15_robot/AUDIT_05_20261016.md) | `71207fe07c2728ebf81bdfb0c34fac8e2ae0ab25` | `8b3fdb6b6479bd943c14b3b36d2accfab3d5b24b` | Независимый аудит offline M15; не LIVE |
| [#559](https://github.com/alkospacer123/market-pattern-discovery/pull/559) | [`ControlCenter/docs/CC03_H1_SOURCE_FEASIBILITY.md`](../historical-prs/pr-559/ControlCenter/docs/CC03_H1_SOURCE_FEASIBILITY.md) | `650e6f5a6940daa1f8b02ab79d11858cbf8d5484` | `1bdd8386ad45bba32a47c9f97a40fa05a66bbcad` | CC-03/H1: NO_SAFE_SOURCE, старый источник не принят |
| [#560](https://github.com/alkospacer123/market-pattern-discovery/pull/560) | [`audit_only/t3_initial_stop_forensics_v1/REPORT_RU.md`](../historical-prs/pr-560/audit_only/t3_initial_stop_forensics_v1/REPORT_RU.md) | `90a0a552c05f9ae280f4f2350fd013ea507ea00f` | `1c799cf534b9bf2bc9aaa8327feb40c2bb3817b5` | Укороченные стопы не прошли критерии устойчивости |
| [#562](https://github.com/alkospacer123/market-pattern-discovery/pull/562) | [`audit_only/t3_entry_diagnostics_v1/REPORT_RU.md`](../historical-prs/pr-562/audit_only/t3_entry_diagnostics_v1/REPORT_RU.md) | `40b59a495936adc8110a60f8c25028bbbc9c2e8d` | `ea5837fda2a5a7838b3cd9a9f9607763f895e976` | Диагностика входов; фильтр и прибыльность не подтверждены |
| [#563](https://github.com/alkospacer123/market-pattern-discovery/pull/563) | [`audit_only/t3_m15_stretched_breakout_confirmation_v1/REPORT_RU.md`](../historical-prs/pr-563/audit_only/t3_m15_stretched_breakout_confirmation_v1/REPORT_RU.md) | `91b36991ea9b559cb318993948b061e154710e2c` | `c841de4753bd6e0425da1e31535af58b043a9cfe` | Подтверждение пробоя не удовлетворило основному критерию |
| [#566](https://github.com/alkospacer123/market-pattern-discovery/pull/566) | [`V20_TradingSystem_M15/V20-04/README_RU.md`](../historical-prs/pr-566/V20_TradingSystem_M15/V20-04/README_RU.md) | `01d04ac2bd5c567940defe1d57be3f67b84469f2` | `c60321304894095e1f9d82e78fc93ceae0b92a02` | Ранний V20-04 offline bootstrap, не R088 |
## Границы доказательств

- Содержимое этих шести файлов совпадает с соответствующими оригинальными Git blobs: **MATCH 6/6**. Это НЕ означает архивирование всех файлов PR, релевантных test fixtures, оригинальных котировок, вложенных CSV/ZIP/XLSX или всех отчётов.
- В отчётах могут сохраняться относительные Markdown-ссылки на соседние материалы оригинального PR. **При открытии ссылок в этом частичном архиве часть целей пока отсутствует.** Для полного контекста идти по ссылке PR и исходному HEAD.
- В PR #540 аудит относится к отдельному старому offline M15, не действующему V20. В PR #566 — устаревшая ранняя документация V20-04; **приоритет** у актуального [R088](https://github.com/alkospacer123/market-pattern-discovery/blob/main/V20_TradingSystem_M15/V20-08/LIVE_RELEASE_R088_20261120_RU.md).
- Автоматическая поверхностная проверка исходников не обнаружила распространённых шаблонов секретов, персональных email, явно указанных номеров счетов или пользовательских Windows путей. Это не полный privacy audit исторических репозиториев. Нельзя автоматически публиковать другие файлы.
- Не удалять самостоятельные исходные ветки H1/M15 или каталоги `TradingSystemLab/` и `IntradayLab/` из действующего репозитория: V20 использует `TradingSystemLab.stage8_robot` и `IntradayLab.core`.
- **Остаётся:** независимая копия полной современной Git-истории, Issues/PR/CI, оригиналов исследовательских артефактов и изолированный R6 restore. Никакой LIVE/FINAM операции не выполнялось.

До отдельного разрешения владельца этот PR остаётся Draft; будущий merge допускается только без удаления веток и исходных файлов.
