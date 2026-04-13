# Contribution


## Requirement

- [nodejs](https://nodejs.org/en/)


## Chrome 

1. Clone this repo:

```
git clone https://github.com/immersive-translate/immersive-translate.git
```

2. Install Dependencies

```bash
cd immersive-translate
npm install
```

3. Build

```
npm run build
```

4. Open Chrome Extension Manager `chrome://extensions`:

Load `dist/chrome`.

### Package for end users (download + import)

If you want to produce a downloadable package for users:

```bash
npm run chrome:package
```

Then send the generated file:

`dist/immersive-translate-chrome-unpacked-v<version>.zip`

User steps:

1. Download the zip and unzip it
2. Open `chrome://extensions`
3. Enable **Developer mode**
4. Click **Load unpacked**
5. Select the extracted `chrome` folder


## Dev

If you want to develope this project, Firefox is the best choice.


### Firefox

1. Download [Firefox](https://www.mozilla.org/en-US/firefox/new/)
2. Install [web-ext](https://extensionworkshop.com/documentation/develop/getting-started-with-web-ext/)

```bash
npm install --global web-ext
```

3. Start watch and develope:

```
make start
```

then, it will start firefox automatically, and you can now start development.


### Chrome 

If you want to develop with chrome, one more thing todo is you should download [watchexec](https://github.com/watchexec/watchexec)


```
brew install watchexec
```


and then run:

```
make watch
```

