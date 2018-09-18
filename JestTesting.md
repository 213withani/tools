# Intro
https://wanago.io/2018/08/27/testing-javascript-tutorial-types-of-tests-of-unit-testing-with-jest/

The test function runs a test.
```
const toDoList = shallow(<ToDoList tasks={[]}/>);
* expect(app.containsMatchingElement(<h1>Hello world!</h1>)).toEqual(true);
* expect(toDoList).toContainReact(<ul/>);
* expect(toDoList.find('li').length).toEqual(0);

const toDoList = shallow(<ToDoList tasks={tasks}/>);
* expect(toDoList.find('li').length).toEqual(tasks.length);


const toDoListInstance = shallow(
        <ToDoList tasks={tasks}/>
      );
expect(toDoListInstance).toMatchSnapshot();

     
exports[`ToDoList component when provided with array of tasks should render correctly 1`] = `
<ul>
  <Task
    id={0}
    key="0"
    name="Wash the dishes"
  />
  <Task
    id={1}
    key="1"
    name="Make the bed"
  />
</ul>
`;
```

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

# Jest documentation
https://jestjs.io/docs/en/using-matchers

expect returns expectation objects to call matchers on them

toBe vs toEqual (exact equality vs check the value of an object)

toEqual recursively checks every field of an object or array.

* toBeTruthy matches anything that an if statement treats as true
* toBeFalsy matches anything that an if statement treats as false

#

Writing more tests doesn't mean you get more code quality.

1. What makes a good test
2. Testing strategies
3. Keep tests clean.

## 1. What makes a good test
* fast, doesn't break, easy to write and read, catches bugs, and good coverage to effort ratio

My opinion: I like tests that are easy and it catches bugs.

Fb test hackatons don't work. When good tests are found, share them.

## 2. Testing strategies
* Finding a testing strategy

Flux: (counter example)
UI: doesn't have any busines logic takes Data Store and renders what's in store
ACTION: Function call, INCREMENT_COUNTER. Dispatch when button clicked. Finds mutation.
MUTATION: Updates store. Business logic.
 
STORE -> UI -> ACTION -> MUTATION
STORE -> render -> UI -> dispatch -> ACTION -> increment_counter -> MUTATION


## 3. Keep tests clean.
