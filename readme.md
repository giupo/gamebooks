# [Project Aon Gamebooks](https://gamebooks.indecorous.tk/)

Desktop and mobile apps for the [1980s game books by Joe Dever](https://www.projectaon.org/en/Main/Home). The apps keep track of players' progress, and saves their statistics and items as they read through the choose-your-own-adventure titles.

## Built with

[Angular](https://angular.io/)
[Ionic](https://ionicframework.com/)
[Electron](https://electronjs.org/)

## Showcase

[iOS](https://appetize.io/app/w7ee7nz5c3q9mkt74heb0z1dt0)

## Setup

### Install [Node](https://nodejs.org/)

### Install dependencies

```shell
npm install -g cordova
npm install -g ionic
npm install
```

## Run

Dev:
```shell
npm run start --livereload
```

Browser:
```shell
ionic cordova run browser
```

iOS:
```shell
ionic cordova run ios --livereload
```

Android:
```shell
ionic cordova run android --livereload
```

Desktop:
```shell
ionic cordova run electron
```

### Build

#### Browser, iOS and Android:
```shell
ionic cordova build --prod --release browser
ionic cordova build --prod --release ios
ionic cordova build --prod --release android
```

#### Windows, macOS and Linux:
```shell
ionic cordova build --prod --release electron
```

```shell
electron-builder build --mac --project=platforms/electron/www -c.directories.buildResources=resources
electron-builder build --windows project=platforms/electron/www -c.directories.buildResources=resources
electron-builder build --linux project=platforms/electron/www -c.directories.buildResources=resources
```

--

@todo: Deploy to Heroku: https://github.com/heroku/heroku-buildpack-static
@todo: Release code to GitHub
@todo: Update forum "This has been rewritten and re-released to include all the Lone Wolf, Grey Star and Freeway Warrior titles, here."