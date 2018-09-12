#
https://wanago.io/2018/08/27/testing-javascript-tutorial-types-of-tests-of-unit-testing-with-jest/

The test function runs a test.

## alias
it === test

```
const divide = require('./divide');
 
test('dividing 6 by 3 equals 2', () => {
  expect(divide(6, 3)).toBe(2);
});
```
https://jestjs.io/docs/en/expect#expectvalue


# debug

Runs less tets, hopefully only one.
```
npm test -t 'ComponentName.test.js'
```

https://airbnb.io/enzyme/docs/api/ShallowWrapper/debug.html

console.log(wrapper.debug());

## debug output
your markup
ex. <div>some text </div>
