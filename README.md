# Get colors from string

[![Greenkeeper badge](https://badges.greenkeeper.io/xcatliu/get-colors-from-string.svg)](https://greenkeeper.io/)


Get colors from string, supported color styles:

- Regular HEX color: `#000`, `#f2f2f2`
- rgb, rgba, hsl, hsla: `rga(120, 120, 120)`, `hsla(240,100%,50%,0.05)`
- Named color: `red`, `yellow`

## Getting Started

```bash
npm install get-colors-from-string --save
```

### Usage

```js
import getColorsFromString from 'get-colors-from-string';

const exampleString = `
body {
  background: white;
  color: #333;
}

h1 {
  background: rgba(0, 0, 0, 0.3);
  color: #333;
}
`;

console.log(getColorsFromString(exampleString));
// [ "#333", "rgba(0, 0, 0, 0.3)", "white" ]
```
