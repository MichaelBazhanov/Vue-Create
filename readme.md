# Vue CLI, установка и обновление

> Устанавливаем, обновляем, дополняем.

#### **Установка vue**
```sh
$ vue init webpack-simple my-project
$ cd my-project
$ npm install
$ npm run dev
```

##### **Обновление Vue**
```sh
$ yarn upgrade vue@^2.6.12
```

##### **Обновление package.json**
```sh
"browserslist": [
	"> 1%",
	"last 2 versions",
	"not dead"
],
```

##### **Обновление Babel**
```sh
$ Замена старого написания на новое, плюс доп (удалить из package.json)
	"babel-core": "^6.26.0",
	"babel-preset-env": "^1.6.0",
	"babel-preset-stage-3": "^6.24.1",
$ yarn add --dev babel-loader @babel/core @babel/preset-env @babel/plugin-syntax-dynamic-import @babel/plugin-transform-runtime

```
##### **Обновление .babelrc**
```sh
{
	"presets": [
		"@babel/preset-env"
	],
	"plugins": [
		"@babel/plugin-transform-runtime",
		"@babel/plugin-syntax-dynamic-import"
	]
}
```

##### **Обновление webpack**
```sh
$ yarn upgrade webpack@^4.29.5       1
$ yarn upgrade webpack@^3.11.0       2
$ yarn add --dev webpack-cli@^4.2.0  3
```

##### **Обновление всех зависимостей**
```sh
$ yarn outdated (осмотр устаревших зависимостей)
$ yarn upgrade --latest
$ или
$ yarn upgrade-interactive --latest
```
> https://classic.yarnpkg.com/ru/docs/cli/upgrade/

> https://classic.yarnpkg.com/ru/docs/cli/upgrade-interactive


##### **Vue Test Utils**
```sh
$ yarn add --dev @vue/test-utils vue-jest babel-jest @babel/core @babel/preset-env babel-core@^7.0.0-bridge.0
```
> https://vue-test-utils.vuejs.org/installation/#semantic-versioning

> В этой инструкции содержится описание настройки транспиллера babel (.babelrc file) так и тест-ранера jest (jest.config.js file)


