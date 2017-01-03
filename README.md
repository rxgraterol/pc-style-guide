# Platform Convergence Style Guide
Guía de estilo de desarrollo en Platform Convergence

## Indent

- We use an indentation of 4 spaces, instead of 2


## Line max length

 - The limit for each line of code is set at 120 characters. It will produce an error if the limit is surpassed.

## Iteration

- We use the 'each' method for looping and we define the element itterator name at the beggining of the sentence
```java
    // bad
    domainAttributes.each {
      println it.id
    }

    // good
    domainAttributes.each { it ->
      println it.id
    }
```

## Conditional Statements (if / else)
- For small conditional statements we try to compact them in one line if the statement dont surpass the maximun line lenght of 120 characters

```java
    // bad
    if(weKickAsses) {
        awesomeMethod()
    }
    // good
    if(weKickAsses) awesomeMethod()
```
## Method Definition
- Define the method without a type, just with the 'def' definition

```java
class MathExample {
 
    // bad
    Integer sum(a,b) {
      int c = a+b
      println(c)
      return c
    }
    
    // good
    def sum(a,b) {
      def c = a+b
      println(c)
      return c
    }
    
}
```
