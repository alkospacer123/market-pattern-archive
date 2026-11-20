# Архивная партия №4 — методы, исходники и тесты отвергнутых исследований

**Дата:** 20.11.2026. **Статус:** `STAGED_DRAFT / ORIGINAL_GIT_BLOB_MATCH_8_OF_8 / NOT_MERGED / NO_SOURCE_DELETE`.

Архивные отчёты из PR #557 (PARTIAL_TP_2R_50: CASH_MODEL_NOT_VALIDATED / INCONCLUSIVE) и #564 (BE1 AFTER +1R: rejected) были ранее сохранены отдельными копиями. Эта партия добавляет **первичные методы и часть offline-кода**, которые не присутствуют по этим путям в текущем `market-pattern-discovery/main`. Никакого переноса действующих V20, CC, LIVE, FINAM, приватных аккаунтов и секретов.

| PR-источник | Оригинальный путь / новая архивная копия | Исторический HEAD SHA | Git blob SHA-1 источника = архив | Роль |
|---|---|---|---|---|
| [#557](https://github.com/alkospacer123/market-pattern-discovery/pull/557) | [`audit_only/t3_h1_m15_partial_tp_2r_50/PROTOCOL_RU.md`](../historical-prs/pr-557/audit_only/t3_h1_m15_partial_tp_2r_50/PROTOCOL_RU.md) | `5836971e7ff8e472d8128c675c4f837b40a036ef` | `ef81ba22e884eb60a3b9f7a3dc21a5153a2ab5ea` | Предварительно зарегистрированный метод сравнения |
| [#557](https://github.com/alkospacer123/market-pattern-discovery/pull/557) | [`audit_only/t3_h1_m15_partial_tp_2r_50/EXECUTION_CORRECTION.json`](../historical-prs/pr-557/audit_only/t3_h1_m15_partial_tp_2r_50/EXECUTION_CORRECTION.json) | `5836971e7ff8e472d8128c675c4f837b40a036ef` | `0314ce11d485faedc4a685527be5722613b87ba0` | Исправление неверного учёта исполнения |
| [#557](https://github.com/alkospacer123/market-pattern-discovery/pull/557) | [`audit_only/t3_h1_m15_partial_tp_2r_50/SOURCE_MANIFEST.json`](../historical-prs/pr-557/audit_only/t3_h1_m15_partial_tp_2r_50/SOURCE_MANIFEST.json) | `5836971e7ff8e472d8128c675c4f837b40a036ef` | `55fc7c14bbce80994d77b2284b3df727cd37574f` | Границы данных и исходные SHA |
| [#557](https://github.com/alkospacer123/market-pattern-discovery/pull/557) | [`audit_only/t3_h1_m15_partial_tp_2r_50/test_synthetic.py`](../historical-prs/pr-557/audit_only/t3_h1_m15_partial_tp_2r_50/test_synthetic.py) | `5836971e7ff8e472d8128c675c4f837b40a036ef` | `ea4b29331a62a545c8c948e7716509abe9eae535` | Исходный offline синтетический тест |
| [#564](https://github.com/alkospacer123/market-pattern-discovery/pull/564) | [`audit_only/t3_m15_be1_after_1r_v1/PROTOCOL_RU.md`](../historical-prs/pr-564/audit_only/t3_m15_be1_after_1r_v1/PROTOCOL_RU.md) | `258d13df775f68149875d02a00c2289480e40666` | `9801d969de275104bd011df44cdf59b2900d20cc` | Протокол до получения результата |
| [#564](https://github.com/alkospacer123/market-pattern-discovery/pull/564) | [`audit_only/t3_m15_be1_after_1r_v1/INDEPENDENT_VERIFICATION.json`](../historical-prs/pr-564/audit_only/t3_m15_be1_after_1r_v1/INDEPENDENT_VERIFICATION.json) | `258d13df775f68149875d02a00c2289480e40666` | `251eb7899766c276ba1a3cc605cf26e740d53e36` | Границы независимой проверки |
| [#564](https://github.com/alkospacer123/market-pattern-discovery/pull/564) | [`audit_only/t3_m15_be1_after_1r_v1/engine.py`](../historical-prs/pr-564/audit_only/t3_m15_be1_after_1r_v1/engine.py) | `258d13df775f68149875d02a00c2289480e40666` | `58c30c8011f473f9558d5177c6c50fc479c88ca6` | Исходный offline экспериментальный BE1-движок (НЕ LIVE) |
| [#564](https://github.com/alkospacer123/market-pattern-discovery/pull/564) | [`audit_only/t3_m15_be1_after_1r_v1/test_contract.py`](../historical-prs/pr-564/audit_only/t3_m15_be1_after_1r_v1/test_contract.py) | `258d13df775f68149875d02a00c2289480e40666` | `efc0fb447a0ba40cd790eac568afee39f37787a1` | Синтетический контрактный offline-тест |

## Проверки и границы

- Для восьми файлов проверены Git blob SHA-1 у HEAD исходных закрытых PR и в архивной ветке: **MATCH 8/8**; скопированы исходные байты без редактирования. Это не гарантирует побайтовую сохранность всего дерева PR и не является SHA256 независимого ZIP.
- До копирования каждый текст прошёл ограниченную проверку известных форматов ключей/секретов и пользовательских путей; явных совпадений не выявлено. `SOURCE_MANIFEST.json` отдельно проверен на структуру JSON и подозрительные числа: длинные числовые последовательности относились к исследовательским метрикам, а не распознанным идентификаторам счетов. **Это не полноценный privacy-аудит** всего исследования.
- Исторические отчёты могут ссылаться относительными путями на отсутствующие здесь файлы. Для воспроизводимости ещё нужны другие модули, исходные данные, тесты и точные версии окружения. Присутствие `engine.py` **не** означает, что эксперимент запускается из текущей архивной папки, и не разрешает запуск H1/M15 или LIVE.
- Первоначальные PR #557/#564 и их Git ветки сохранены в `market-pattern-discovery`; из шести рабочих каталогов ничего не перемещено. Существующие V20-зависимости `TradingSystemLab.stage8_robot` и `IntradayLab.core` не трогать.
- В `market-pattern-archive/main` после #3 подтверждено **11 отдельных исходных файлов из 10 исторических PR**, а после отдельного одобрения и Merge этого PR станет 19. Это **не** 19 независимых PR и не сохранение всех 425 изменённых файловых записей. Число «425−19» не эквивалентно числу уникальных недостающих первоисточников; некоторые присутствуют в текущем рабочем MAIN, часть пересекается по истории.
- Полный текущий Git mirror, независимый экспорт GitHub PR/Issues/CI, полный privacy review, offline reproductions и cold restore остаются `NOT_VERIFIED`.

## Для следующего этапа

Расширять архив по принципу `source file + protocol + implementation + test + evidence + independent verification`; не копировать массово по расширениям, не публиковать FINAM/DPAPI/SQLite. После независимого полного защитного комплекта, dependency/offline regressions и отдельного разрешения можно обсуждать удаление **конкретных** ненужных файлов, но не целых шести каталогов.

**R7 архивное копирование ≠ R5 окончательный Backup ≠ R6 Cold Restore.** Документ не предоставляет полномочий Merge, удаления исходников или торговых действий.
