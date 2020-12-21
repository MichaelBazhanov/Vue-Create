# Vue CLI, установка и обновление

> Устанавливаем, обновляем, дополняем.

#### Установка vue
```sh
$ vue init webpack-simple my-project
$ cd my-project
$ npm install
$ npm run dev
```

##### Обновление всех зависимостей
```sh
$ yarn upgrade --latest
$ или
$ yarn upgrade-interactive --latest
```
> https://classic.yarnpkg.com/ru/docs/cli/upgrade/

> https://classic.yarnpkg.com/ru/docs/cli/upgrade-interactive


##### Vue Test Utils
```sh
$ yarn add --dev @vue/test-utils vue-jest babel-jest @babel/core @babel/preset-env babel-core@^7.0.0-bridge.0
```
> https://vue-test-utils.vuejs.org/installation/#semantic-versioning

> В этой инструкции содержится описание настройки транспиллера babel (.babelrc file) так и тест-ранера jest (jest.config.js file)


