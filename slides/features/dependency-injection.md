### Dependency Injection

```
import {HttpClient} from 'aurelia-http-client';

export class Customer{
  static inject() [HttpClient];
  constructor(http){
    this.http = http;
  }
}
```
Or using decorators

```
import {inject} from 'aurelia-framework';
import {HttpClient} from 'aurelia-http-client';

@inject(HttpClient)
export class Customer{
  constructor(http){
    this.http = http;
  }
}
```