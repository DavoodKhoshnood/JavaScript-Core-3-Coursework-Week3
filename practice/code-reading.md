# Code reading

## Question 1

Take a look at the following code:

```
1    let x = 1;
2    function f1() {
3        let x = 2;
4        console.log(x);
5    }
6    console.log(x);
```

Explain why line 4 and line 6 output different numbers.

In line 4 x is local variable of function f1 and in line 6 x is a global variable which defined in line 1.

## Question 2

Take a look at the following code:

```
let x = 10

function f1()
{
    console.log(x)
    let y = 20
}

console.log(f1())
console.log(y)
```

What will be the output of this code. Explain your answer in 50 words or less.

console.log(f1()) and console.log(y) will print undefine variable.

## Question 3

Take a look at the following code:

```
const x = 9;

function f1(val) {
  val = val + 1;
  return val;
}

f1(x);
console.log(x);

const y = { x: 9 };

function f2(val) {
  val.x = val.x + 1;
  return val;
}

f2(y);
console.log(y);
```

What will be the output of this code. Explain your answer in 50 words or less.

console.log(x) will print 9 because it doesn't change anywhere,
console.log(y) will print 10 because x is a property of y that sent to function f2
