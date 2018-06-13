# TS-hyperdown
[SegmentFault / HyperDown.js](https://github.com/SegmentFault/HyperDown.js) TypeScript version and ES6 version

SegmentFault / HyperDown.js的TypeScript版本和ES6版本

## Getting Started
```javascript
npm install ts-hyperdown
```
**use in Angular4**
```javascript
import { Parser } from 'TS-hyperdown';
```

```javascript
export class CreateComponent implements OnInit {

  parser = new Parser;

  constructor() { }

  ngOnInit() {
    console.log(this.parser.makeHtml("### hello world"));
  }

}
```

But,TypeScript version can't work in Angular5 and up which I have no idea to solve it.

You can use ES6 version in Angular5 and up

**use in Angular5 and up**
```javascript
import { Parser } from 'TS-hyperdown/parser';
```

```javascript
export class CreateComponent implements OnInit {

  parser = new Parser;

  constructor() { }

  ngOnInit() {
    console.log(this.parser.makeHtml("### hello world"));
  }

}
```

**use in Vue**
```javascript
import { Parser } from "ts-hyperdown/parser";

export default {
  name: "HelloWorld",
  mounted() {
    this.test();
  },
  methods: {
    test() {
      let parser = new Parser();
      console.log(parser.makeHtml("### hello world"));
    }
  }
};
```
