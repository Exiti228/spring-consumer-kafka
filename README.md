# Быстрый старт
В микросервисе происходит получения сообщения из Kafka. Сообщение сохраняется в базу данных, для удобства h2, но можно выбрать любую другую.
## API
```http
GET http://URL:8080/metrics
```
## Формат ответа
```JSON
[
  {
    "id": 1,
    "metricsName": "asd",
    "metrics": [
      {
        "id": 1,
        "usedTimeMs": 0,
        "usedMemoryMb": 0,
        "serviceName": "dddddd",
        "wasError": false
      },
      {
        "id": 2,
        "usedTimeMs": 0,
        "usedMemoryMb": 0,
        "serviceName": "dddddd",
        "wasError": false
      }
    ]
  },
  {
    "id": 2,
    "metricsName": "asd",
    "metrics": [
      {
        "id": 3,
        "usedTimeMs": 0,
        "usedMemoryMb": 0,
        "serviceName": "dddddd",
        "wasError": false
      },
      {
        "id": 4,
        "usedTimeMs": 0,
        "usedMemoryMb": 0,
        "serviceName": "dddddd",
        "wasError": false
      }
    ]
  }
]
```
## API
```http
GET http://URL:8080/metrics/{metricsName}
```
## Формат ответа
```JSON
[
  {
    "id": 1,
    "metricsName": "asd",
    "metrics": [
      {
        "id": 1,
        "usedTimeMs": 0,
        "usedMemoryMb": 0,
        "serviceName": "dddddd",
        "wasError": false
      },
      {
        "id": 2,
        "usedTimeMs": 0,
        "usedMemoryMb": 0,
        "serviceName": "dddddd",
        "wasError": false
      }
    ]
  }
]
```