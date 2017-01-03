# pc-style-guide
Guía de estilo de desarrollo en Platform Convergence

## Indent

- We use an indentation of 4 spaces, instead of 2

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

## Line max length

 - The limit for each line of code is set at 120 characters. It will produce an error if the limit is surpassed.
