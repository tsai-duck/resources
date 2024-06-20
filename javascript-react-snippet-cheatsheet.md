# JS + React Snippets

### Javascript

|  Prefix | Method                                              |
| ------: | --------------------------------------------------- |
|  `imp→` | `import moduleName from 'module'`                   |
|  `imn→` | `import 'module'`                                   |
|  `imd→` | `import { destructuredModule } from 'module'`       |
|  `ime→` | `import * as alias from 'module'`                   |
|  `ima→` | `import { originalName as aliasName} from 'module'` |
|  `exp→` | `export default moduleName`                         |
|  `exd→` | `export { destructuredModule } from 'module'`       |
|  `exa→` | `export { originalName as aliasName} from 'module'` |
|  `enf→` | `export const functionName = (params) => { }`       |
|  `edf→` | `export default (params) => { }`                    |
| `ednf→` | `export default function functionName(params) { }`  |
|  `met→` | `methodName = (params) => { }`                      |
|  `fre→` | `arrayName.forEach(element => { }`                  |
|  `fof→` | `for(let itemName of objectName { }`                |
|  `fin→` | `for(let itemName in objectName { }`                |
| `anfn→` | `(params) => { }`                                   |
|  `nfn→` | `const functionName = (params) => { }`              |
|  `dob→` | `const {propName} = objectToDescruct`               |
|  `dar→` | `const [propName] = arrayToDescruct`                |
|  `sti→` | `setInterval(() => { }, intervalTime`               |
|  `sto→` | `setTimeout(() => { }, delayTime`                   |
| `prom→` | `return new Promise((resolve, reject) => { }`       |
| `cmmb→` | `comment block`                                     |

<div style="page-break-after: always;"></div>

<table>
</tr>
<tr width="100%">
<td width="33%" valign="top">

### `desc`

```javascript
describe('$1', () => {
  $2
})
```

</td>
<td width="33%" valign="top">

### `test`

```javascript
test('should $1', () => {
  $2
})
```

</td>
<td width="33%" valign="top">

### `tit`

```javascript
it('should $1', () => {
  $2
})
```

</td>
</tr>
</table>

### `stest`

```javascript
import React from 'react'
import renderer from 'react-test-renderer'

import { $1 } from '../$1'

describe('<$1 />', () => {
  const defaultProps = {}
  const wrapper = renderer.create(<$1 {...defaultProps} />)

  test('render', () => {
    expect(wrapper).toMatchSnapshot()
  })
})
```

### `srtest`

```javascript
import React from 'react'
import renderer from 'react-test-renderer'
import { Provider } from 'react-redux'

import store from 'src/store'
import { $1 } from '../$1'

describe('<$1 />', () => {
  const defaultProps = {}
  const wrapper = renderer.create(
    <Provider store={store}>
      <$1 {...defaultProps} />)
    </Provider>,
  )

  test('render', () => {
    expect(wrapper).toMatchSnapshot()
  })
})
```

<div style="page-break-after: always;"></div>

# JS + React Snippets

### Console

| Prefix | Method                                                      |
| ------ | ----------------------------------------------------------- |
| `clg→` | `console.log(object)`                                       |
| `clo→` | ``console.log(`object`, object) ``                          |
| `clj→` | ``console.log(`object`, JSON.stringify(object, null, 2)) `` |
| `ctm→` | ``console.time(`timeId`) ``                                 |
| `cte→` | ``console.timeEnd(`timeId`) ``                              |
| `cas→` | `console.assert(expression,object)`                         |
| `ccl→` | `console.clear()`                                           |
| `cco→` | `console.count(label)`                                      |
| `cdi→` | `console.dir`                                               |
| `cer→` | `console.error(object)`                                     |
| `cgr→` | `console.group(label)`                                      |
| `cge→` | `console.groupEnd()`                                        |
| `ctr→` | `console.trace(object)`                                     |
| `cwa→` | `console.warn`                                              |
| `cin→` | `console.info`                                              |

<div style="page-break-after: always;"></div>

# JS + React Snippets

### React

