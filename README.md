# TechQuiz

Tech Quiz could can test your knowledge or organize interview 


## Table of Contents
1. [Prototype](#prototype)
1. [Closure](#closure)
1. [Min function](#min-value)
1. [Prime Number](#prime-number)
1. [Reverse Number](#reverse-number)

<a name="prototype"/>

## 1. Prototype

Implement inheritance

```
   horse.legs   // 4
   unicorn.legs // 4
   unicorn.corn // 1;
```



Possible answer:
```javascript
    function horse( ) { this.legs = 4 };
    function unicorn() { this.corn = 1; }
    
    unicorn.prototype = new horse();
```

Another possible answer:
```javascript
    class horse {
      constructor(legs = 4){
        this.legs = legs;
      }
    }
    
    class unicorn extends horse{
      constructor(legs, corn = 1){
        super(legs);
        this.corn = corn;
      }
    }
    
    unic = new unicorn();
```

<a name="closure"/>

## 2. Closure

Describe what is closure.

```
const sum = () => { ... };

sum(1)(2) // 3
sum(3)(2) // 5   
 
```

Possible answer:
```javascript
const sum = (a) => {
    return (b) => {
        return a + b;
    }
}
```

<a name="min-value"/>

## 3. Min value

Write function that find min value.

```
const min = ()=>{ ... };

min(2, 2) == 2;     // true
min(3, -1) == -1;   // true
min(1, 3) == 3;     // false
 
```

Possible answer:
```javascript
const min = () => {
  x = [...arguments];
  x.sort((a,b)=>a>b);
  return x[0];
}

const min2= () =>{
  return Math.min(...arguments)
}
```

<a name="prime-number"/>

## 4. Prime Number

Write function that define is number prime.
```
isPrime(1); // true
isPrime(5); // true
isPrime(6); // false
isPrime(9); // false
```

Possible answer:
```javascript
const isPrime = (x) => {
  
  for(let i= x-1; i > 1; i--) {
    if(x%i === 0){
      return false;
    };
  }
  
  return true
}
```

<a name="reverse-number"/>

## 1. Reverse number 

Write function to reverse digits in number.
```
const x = 12345;

revers(x) // 54321

```

Possible answer:
```javascript

fucntion revers(x) {
    x = '' + x;
    x = x.split('').reverse().join('');
    
    return Number(x);
    // or parseInt(x);
}

```

## 1. text 

Write .
```

```

Possible answer:
```javascript

```