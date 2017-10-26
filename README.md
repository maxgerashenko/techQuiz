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

```
   horse.legs // 4
   unicorn.legs // 4
   unicorn.corn // 1;
```



Possible answer:
```javascript
    function horse( ) { this.legs = 4 };
    function unicorn() { this.corn = 1; }
    
    unicorn.prototype = new car();
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

## Closure

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

## Min value

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

## Prime Number

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