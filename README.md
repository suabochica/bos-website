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

### Publish process
After update the page and run the `npm run build` command:

1. Go to [cPanel](https://shared10.hostgator.co:2083/cpsess0840575723/frontend/hostgator_latam/filemanager/index.html)
2. Open the _File Manager_
3. Navigate to the `public_html` folder
4. If you change global styles, delete all the files from `public_html/styles` and upload all the files in `dist/styles`
5. If you change component styles, delete all the files from `public_html/css` and upload all the files in `dist/css`
6. If you change scripts, delete all the files from `public_html/js` and upload all the files in `dist/js`
7. Alway, replace the `public_html/index.html` file with `dist/index.html` file


### Refs

- [Ashford-Ashford](http://ashford-ashford.com)
- [Anchor transition to the navigation menu](https://codepen.io/melnik909/pen/KGxdjY?editors=1100)

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).
