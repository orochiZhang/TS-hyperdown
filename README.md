# TS-hyperdown
SegmentFault / HyperDown.js TypeScript version
SegmentFault / HyperDown.js的TypeScript版本

## Getting Started
```javascript
npm install ts-hyperdown
```
use in Angular4
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


