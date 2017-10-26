# TechQuiz

Tech Quiz could can test your knowledge or organize interview 


## Table of Contents
1. [Prototype](#prototype)
1. [Closure](#closure)
1. [Min function](#min-value)
1. [Prime Number](#prime-number)

<a name="prototype"/>

## Prototype

Implement inheritance

```javascript
    

```

<a name="closure"/>

## Closure

Describe what is closure.

```javascript
const sum = () => { ... };

sum(1)(2) // 3
sum(3)(2) // 5   
 
```

<a name="min-value"/>
## Min value
Write function that find min value.

```javascript
const min = ()=>{ ... };

min(2, 2) == 2;     // true
min(3, -1) == -1;   // true
min(1, 3) == 3;     // false
 
```

Possible answer:
```
function min() {
  x = [...arguments];
  x.sort((a,b)=>a>b);
  return x[0];
}

function min2() {
  return Math.min(...arguments)
}
```

<a name="prime-number"/>
## Prime Number

```javascript
isPrime(5); // true
isPrime(6); // false
```