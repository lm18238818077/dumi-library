## Toast

Demo:

```tsx
import React from 'react';
import { Toast } from 'dumi-library';

export default () => {
  const handle = (type) => {
    Toast[type](type);
  };
  return (
    <div>
      <button onClick={handle.bind(this, 'fail')}>fail</button>
      <button onClick={handle.bind(this, 'info')}>info</button>
      <button onClick={handle.bind(this, 'success')}>success</button>
      <button onClick={handle.bind(this, 'loading')}>loading</button>
      <button onClick={handle.bind(this, 'hide')}>hide</button>
    </div>
  );
};
```