|      Prefix | Method                                                                      |
| ----------: | --------------------------------------------------------------------------- |
|      `imr→` | `import React from 'react'`                                                 |
|     `imrd→` | `import ReactDOM from 'react-dom'`                                          |
|     `imrc→` | `import React, { Component } from 'react'`                                  |
|    `imrpc→` | `import React, { PureComponent } from 'react'`                              |
|     `imrm→` | `import React, { memo } from 'react'`                                       |
|     `imrr→` | `import { BrowserRouter as Router, Route, NavLink} from 'react-router-dom'` |
|     `imbr→` | `import { BrowserRouter as Router} from 'react-router-dom'`                 |
|    `imbrc→` | `import { Route, Switch, NavLink, Link } from react-router-dom'`            |
|    `imbrr→` | `import { Route } from 'react-router-dom'`                                  |
|    `imbrs→` | `import { Switch } from 'react-router-dom'`                                 |
|    `imbrl→` | `import { Link } from 'react-router-dom'`                                   |
|   `imbrnl→` | `import { NavLink } from 'react-router-dom'`                                |
|     `imrs→` | `import React, { useState } from 'react'`                                   |
|    `imrse→` | `import React, { useState, useEffect } from 'react'`                        |
|    `redux→` | `import { connect } from 'react-redux'`                                     |
| `rcontext→` | `const $1 = React.createContext()`                                          |

<div style="page-break-after: always;"></div>

# JS + React Snippets

### React Hooks

|               Prefix | Method                                             |
| -------------------: | -------------------------------------------------- |
|    `useStateSnippet` | `const [$1, set$1] = useState($2)`                 |
|  `useReducerSnippet` | `const [state, dispatch] = useReducer($1, $2, $3)` |
|  `useContextSnippet` | `const $1 = useContext($2)`                        |
|     `useMemoSnippet` | `useMemo(() => $1, [$2])`                          |
| `useCallbackSnippet` | `useCallback(() => { $1 }, [$2],)`                 |
|      `useRefSnippet` | `const $1 = useRef($2)`                            |
|   `useEffectSnippet` | `useEffect(() => { $1 return () => { $2 }}, [$3])` |

### Redux

|       Prefix | Method                    |
| -----------: | ------------------------- |
|  `rxaction→` | `redux action template`   |
|   `rxconst→` | `export const $1 = '$1'`  |
| `rxreducer→` | `redux reducer template`  |
|  `rxselect→` | `redux selector template` |
|   `rxslice→` | `redux slice template`    |

<div style="page-break-after: always;"></div>

# JS + React Snippets

### React Components

_TypeScript_ has its own components and snippets. Just prepend `ts`,
ie. `tsrcc`

<table width="200px">
<tr width="100%">
<td width="50%" valign="top">

### `rfc`

```javascript
import React from 'react'

export default function $1() {
  return <div>$0</div>
}
```

</td>
<td width="50%" valign="top">

### `rfce`

```javascript
import React from 'react'

function $1() {
  return <div>$0</div>
}

export default $1
```

</td>
</tr>
<tr width="100%">
<td width="50%" valign="top">

### `rafc`

```javascript
import React from 'react'

export const $1 = () => {
  return <div>$0</div>
}
```

</td>
<td width="50%" valign="top">

### `rafce`

```javascript
import React from 'react'

const $1 = () => {
  return <div>$0</div>
}

export default $1
```

</td>
</tr>
<tr width="100%">
<td width="50%" valign="top">

### `rmc`

```javascript
import React, { memo } from 'react'

export default memo(function $1() {
  return <div>$0</div>
})
```
</td>
<td width="50%" valign="top">
</td>
</tr>
</table>

<div style="page-break-after: always;"></div>

# JS + React Snippets

### HOC

### `hocredux`

```javascript
import React from 'react'
import PropTypes from 'prop-types'
import { connect } from 'react-redux'

export const mapStateToProps = (state) => ({})

export const mapDispatchToProps = {}

export const $1 = (WrappedComponent) => {
  const hocComponent = ({ ...props }) => <WrappedComponent {...props} />

  hocComponent.propTypes = {}

  return hocComponent
}

export default (WrapperComponent) =>
  connect(mapStateToProps, mapDispatchToProps)($1(WrapperComponent))
```

### `hoc`

```javascript
import React from 'react'
import PropTypes from 'prop-types'

export default (WrappedComponent) => {
  const hocComponent = ({ ...props }) => <WrappedComponent {...props} />

  hocComponent.propTypes = {}

  return hocComponent
}
```

<div style="page-break-after: always;"></div>

# JS + React Snippets

### Redux Components

### `rfcredux`

```javascript
import React, { Component } from 'react'
import { connect } from 'react-redux'

export const FileName = () => {
  return <div>$4</div>
}

const mapStateToProps = (state) => ({})

const mapDispatchToProps = {}

export default connect(mapStateToProps, mapDispatchToProps)(FileName)
```

### `reduxmap`

```javascript
const mapStateToProps = (state) => ({})

const mapDispatchToProps = {}
```

