# JS Fundamentals Checkpoint 6 Drills

## 1
**Learning:** basic arithmetic operations, precedence

**Question:** Write a function named `celciusToFahrenheit` that accepts a numeric parameter named `celcius` representing a temperature in degrees celcius. Return the temperature converted to degrees fahrenheit. Remember that the formula to convert celcius to fahrenheit is `fahrenheit = (celcius x 9/5) + 32`.

**Solution:**

```
  function celciusToFahrenheit(celcius) {
    return (celcius * 9/5) + 32;
  }
```

## 2
**Learning:** basic arithmetic operations, Math object

**Question:** Write a function named `circleArea` that accepts a single numeric value named `r` representing the radius of a circle. Return the area of teh circle using the formula `area = PI x r^2`.

**Solution:**

```
function circleArea(r) {
  return Math.PI * Math.pow(r, 2);
}
```

## 3
**Learning:** arithmetic expressions, modulus, numeric types are not integers, string construction using template literals

**Question:** Write a function named `integerDivision` that accepts two numbers named `a` and `b` and calculates the integer value `a/b` and the remainder after division. Then return a string in the format `"a / b is quotient with remainder r"`. 

*Hint: which method of the Math object will give you just the integer part of a number?* 

**Solution:**

```
function integerDivision(a, b) {
  let quotient = Math.trunc(a / b);
  let remainder = a % b;
  return `${a} / ${b} is ${quotient} with remainder ${remainder}`;
}
```

## 4
**Learning:** simple conditional, basic validation

**Question:** Revisit the integer division question from above. In that question we did not consider what happens if the function was called with the parameter b = 0. Since division by zero is not defined it would not be possible to perform that operation. Write a new function that provides the same functionality as `integerDivision` but if `b = 0` returns `'Sorry, cannot divide by zero'` instead.

**Solution:**

```
function integerDivision2(a, b) {
  if(b == 0) {
    return 'Sorry, cannot divide by zero';
  } else {
    return integerDivision(a, b);
  }
}
```
