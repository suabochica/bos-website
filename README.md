# Bos Website

## Web Tech-Stack

- Hugo

### Compiles and hot-reloads for development

```
hugo serve
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
