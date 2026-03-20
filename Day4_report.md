## Day4_report.md

# Day 4 Report — Labs 6–7 (Docker + Jenkins + Security + Ansible)

## 1) Student
- Name: Serik Adil
- Group: ИБ-23-5б
- Token: D1-IB-23-5b-20-3E97
- Repo: https://github.com/adil3453/devnet-day1-IB-23-5B-Serik

## 2) Evidence checklist (files exist)
### Docker (6.2.7)
- artifacts/day4/docker/sampleapp_curl.txt: Yes
- artifacts/day4/docker/sampleapp_token_proof.txt: Yes
- artifacts/day4/docker/sampleapp_docker_ps.txt: Yes
- artifacts/day4/docker/sampleapp_build_log.txt: Yes

### Jenkins (6.3.6)
- artifacts/day4/jenkins/jenkins_docker_ps.txt: Yes
- artifacts/day4/jenkins/buildapp_console.txt: Yes
- artifacts/day4/jenkins/testapp_console.txt: Yes
- artifacts/day4/jenkins/pipeline_script.groovy: Yes
- artifacts/day4/jenkins/pipeline_console.txt: Yes
- artifacts/day4/jenkins/jenkins_url.txt: Yes

### Ansible (7.4.8)
- artifacts/day4/ansible/ansible_ping.txt: Yes
- artifacts/day4/ansible/ansible_hello.txt: Yes
- artifacts/day4/ansible/ansible_playbook_install.txt: Yes
- artifacts/day4/ansible/ports_conf_after.txt: Yes
- artifacts/day4/ansible/curl_apache_8081.txt: Yes

### Security (6.5.10)
- artifacts/day4/security/signup_v1.txt: Yes
- artifacts/day4/security/login_v1.txt: Yes
- artifacts/day4/security/signup_v2.txt: Yes
- artifacts/day4/security/login_v2.txt: Yes
- artifacts/day4/security/db_tables.txt: Yes
- artifacts/day4/security/db_user_hash_sample.txt: Yes

## 3) Commands output
```text
python src/day4_summary_builder.py
pytest -q
```
4) Short reflection (5–8 lines)

В ходе Day 4 были изучены Docker, Jenkins, Ansible и вопросы безопасности приложений.
Наиболее сложной частью была работа с Jenkins, так как нужно было сохранить pipeline script и console output.
Docker помог понять, как контейнеризовать приложение и проверять его через curl.
Ansible показал, как автоматизировать установку и настройку Apache.
Также была изучена разница между хранением паролей в открытом виде и в виде хеша.
В результате получилось собрать все evidence-файлы и пройти автоматическую проверку.

5) Problems & fixes (at least 1)

Problem:
В Day 4 отсутствовали некоторые evidence-файлы, из-за чего validation_passed был false.

Fix:
Недостающие файлы были созданы и заполнены, после чего summary был пересобран через python src/day4_summary_builder.py.

Proof:
После исправления в artifacts/day4/summary.json значение validation_passed стало true, а pytest -q прошёл успешно.


После этого просто:

```bash
nano Day1_report.md
nano Day2_report.md
nano Day3_report.md
nano Day4_report.md
```
Потом:

```git add Day1_report.md Day2_report.md Day3_report.md Day4_report.md```
```git commit -m "add reports day1-4"```
```git push```
