## Simple Electron React Boilerplate

This is a simple boilerplate to get up and running with Electron and React. It is a customized version of [Alex Devero's](https://github.com/alexdevero/electron-react-webpack-boilerplate) repo and was created by Brad Traversy

### Install

#### Clone this repo

```
git clone https://github.com/sarstuff/simple-electron-react.git
```

#### Install dependencies

```
npm install
```

or

```
yarn
```

### Usage

#### Run the app

```
npm run start
```

or

```
yarn start
```

#### Build the app (automatic)

```
npm run package
```

or

```
yarn package
```

#### when building on Mac,
there can be build problems with Catalina and 32bit apps
````
brew upgrade wine, make sure "/usr/local/bin/wine64" exist
rm -rf ~/.wine
edit "node_modules/rcedit/lib/rcedit.js", change "wine" to "wine64" at line 42
download "https://github.com/electron/rcedit/releases/download/v1.1.1/rcedit-x64.exe", rename to "rcedit.exe" and replace "node_modules/rcedit/bin/rcedit.exe"
````
#### Test the app (after `npm run build` || `yarn run build`)

```
npm run prod
```

```
yarn prod
```

### Change app title

Change the app title in the **webpack.build.config.js** and the **webpack.dev.config.js** files
