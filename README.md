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


