# placement-engineer-coding-test
Test coding knowledge of placement students.

Given the following JavaScript code


```js
export function will_return_some_value(some_array_of_intgers) {
  let return_some_value = 0;

  some_array_of_intgers.forEach((num) => {
    if (num == 5) {
      return_some_value += 7;
    } else if (num % 2 == 1) {
      return_some_value += num + 2;
    } else if (num % 3 == 1) {
      return_some_value += additional(num);
    } else {
      return_some_value += 3;
    }
  });

  return return_some_value;
}

export function additional(an_intger) {
  let return_some_value = 0;

  let modified_input = an_intger * 5;

  if (modified_input % 3) {
    return_some_value += an_intger * 7;
  } else if (modified_input % 4 == 1) {
    return_some_value += modified_input + 2;
  }

  return return_some_value;
}
```

What is the output of each function call: 
- will_return_some_value([0, 1, 1, 2, 3]);
- will_return_some_value([5, 8, 13, 21]);
- will_return_some_value([1, 1, 2]);
- will_return_some_value([5, 8]);
- will_return_some_value([13, 21]);
