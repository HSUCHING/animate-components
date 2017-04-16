# FAQs

### I want to change the element type
When you render the children elements under the animation component, it wraps them inside a `span` with **inline display** by default. To render a block level element instead of inline element, you can pass prop `block` to the component like this

```javascript
import React from 'react';

import { Entrance } from 'animate-components';

class App extends React.Component {
  render () {
    return (
      <Entrance duration="2s" block>
        <h1>Hello World!</h1>
      </Entrance>
    );
  }
}
```

This will give the output 

```html
<div data-reactroot style="position: relative; animation: joknde 3s ease 0s 1 normal none running; backface-visibility: visible;">
  <h1>Hello World!</h1>
</div>
```