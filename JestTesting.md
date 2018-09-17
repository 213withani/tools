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
