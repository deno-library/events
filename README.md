# EventEmitter
EventEmitter for deno, API is the same as Nodejs, Have all the APIs of nodejs

## Doc
```
https://nodejs.org/dist/latest-v12.x/docs/api/events.html#events_class_eventemitter
```

## Useage
```ts
import EventEmitter from "https://deno.land/x/events/mod.ts";

// class
class A extends EventEmitter {}
const a = new A();
a.on("message", msg => {
  console.log(msg);
});
a.emit("message");

// or
const ee = new EventEmitter();
ee.on("message", msg => {
  console.log(msg);
});
emitter.emit("message");
```