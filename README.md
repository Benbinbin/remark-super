# remark-super
This is a remark plugin to transform `^text^` into a `<sup>text</sup>` element.

## Install

```bash
npm install remark-super
```

## Usage

```js
import {remark} from 'remark';
import remarkSuper from 'remark-super';

const doc = 'This is a ^superscript^';
remark().use(remarkSuper).process(doc).then(file => {
    console.log(String(file));
    // => This is a <sup>superscript</sup>
});
```

## License
[MIT](./LICENSE)