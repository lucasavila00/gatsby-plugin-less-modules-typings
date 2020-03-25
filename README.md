# gatsby-plugin-less-modules-typings

A Gatsby plugin that provides typings for less modules.

The reason this plugin is created is because the ones that are already out there, have multiple problems, for example not working with newer versions of Gatsby, or transforming ALL less files regardless of if they're modules or not.

Based on [https://github.com/RobertMenke/gatsby-transformer-typescript-css-modules](https://github.com/RobertMenke/gatsby-transformer-typescript-css-modules)

## Install

```sh
npm i gatsby-plugin-less-modules-typings
```

Then add the plugin to your `gatsby-config.js` file:

```js
plugins: [
  // ...
  "gatsby-plugin-less-modules-typings",
]
```

Now you can import styles normally in TypeScript:

```ts
import * as styles from "./my.module.less"
```

:warning: This plugin **only** creates typings for LESS Modules, meaning files which names are ending with `.module.less`.

## License

[MIT License](LICENSE)
