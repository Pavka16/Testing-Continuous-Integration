## Домашнее задание к лекции «Unit-тестирование»
---
### Важные моменты
Каждая задача выполняется в виде отдельного проекта с собственным GitHub-репозиторием.

*ESLint* не должен выдавать ошибок.

*Jest* должен обеспечивать 100-процентное покрытие по строкам для тестируемых функций.

Ко всем задачам должен быть подключён *AppVeyor* и выставлен бейджик статуса.

Используйте *import/export*, а не *require*.
В качестве шаблона можете использовать [готовый проект](https://github.com/Pavka16/ajs-homeworks/tree/master/ci-template).

В личном кабинете на сайте [netology.ru](netology.ru) в поле комментария к домашней работе добавьте ссылки на ваши GitHub-проекты.

## Описание установки
---
```
npm init
# При инициалиализации в качестве тестовой команды указать:
# test command: jest --coverage
npm install --save-dev jest babel-jest @babel/core @babel/cli @babel/preset-env
npm install core-js@3
```
Не забудьте про *.babelrc* и *.browserslistrc*.


В *.babelrc*:
``` js
{
  "presets": [["@babel/preset-env", {
    "useBuiltIns": "usage",
    "corejs": 3
  }]]
}
```
Запуск тестов:
``` js
npm test
```
---

### [Чистые функции](git@github.com:Pavka16/pure-functions.git)
### [Matchers](git@github.com:Pavka16/matchers.git)
