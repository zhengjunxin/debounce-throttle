# debounce-throttle

## 原因
只想简单使用 lodash 的 debounce 和 throttle 函数，但是 lodash 库显得太大了，分别下载 lodash.debounce 和 lodash.throttle 又有代码冗余，因为 lodash.throttle 内包含 lodash.debounce 的代码。所以利用[lodash-cli](https://lodash.com/custom-builds)定制了 debounce 和 throttle 函数。

## 引用
该定制为 UMD 的，所以支持多种引用方式

import 引入
``` javascript
import {debounce, throttle} from 'debounce-throttle'
```

require 引入
``` javascript
const {debounce, throttle} = require 'debounce-throttle'
```

定义在全局对象上
``` javascript
const {debounce, throttle} = window._
```

## 使用
具体使用见[lodash文档](https://lodash.com/docs/4.17.4)
