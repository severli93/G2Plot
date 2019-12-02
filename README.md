# G2Plot

> A charting library based on the Grammar of Graphics.

English | [简体中文](./README.zh-CN.md)

[![Version](https://badgen.net/npm/v/@antv/g2plot)](https://www.npmjs.com/@antv/g2plot)
[![NPM downloads](http://img.shields.io/npm/dm/@antv/g2plot.svg)](http://npmjs.com/@antv/g2plot)
![Latest commit](https://badgen.net/github/last-commit/antvis/g2plot)

`G2Plot` is an interactive and responsive charting library. Based on [the grammar of graphics](https://github.com/antvis/g2), G2Plot enables users to easily generate high-quality statistical charts through a few lines of code.

Moreover, combining with [AntV design principles](https://antv.vision/en/docs/specification/principles/basic), G2Plot provides standard and elegant visual styles as well to serve better user experience.

<img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*MjhQQLsbWeQAAAAAAAAAAABkARQnAQ" width="200"><img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*CkSoSpPfWQMAAAAAAAAAAABkARQnAQ" width="200"><img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*ZYmtSqcNDtkAAAAAAAAAAABkARQnAQ" width="200"><img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*gV_JQZVbDWAAAAAAAAAAAABkARQnAQ" width="200">

## Features

### 📦 elegant charts out of box

G2Plot is powered by a professional design-dev team for enterprise-class products. It not only provides elegant visual styles by the visualization design principles, but also equips with the best config-options for each chart by default.

Even though you are not an expert in data visualization, you still can create elegant charts through a few lines of code.

<img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*rqI2Qqt0pTwAAAAAAAAAAABkARQnAQ" width="600" />

### 📊 responsive layout

The responsive ability of G2Plot guarantees the legibility and great information density in any display size and data status.

<img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*ifK1TLi_4WoAAAAAAAAAAABkARQnAQ" width="600" />

### 📚story-telling dashboard

The concept of layers, in G2Plot, provides the possibilities of multi-chart storytelling through the overlapping, combination and connection mode of charts. In addition, G2Plot is exploring the technique of enriching the visual expressiveness of charts, such as transferring traditional statistical charts to more creative infographics.

<img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*gd00QaD9110AAAAAAAAAAABkARQnAQ" width="600" />

## Installation

```bash
$ npm install @antv/g2plot
```

## Usage

<img src="https://gw.alipayobjects.com/mdn/rms_d314dd/afts/img/A*37siRJftYDIAAAAAAAAAAABkARQnAQ" width="450">

```html
<div id="container"></div>
```

```js
import { Bar } from '@antv/g2plot';

const data = [
  { year: '1951 年', sales: 38 },
  { year: '1952 年', sales: 52 },
  { year: '1956 年', sales: 61 },
  { year: '1957 年', sales: 145 },
  { year: '1958 年', sales: 48 },
];

const bar = new Bar(document.getElementById('container'), {
  data,
  xField: 'sales',
  yField: 'year',
  colorField: 'year',
});

bar.render();
```

## Development

```bash
$ npm install

# run test case
$ npm run test

# run demos
$ npm start
```

## How to Contribute

Please let us know if you have any question and feedback. Check out [issues](https://github.com/antvis/g2plot/issues) for bug reports or suggestions first.

To become a contributor, please follow our [contributing guide](https://github.com/antvis/g2plot/blob/master/CONTRIBUTING.md).

## License

MIT
