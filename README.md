# Bos Website

## Web Tech-Stack

- Vue
- CSS3

## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Run your tests

```
npm run test
```

### Lints and fixes files

```
npm run lint
```

### Project Structure

```
bos-website/
|-- public/              			# folder to store the static files
|   |-- styles/			            # folder to store the  static styles
|   |	|-- _global.css
|   |	|-- _reset.css
|   |	|-- _variables.css
|   |   |-- main.css
|   |   ...
|-- index.html              		# File to expose the vue entry point
|-- favicon.ico
|   ...
|-- src/      	        			# vue project folder
|   |-- assets/			            # folder to store the assets
|   |	|-- logo.png
|   |   ...
|   |-- components/			        # folder to store the project components
|   |   ...
|   |-- App.vue			            # file to build the vue app.
|   |-- main.js			            # file to retrieve the entry point from public/index.html
|   ...
`-- README.md
```

### Issues

- When run `npm run build`, the `/dist` folder is generated with a blank page.
  - _Solution:_ create the `vue.config.js` file with the next content:

```js
module.exports = {
  publicPath: ""
};
```

### Refs

- [Ashford-Ashford](http://ashford-ashford.com)
- [Anchor transition to the navigation menu](https://codepen.io/melnik909/pen/KGxdjY?editors=1100)

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).
