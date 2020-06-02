# EventEmitter
EventEmitter for deno, API is the same as Nodejs, Have all the APIs of nodejs

## Useage
```ts
import EventEmitter from "https://deno.land/x/events/mod.ts";
// or
import EventEmitter from "https://raw.githubusercontent.com/fuxingZhang/deno-EventEmitter/master/mod.ts";

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