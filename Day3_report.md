## Day3_report.md

# Day 3 Report — Lab 4.5.5 + Auto-check artifacts

## 1) Student
- Name: Serik Adil
- Group: ИБ-23-5б
- Token: D1-IB-23-5b-20-3E97
- Repo: https://github.com/adil3453/devnet-day1-IB-23-5B-Serik

## 2) Lab 4.5.5 completion evidence
- API docs (Try it out) screenshots: выполнены GET /books и другие запросы через API docs
- Postman screenshots: выполнены запросы GET /books, POST /loginViaBasic, POST /books
- Python run screenshot: выполнен скрипт `day3_library_lab.py` и запущен pytest

## 3) Artifacts checklist
- artifacts/day3/books_before.json: Yes
- artifacts/day3/books_sorted_isbn.json: Yes
- artifacts/day3/mybook_post.json: Yes
- artifacts/day3/books_by_me.json: Yes
- artifacts/day3/add100_report.json: Yes
- artifacts/day3/postman_collection.json: Yes
- artifacts/day3/postman_environment.json: Yes
- artifacts/day3/curl_get_books.txt: Yes
- artifacts/day3/curl_get_books_isbn.txt: Yes
- artifacts/day3/curl_get_books_sorted.txt: Yes
- artifacts/day3/summary.json: Yes

## 4) Command outputs (paste exact)
### 4.1 Script run
```text
python src/day3_library_lab.py --count 100
```
4.2 Tests
```
pytest -q
```
```
4 passed 100%
```
5) Problems & fixes (at least 1)

Problem:
В Postman запрос POST /books сначала возвращал ошибку валидации.

Fix:
Формат тела запроса был изменён с Text на JSON, после чего запрос начал выполняться корректно.

Proof:
После исправления были успешно созданы файлы ```mybook_post.json,``` ``` books_by_me.json``` и ```add100_report.json,``` а тест ```pytest -q``` прошёл успешно.
