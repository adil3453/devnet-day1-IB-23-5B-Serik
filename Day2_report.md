## Day2_report.md


# Day 2 Report — Git + Data Formats + Tests

## 1) Student
- Name: Serik Adil
- Group: ИБ-23-5б
- Token: D1-IB-23-5b-20-3E97
- Repo: https://github.com/adil3453/devnet-day1-IB-23-5B-Serik

## 2) NetAcad progress
- Module 2.2 done: Yes
- Module 3.1–3.6 done: Yes

## 3) Git evidence
- File `artifacts/day2/git_log.txt` exists: Yes
- File `artifacts/day2/conflict_log.txt` exists: Yes
- Conflict note (1–2 lines): Во время выполнения задания возник конфликт в README.md, который был исправлен вручную и успешно завершён merge commit.

## 4) Generated artifacts (Day2)
- normalized.json: Yes
- normalized.yaml: Yes
- normalized.xml: Yes
- normalized.csv: Yes
- summary.json: Yes

## 5) Commands output (paste EXACT output)
### 5.1 Generator
```text
python src/day2_data_formats.py --input artifacts/day1/response.json
```
5.2 Tests
```
pytest -q
```
```
4...passed
```
6) What I learned (3–6 bullets)

Научился работать с ветками Git.

Научился создавать Pull Request и делать merge.

Научился решать merge conflict.

Научился сохранять данные в форматах JSON, YAML, XML и CSV.

Научился проверять файлы через pytest.

7) Problems & fixes (at least 1)

Problem:
Во время работы с Git возник конфликт при слиянии веток.

Fix:
Конфликт в файле README.md был исправлен вручную, после чего был выполнен merge commit.

Proof (command/file):
Файлы ```artifacts/day2/conflict_log.txt``` и ```artifacts/day2/git_log.txt``` были успешно созданы, а merge завершился без ошибок.
