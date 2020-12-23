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
"scripts": {
    "dev": "cross-env NODE_ENV=development webpack-dev-server --open --hot",
    "build": "cross-env NODE_ENV=production webpack --progress --hide-modules",
    "test": "jest"
},
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

##### **Обновление webpack** Возможно эти версии пакетов по одиночке можно обновить вверх
```sh
$ yarn upgrade webpack@^4.29.5
$ yarn upgrade webpack-dev-server@^3.11.0
$ yarn add --dev webpack-cli@^4.2.0
$ yarn upgrade vue-loader@^15.6.4
>	Подключаем VueLoaderPlugin в webpack.config.js
>	const VueLoaderPlugin = require('vue-loader/lib/plugin')
>	plugins: [
		new VueLoaderPlugin(),
	],
$ yarn upgrade vue-template-compiler@^2.6.7
```

##### **Обновление всех зависимостей**
```sh
$ yarn outdated (осмотр устаревших зависимостей)
$ yarn upgrade --latest
$ или
$ yarn upgrade-interactive --latest
	"cross-env": "^5.0.5", > "^7.0.3" good
    "css-loader": "^0.28.7",
    "file-loader": "^1.1.11", > "^6.2.0" bad
    "node-sass": "^4.5.3",
    "sass-loader": "^6.0.6",
```
> https://classic.yarnpkg.com/ru/docs/cli/upgrade/

> https://classic.yarnpkg.com/ru/docs/cli/upgrade-interactive


##### **Добавление модульное(UNIX) тестирование компонентов  Vue Test Utils**
```sh
$ yarn add --dev @vue/test-utils jest vue-jest babel-jest @babel/core @babel/preset-env babel-core@^7.0.0-bridge.0
```
> https://vue-test-utils.vuejs.org/installation/#semantic-versioning

> В этой инструкции содержится описание настройки транспиллера babel (.babelrc file) так и тест-ранера jest (jest.config.js file)
> Сами же тесты складываются:
> 1) В папку components/__test__
> 2) либо хранятся в папке где находится сам компонент Vue



