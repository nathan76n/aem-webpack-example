# Webpack folder

Copy the two Webpack folders into your project:

- `webpack.core` contains basic configurations for npm, Webpack, Babel and Jest. Our goal for further development of this project is to allow you to update this folder without having to manually configure it again.
- `webpack.project` is meant to contain your project-specific configuration. It allows you to override and extend certain parts of `webpack.core`. Check out [the folder's index.js](./webpack.project/index.js) for more details.

# .gitignore

A .gitignore file should be added to the project so the files generated by Webpack are not version-controlled. Nobody should ever modify them directly, so you don't have to track them in Git.

```
**/webpack.bundles/*.bundle.*
```

# .browserslistrc

Tools such as Autoprefixer and Stylelint can use a shared configuration file with a list of browsers. An example is included here.
