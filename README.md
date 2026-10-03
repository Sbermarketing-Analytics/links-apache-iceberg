# Всё про Apache Iceberg: полезные ссылки

Ресурсы по Apache Iceberg, собранные в одном месте: от первых шагов до продвинутого обслуживания. Акцент на официальной документации, открытых каталогах и работающих примерах.

Метки: ✅ — ссылка доступна; ⚠️ — автоматическая проверка невозможна, но источник фигурирует в официальных материалах.

## Содержание

- [С чего начать](#с-чего-начать)
- [Справочники](#справочники)
- [Основы формата](#основы-формата)
- [Каталоги](#каталоги)
- [Движки запросов](#движки-запросов)
- [Практика](#практика)
- [Оптимизация](#оптимизация)
- [Версионирование](#версионирование)
- [Облака](#облака)
- [Стриминг и инструменты](#стриминг-и-инструменты)
- [Контент](#контент)
- [Сообщества](#сообщества)

## С чего начать

- [Практический курс](https://subquery.ru/course/iceberg) — русскоязычный курс: 6 глав, 19 уроков.
- [Введение в Iceberg](https://subquery.ru/blog/courses/iceberg/introduction) — формат простыми словами, с примерами.
- [Spark Quickstart](https://iceberg.apache.org/spark-quickstart/) ✅ — быстрый старт с Docker Compose.

## Справочники

| Ресурс | Что внутри | Статус |
| --- | --- | --- |
| [Официальный сайт](https://iceberg.apache.org/) | Обзор проекта и возможности | ✅ |
| [Документация](https://iceberg.apache.org/docs/latest/) | Концепции и интеграции | ✅ |
| [Спецификация](https://iceberg.apache.org/spec/) | Формат v1–v3 детально | ✅ |
| [Релизы](https://iceberg.apache.org/releases/) | Версии и артефакты | ✅ |
| [Блог](https://iceberg.apache.org/blog/) | Новости и техматериалы | ✅ |

## Основы формата

- [Архитектура и концепции](https://subquery.ru/blog/courses/iceberg/architecture-and-concepts) — файлы данных, манифесты, метаданные.
- [ACID-транзакции](https://subquery.ru/blog/courses/iceberg/acid-transactions) — гарантии целостности.
- [UPDATE и DELETE](https://subquery.ru/blog/courses/iceberg/updates-and-deletes) — copy-on-write и merge-on-read.
- [Эволюция схемы](https://subquery.ru/blog/courses/iceberg/data-types-and-schema-evolution) — безопасные изменения структуры.

## Каталоги

| Каталог | Описание | Статус |
| --- | --- | --- |
| [Урок про каталоги](https://subquery.ru/blog/courses/iceberg/catalogs) | Выбор каталога для таблиц | ✅ |
| [Протокол REST Catalog](https://iceberg.apache.org/docs/latest/rest-protocol/) | Спецификация протокола | ✅ |
| [Клиент REST-каталога](https://iceberg.apache.org/docs/latest/rest-catalog/) | Настройка Spark/Flink | ✅ |
| [Apache Polaris](https://polaris.apache.org/) | Открытый каталог ASF | ✅ |
| [Polaris (GitHub)](https://github.com/apache/polaris) | Код и быстрый старт | ✅ |
| [Lakekeeper](https://lakekeeper.io/) | REST-каталог на Rust | ✅ |
| [Lakekeeper (GitHub)](https://github.com/lakekeeper/lakekeeper) | Исходники и деплой | ✅ |
| [Project Nessie](https://projectnessie.org/) | Каталог с ветвлением | ✅ |
| [Unity Catalog](https://github.com/unitycatalog/unitycatalog) | Мультимодальный каталог LF | ✅ |
| [AWS Glue](https://iceberg.apache.org/docs/latest/aws/#glue-catalog) | Каталог в AWS | ✅ |
| [Hive Metastore](https://iceberg.apache.org/docs/latest/hive/) | Глобальный каталог Hive | ✅ |

## Движки запросов

| Движок | Ресурс | Статус |
| --- | --- | --- |
| [Экосистема движков](https://subquery.ru/blog/courses/iceberg/query-engines-and-ecosystem) | Обзор Spark, Flink, Trino, Python | ✅ |
| [Trino (статья)](https://subquery.ru/blog/trino) | Обзор Trino и интеграций | ✅ |
| [DuckDB](https://duckdb.org/docs/current/core_extensions/iceberg/overview.html) | Расширение Iceberg | ✅ |
| [Trino connector](https://trino.io/docs/current/connector/iceberg.html) | Коннектор Iceberg | ✅ |
| [PyIceberg](https://py.iceberg.apache.org/) | Python-реализация | ✅ |
| [iceberg-rust](https://github.com/apache/iceberg-rust) | Реализация на Rust | ✅ |
| [iceberg-go](https://github.com/apache/iceberg-go) | Реализация на Go | ✅ |
| [StarRocks](https://docs.starrocks.io/docs/data_source/catalog/iceberg/) | Внешний каталог StarRocks | ⚠️ |
| [ClickHouse](https://clickhouse.com/docs/en/engines/table-engines/integrations/iceberg) | Движок в ClickHouse | ✅ |
| [Flink Quickstart](https://iceberg.apache.org/flink-quickstart/) | Старт со Flink | ✅ |

## Практика

- [Упражнение: каталоги](https://subquery.ru/blog/courses/iceberg/catalogs-exercise) — создание таблицы и снапшоты.
- [Упражнение: эволюция схемы](https://subquery.ru/blog/courses/iceberg/schema-evolution-exercise) — правка колонок на живых данных.
- [Упражнение: партицирование](https://subquery.ru/blog/courses/iceberg/partitioning-exercise) — партиции и отсечение файлов.
- [Упражнение: time travel](https://subquery.ru/blog/courses/iceberg/timetravel-exercise) — путешествие по истории.
- [Упражнение: ветвление](https://subquery.ru/blog/courses/iceberg/branching-exercise) — теги и ветки руками.
- [Упражнение: обслуживание](https://subquery.ru/blog/courses/iceberg/maintenance-exercise) — чистка таблиц.
- [docker-spark-iceberg](https://github.com/databricks/docker-spark-iceberg) ✅ — готовый стенд для экспериментов.
- [Nessie Sandbox](https://projectnessie.org/guides/try-nessie/) ✅ — Nessie + MinIO в Docker.
- [Hive Quickstart](https://iceberg.apache.org/hive-quickstart/) ✅ — работа с Hive.

## Оптимизация

- [Партицирование и эволюция](https://subquery.ru/blog/courses/iceberg/partitioning-and-partition-evolution) — hidden partitioning и трансформации.
- [Кластеризация](https://subquery.ru/blog/courses/iceberg/clustering) — Z-ordering.
- [Метатаблицы](https://subquery.ru/blog/courses/iceberg/metadata-tables) — диагностика через SQL.
- [Обслуживание таблиц](https://subquery.ru/blog/courses/iceberg/table-maintenance) — компакция и гигиена.
- [Диагностика медленных запросов](https://subquery.ru/blog/iceberg-queries-speedup) — пять структурных причин.
- [Maintenance (доки)](https://iceberg.apache.org/docs/latest/maintenance/) ✅ — официальное руководство.
- [RisingWave: small files](https://risingwave.com/blog/iceberg-small-file-problem/) ✅ — проблема мелких файлов.
- [Dremio: компакция](https://www.dremio.com/blog/compaction-in-apache-iceberg-fine-tuning-your-iceberg-tables-data-files/) ⚠️ — тонкая настройка.

## Версионирование

- [Time travel и откат](https://subquery.ru/blog/courses/iceberg/timetravel-and-rollback) — версии таблицы и rollback.
- [Теги и ветки](https://subquery.ru/blog/courses/iceberg/tagging-and-branching) — Git-подобный workflow.
- [Branching and Tagging (доки)](https://iceberg.apache.org/docs/latest/branching/) ✅ — официальное описание.
- [Time Travel (справочник)](https://iceberglakehouse.com/iceberg/iceberg-time-travel/) ✅ — синтаксис в движках.

## Облака

| Платформа | Ресурс | Статус |
| --- | --- | --- |
| [Snowflake](https://docs.snowflake.com/en/user-guide/tables-iceberg) | Iceberg-таблицы в Snowflake | ⚠️ |
| [Google BigQuery](https://cloud.google.com/bigquery/docs/iceberg-tables) | Managed и внешние таблицы | ✅ |
| [AWS Athena](https://docs.aws.amazon.com/athena/latest/ug/querying-iceberg.html) | Запросы в AWS | ✅ |
| [Databricks](https://docs.databricks.com/gcp/en/iceberg/) | Iceberg в Unity Catalog | ✅ |
| [Microsoft Fabric OneLake](https://learn.microsoft.com/en-us/fabric/onelake/onelake-iceberg-tables) | Виртуализация Delta ↔ Iceberg | ✅ |
| [Cloudera](https://www.cloudera.com/open-source/apache-iceberg.html) | Open data lakehouse CDP | ✅ |
| [Лейкхаус Google](https://subquery.ru/blog/6-layer-lakehouse-from-google) | Разбор шести слоёв производительности | ✅ |
| [Borderless Lakehouse](https://cloud.google.com/blog/products/data-analytics/introducing-the-borderless-lakehouse) | Федерация каталогов | ✅ |

## Стриминг и инструменты

- [Kafka Connect](https://iceberg.apache.org/docs/latest/kafka-connect/) ✅ — запись событий в реальном времени.
- [Debezium → Iceberg](https://memiiso.github.io/debezium-server-iceberg/) ✅ — CDC из реляционных баз.
- [Apache Amoro](https://amoro.network) ✅ — автономная оптимизация таблиц.
- [apache/iceberg-rest-fixture](https://github.com/apache/iceberg-rest-fixture) ⚠️ — тестовый REST-каталог.

## Контент

- [DuckDB и Apache Iceberg](https://subquery.ru/blog/duckdb-iceberg) — лейкхаус без кластера.
- [Trino, DuckDB и Iceberg](https://subquery.ru/blog/iceberg-trino-duckdb) — практическая заметка.
- [Ryan Blue: A High-Performance Format](https://www.dremio.com/blog/iceberg-a-high-performance-format-for-huge-analytic-tables/) ⚠️ — статья создателя формата.
- [Архитектура под капотом](https://www.dremio.com/blog/apache-iceberg-an-architectural-look-under-the-covers/) ⚠️ — устройство формата.
- [Netflix: Iceberg и Spark](https://netflixtechblog.com/iceberg-and-spark-in-netflix-production-b5d9eaad927b) ⚠️ — опыт продакшена.
- [Iceberg Knowledge Base](https://iceberglakehouse.com/iceberg/) ✅ — справочник терминов.
- [The Definitive Guide](https://github.com/developer-advocacy-dremio/definitive-guide-to-apache-iceberg) ✅ — код примеров книги O'Reilly.
- [Talks и Iceberg Summit](https://iceberg.apache.org/talks/) ✅ — записи докладов.
- [YouTube @ApacheIceberg](https://www.youtube.com/@ApacheIceberg) ✅ — официальный канал.

## Сообщества

| Ресурс | Статус |
| --- | --- |
| [apache/iceberg (GitHub)](https://github.com/apache/iceberg) | ✅ |
| [Страница Community](https://iceberg.apache.org/community/) | ✅ |
| [Dev mailing list](https://lists.apache.org/list.html?dev@iceberg.apache.org) | ✅ |
| [Slack-приглашение](https://s.apache.org/iceberg-slack) | ✅ |
| [Тема iceberg на GitHub](https://github.com/topics/iceberg) | ✅ |
| [Telegram: Data Engineers](https://t.me/data_engineers) | ⚠️ |
| [Telegram: DataHub RU](https://t.me/datahub_ru) | ⚠️ |

## Как дополнить

Предложите ресурс через issue или pull request. Важно, чтобы ссылка была живой и по теме Apache Iceberg.