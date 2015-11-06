## KISS

**K**eep **I**t **S**imple, **S**tupid.

## Make it... Make it... Make it

1. Make it work.
1. Make it right.
1. Make it fast.

## Write Tests First

Before you implement, write the test.

### Make the Unit Test as a Bug Report

Before write a test, remember to answer all the questions:

1. What are you testing?
1. What should it do?
1. What is the actual output?
1. What is the expected output?
1. How can the test be reproduced?

```js
// A Unit Test Template
import test from 'tape';

// For each unit test you write,
// answer these questions:
test('What component aspect are you testing?', assert => {
  const actual = 'What is the actual output?';
  const expected = 'What is the expected output?';

  assert.equal(actual, expected,
    'What should the feature do?');

  assert.end();
});
```
