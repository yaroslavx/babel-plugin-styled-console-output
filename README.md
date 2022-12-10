# babel-plugin-styled-console-output

## Usage

```js
const babelPluginStyledConsoleOutput = require('babel-plugin-styled-console-output');

console.log('oh', 'yeah!');
console.error('oh', 'no');
```

.babelrc / babel.config.json

```js
{
  "plugins": [
    // ...
    [
      "module:babel-plugin-styled-console-output",
      {
        "types": {
          "error": { "color": "royalblue", "background": "#fafafa", "divider": "$" },
          "log": {
            "border": "1px solid royalblue ",
            "font-weight": "500",
            "padding": "11px"
          }
        }
      }
    ]
  ]
}
```

outputs

```
oh yeah! // but styled
oh$no // but styled
```

## API

```js
const babelPluginStyledConsoleOutput = require('babel-plugin-styled-console-output');
```

See [api_formatting.md](api_formatting.md) for tips.

## Install

With [npm](https://npmjs.org/) installed, run

```
$ npm install babel-plugin-styled-console-output
```

## Acknowledgments

babel-plugin-styled-console-output was inspired by..

## License

MIT
