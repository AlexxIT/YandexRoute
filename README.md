# Yandex Route

Идея [@andreypolyak](https://github.com/andreypolyak).

```yaml
sensor:
  - platform: yandex_route
    name: На машине
    points:
      - 37.553672,55.715702
      - 37.719112,55.744181
  - platform: yandex_route
    name: Пешком до работы
    points:
      - 37.618860,55.751418
      - 37.631274,55.747073
      - zone.work
    scan_interval: '00:01:00'
    params:
      type: pedestrian  # пешком
      #type: masstransit  # общ.транспорт
      #type: bicycle  # велосипед
      #type: auto  # автомобиль

zone:
  - name: Work
    latitude: 55.741907
    longitude: 37.620453
```