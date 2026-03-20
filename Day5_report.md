# Day 5 Report — DevNet APIs + YANG + Packet Tracer + Webex

## 1) Student
- Name: Serik Adil
- Group: ИБ-23-5б
- Token: D1-IB-23-5b-20-3E97
- Repo: https://github.com/adil3453/devnet-day1-IB-23-5B-Serik

## 2) Lab completion evidence

### Packet Tracer (PT)
- Получены данные о сети через API
- Выполнены запросы к устройствам и хостам
- Проверен внешний доступ

### Webex API
- Получена информация о пользователе
- Создана комната
- Отправлено сообщение
- Получен список сообщений

### YANG / pyang
- Загружен модуль ietf-interfaces.yang
- Выполнена проверка через pyang
- Получено дерево структуры модели

## 3) Artifacts checklist

### Packet Tracer
- artifacts/day5/pt/hosts.json: Yes
- artifacts/day5/pt/network_devices.json: Yes
- artifacts/day5/pt/external_access_check.json: Yes
- artifacts/day5/pt/serviceTicket.txt: Yes
- artifacts/day5/pt/pt_internal_output.txt: Yes
- artifacts/day5/pt/postman_collection.json: Yes
- artifacts/day5/pt/postman_environment.json: Yes

### Webex
- artifacts/day5/webex/me.json: Yes
- artifacts/day5/webex/rooms_list.json: Yes
- artifacts/day5/webex/room_create.json: Yes
- artifacts/day5/webex/message_post.json: Yes
- artifacts/day5/webex/messages_list.json: Yes

### YANG
- artifacts/day5/yang/ietf-interfaces.yang: Yes
- artifacts/day5/yang/pyang_tree.txt: Yes
- artifacts/day5/yang/pyang_version.txt: Yes

### Summary
- artifacts/day5/summary.json: Yes

## 4) Command outputs (paste exact)

### 4.1 Script run
```text
python src/day5_module8.py
```
4.2 Summary builder
```
python src/day5_summary_builder.py
```
4.3 Tests
```
pytest -q
```
5) What I learned (3–6 bullets)

Научился работать с API Packet Tracer

Научился использовать Webex API (создание комнат и отправка сообщений)

Понял структуру YANG моделей

Научился использовать pyang для анализа моделей

Закрепил работу с JSON API и автоматизацией

6) Problems & fixes (at least 1)

Problem:
Некоторые API запросы сначала не возвращали ожидаемый результат.

Fix:
Проверил параметры запросов и формат данных, после чего скорректировал код.

Proof:
Все необходимые файлы в artifacts/day5 были успешно созданы, а тесты pytest -q прошли без ошибок.
