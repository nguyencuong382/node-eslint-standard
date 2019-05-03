# node-eslint-standard

## Overview

## Setup
### Setup plugins for visual code

1. Install [eslint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) to format code automatically based on .eslintrc file config.
2. (Optional) you may want to auto format code when save: File > Preferences > Settings, then choose Extensions > ESlint. Click "Auto Fix On Save"
3. (Optional) Install [prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) to format code automatically based on .prettierrc file config.

### Setup .eslintrc for project
1. Create file .eslintrc same directory with package.json. All of standard config for your code will be here.
2. Copy content of [.eslint](https://github.com/nguyencuong382/node-eslint-standard/blob/master/.eslintrc) file I created into the .eslintrc
3. Install package
```
npm install --save-dev eslint-config-loopback
```
4. Done! when you create some bad code, visual studion will alert error or warning. To fix this: **Ctrl + Shift + L**

### Modify file .eslintrc
We may have many different projects of javascript language (Vuejs, Reactjs, Nodejs,...), each project may has own standard eslint. Eslint also supports many types of standards: [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb), [eslint-config-google](https://www.npmjs.com/package/eslint-config-google), [eslint-config-loopback](https://www.npmjs.com/package/eslint-config-loopback), ...

If you want to follow, for example, eslint-config-airbnb standard:
1. Install package
```
npm install --save-dev eslint-config-airbnb
```
2. Modify file .eslintrc
```
{
  ...
  "extends": "airbnb",
  ...
}
```

## More documents
1. Loopback code style https://loopback.io/doc/en/contrib/style-guide-es6.html
2. Airbnb code style https://github.com/airbnb/javascript
3. Eslint standard rules https://eslint.org/docs/rules/
