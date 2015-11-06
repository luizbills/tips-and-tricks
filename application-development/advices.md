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

## Pure Functions are the Simplest Functions

Functions which have no side-effects and exhibit referential transparency are called pure functions.
A pure function:

- Given the same input, will always return the same output.
- Produces no side effects.
- Relies on no external state.

The simplest functions are pure functions. If a problem can be solved with pure functions, there’s a good chance that pure functions are the simplest solution to the problem.

### About Side Effects

Side effects include any state change that is visible outside the function. That includes logging messages, displaying things to the screen, and throwing exceptions. If it’s possible for a function to throw an exception, that fact should be clearly documented. If it’s possible to avoid an exception and still make the function safe to use, you should favor that course over throwing.
