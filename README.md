# CI-CD._-04
CI/CD._Семинар 04


Сделать локальный шаблон CI и отдельный репозиторий с шаблонами, подключить их к своему основному репозиторию через include?


Создан локальный файл local-smoke-tests.gitlab-ci.yml

smoke-test-job:
  script: echo "SMOKE"

  Создан основной файл

  include:
  - local: local-smoke-tests.gitlab-ci.yml
- remote: https://gitlab.com/ci-cd7655047/5/-/raw/main/remote-included-file.yml
