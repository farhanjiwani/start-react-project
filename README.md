# `start-react-project` v0.1.0

Just a quick way to start a [React](https://reactjs.org/) project without using `create-react-app`.

## Install

```bash
yarn
yarn start
```

### (_Optional_) Add SASS

Add required packages:

```bash
yarn add -D node-sass sass-loader
```

Update `webpack.config.js`:

```js
module: {
    rules: [
        {
            test: /\.s?css$/,
            use: [
                "style-loader", //3. Inject styles into DOM
                "css-loader",   //2. Turns CSS into commonjs
                "sass-loader"   //1. Turns SCSS into CSS
            ]
        }
    ];
}
```

## What's In It

- [HTML5 Boilerplate v7.3](https://html5boilerplate.com/)
- npm modules:
  - (Instructions: [Create React App From Scratch](https://github.com/farhanjiwani/dev-notes/blob/master/react/React-From_Scratch.md))

  - ```json
    "devDependencies": {
        "@babel/cli": "^7.8.4",
        "@babel/core": "^7.8.6",
        "@babel/preset-env": "^7.8.6",
        "@babel/preset-react": "^7.8.3",
        "babel-loader": "^8.0.6",
        "css-loader": "^3.4.2",
        "react": "^16.13.0",
        "react-dom": "^16.13.0",
        "style-loader": "^1.1.3",
        "webpack": "^4.41.6",
        "webpack-cli": "^3.3.11",
        "webpack-dev-server": "^3.10.3"
    },
    "dependencies": {
        "react-hot-loader": "^4.12.19"
    }
    ```
