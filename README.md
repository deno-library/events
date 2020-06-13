# EventEmitter
EventEmitter for deno, API is the same as Nodejs, Have all the APIs of nodejs

Refer to [nodejs events documentation](https://nodejs.org/dist/latest-v12.x/docs/api/events.html#events_class_eventemitter)

## Useage
```ts
import EventEmitter from "https://deno.land/x/events@v1.0.0/mod.ts";

const ee = new EventEmitter();
ee.on("message", msg => {
  console.log(msg);
});
emitter.emit("message");
```  
extends
```ts  
import EventEmitter from "https://deno.land/x/events@v1.0.0/mod.ts";

class A extends EventEmitter {}
const a = new A();
a.on("message", msg => {
  console.log(msg);
});
a.emit("message");
```
