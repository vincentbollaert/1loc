~~~ javascript
const isFunction = v => ['[object Function]', '[object GeneratorFunction]', '[object AsyncFunction]', '[object Promise]'].includes(Object.prototype.toString.call(v));

// Example
isFunction(function() {});          // true
isFunction(function*() {});         // true
isFunction(async function() {});    // true
~~~
