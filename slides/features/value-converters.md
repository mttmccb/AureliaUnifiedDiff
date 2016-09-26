### Value Converters

```javascript
  import moment from 'moment';

  export class DateFormatValueConverter {
    toView(value, format) {
      return moment(value).format(format);
    }
  }
```

```html
<template>
  <require from="./date-format"></require>

  ${currentDate | dateFormat:'M/D/YYYY h:mm:ss a'} <br/>
  ${currentDate | dateFormat:'MMMM Mo YYYY'} <br/>
  ${currentDate | dateFormat:'h:mm:ss a'}
</template>
```