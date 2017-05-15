# debounce-throttle

debounce-throttle 是利用[lodash-cli](https://lodash.com/custom-builds)定制的只包含 debounce 和 throttle 函数的库。

## 原因
在使用 lodash 库的节流函数时，感觉有 2 个问题不太友好，所以定制了只包含 debounce 和 throttle 函数的库，方便自己使用。

- 文件大小问题：无论是下载 lodash 还是分别下载 lodash.debounce, lodash.throttle 都有代码冗余。因为 lodash.throttle 是用 lodash.debounce 实现的，分别下载 lodash.debounce, lodash.throttle 相当于下载了 2 份代码！
- 模块化问题：lodash.debounce 和 lodash.throttle 只支持CMD。

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
