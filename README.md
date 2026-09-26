# clickhouse-role

Устанавливает ClickHouse из официальных `.deb`-пакетов и создаёт БД.

## Переменные

| Переменная | Значение по умолчанию |
|---|---|
| `clickhouse_version` | `22.3.3.44` |
| `clickhouse_database` | `logs` |
| `clickhouse_deb_arch` | `amd64` |

## Использование

```yaml
- hosts: clickhouse
  become: true
  roles:
    - clickhouse-role
