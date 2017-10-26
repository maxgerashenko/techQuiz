# TechQuiz

Tech Quiz could can test your knowledge or organize interview 


####Table of Contents
* <a name="prototype">Prototype</a>
* <a name="closure">Closure</a>

<a name="prototype"/>
### 1 [Prototype](#prototype)
Implement inheritance

```javascript
    

```

### 2 [Closure](#closure)
Describe what is closure.

```javascript
const sum = () => { ... };

sum(1)(2) // 3
sum(3)(2) // 5   
 
```

### 3 Min function
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

### 6 Prime Number

```javascript
isPrime(5); // true
isPrime(6); // false
```