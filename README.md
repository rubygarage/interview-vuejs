# Interview task (VueJS)

### Task

Develop a simple application which manages movie lists of users. App contains 3 user stories - view lists, create list and remove list.

### API
* Authentication - https://developers.themoviedb.org/3/getting-started/authentication
* Lists - https://developers.themoviedb.org/3/account/get-created-lists
* Create list - https://developers.themoviedb.org/3/lists/create-list
* Delete list - https://developers.themoviedb.org/3/lists/delete-list

### Tech stack
* Use JavaScript (ES6+)
* Use Vue
* Use Vuex to manage state of the app
* Code must be covered with unit-tests (at least business logic)
* Use any design library for UI (we have Vue Ant Design in boilerplate)
* Use any other libraries and frameworks to speed up development

### Notes
* Usage templates style for component creation is more preferable
* It is advisable to use scss
* Also advisable to use BEM for class names and style folder structure
* Imagine that this isn’t test task - this is a part of big product and you need to develop new functionality following architecture and code standards used in the team

### Boilerplate

To speed up setting up, configuration and development we prepared boilerplate with the next tech stack:

* vue
* vuex
* axios
* antd
* jest
* vue-testing-library

## Commands
```
yarn install
yarn serve
yarn build
yarn test:unit
```

Use this repository to create your own build if you need to add/modify something to solve a task.
