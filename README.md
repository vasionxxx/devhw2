# Домашнее задание к занятию "GitLab" - BodarevVV
№ Задание №1
# Развернем GitLab и войдем в него для проверки
![alt text](https://github.com/vasionxxx/devhw2/blob/main/gitlab/1.jpg)

# Зарегистрируем gitlab-runner. Скриншот runner в проекте
![alt text](https://github.com/vasionxxx/devhw2/blob/main/gitlab/2.jpg)

# № Задание №2
# Создадим .gitlab-ci.yml
 image: node:latest

 stages:
  - build
  - test

 cache:
  key: ${CI_COMMIT_REF_SLUG}
  paths:
    - node_modules/

 install_dependencies:
  stage: build
  script:
    - npm ci

 lint:
  stage: test
  script:
    - npm run lint

 unit_tests:
  stage: test
  script:
    - npm run test

# Скриншот собранной сборки
![alt text](https://github.com/vasionxxx/devhw2/blob/main/gitlab/3.jpg)
