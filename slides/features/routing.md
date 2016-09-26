### Routing

```
export class App {
  configureRouter(config, router){
    config.title = 'Aurelia';
    config.map([
      { route: ['','welcome'], name: 'welcome', moduleId: './welcome', nav: true, title:'Welcome' },
      { route: 'todos', name: 'todolist', moduleId: './todos/todolist', nav: true },
      { route: 'details', name: 'details', moduleId: './todos/details' }
    ]);

    this.router = router;
  }
}
```

- Child Routing
- Dynamic Routing
- Custom navigation pipeline (filter, auth)