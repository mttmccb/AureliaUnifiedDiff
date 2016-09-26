### Custom Elements

simple-header.js
```javascript
  import {bindable} from 'aurelia-framework';
  export class SimpleHeaderCustomElement {
    @bindable text = '';
  }
```

simple-header.html
```html
<template>
  <div class="header">
    <h1 class="header-title">${text}</h1>
  </div>
</template>
```

```html
<template>
  <require from="./simple-header"></require>

  <simple-header text.bind="Hello!"></header>
</template>
```