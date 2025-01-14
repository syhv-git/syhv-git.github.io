---
layout: essay
type: essay
title: From Java and C++ to Javascript
# All dates must be YYYY-MM-DD format!
date: 2021-09-01
labels:
  - Programing Languages
  - Learning
---

## My programing language background

My first introduction to Javascript was in January of 2021, as my father had the O’Reilly textbook, *Learning PHP, MySQL, & Javascript*, however I only briefly read over the Javascript section. At the time, I was more curious with PHP and MySQL, so I did not go in depth on Javascript. This textbook became a valuable resource, but I did not apply the code I was learning as this was more for an introduction to the syntax of these languages, rather than their capabilities. Also, at the time of acquiring this textbook, I was fascinated by LISP, and was reading, *Structure and Interpretation of Computer Programs*, by Harold Abelson and Gerald Sussman. At the time, I never really saw the true connection between the two languages until August 2021 when I started taking ICS 314 at the University of Hawai\`i at Manoa. Prior to January 2021, I only had knowledge in Java, C, and C++, and used these languages and strictly Object-Oriented programing languages. I enjoyed the structured setting of these languages, but when learning the fundamentals of LISP, I realized how limiting these languages can be. LISP requires the user to define everything beyond basic operations and conditional expressions. My mind was expanding with the possibilities of using procedures in new procedural definitions, and this was my first introduction to Functional programing.

## Learning Javascript

When I started ICS 314, we learned Javascript through, freecodecamp.org, and the aspect of LISP in Javascript became clear. Every function can be utilized as variables, and one can even create a function within another function's scope. However, I would not say I understood LISP, as I only was able to comprehend the first two chapters of the LISP textbook. I ultimately only had experience in Java, C and C++, and this led to some issues when utilizing Javascript. After completing the freecodecamp course, I had a good, basic understanding, but when I worked on my first problem, I had a correct algorithm, but the implementation had a bug. Prior to learning Javascript, all of my variables were declared within their own types, i.e int, float, string, etc., but Javascript declares variables as var, let, and const. My first bug was that I did not initialize my variables to the type of data to be handled. I spent a lot of time trying to re-write my code in a new way, hoping I would find the reason my code did not work, but all it required was one line to be changed,

```
let total; //changed to:    
let total = 0;
```

This seemingly simple and almost intuitive syntactical error was from being conditioned by learning Java, C, and C++, as we could define,

```
int total;
```

The programing language would initialize total to be 0 without a direct assignment. This helped me see the connection to LISP as all variables require the same concept as Javascript, with more basic foundations.

```
(define total 0) //for a LISP representation of the above
```

As stated in the beginning of this section, another connection between LISP and Javascript is the procedure Lambda in LISP. Lambda is the process of creating a procedure within a procedure, without having to define the procedure with a name. This correlates to the ability to create functions within functions in Javascript, called arrow functions. The arrow function is another way to create a function in Javascript and is assigned to a variable. This function can be created within the scope of a defined function, and this makes it so it cannot be called by any other process outside of the defined functions scope. This is fundamental to all languages which fall under the functional programing paradigm.

```
//Javascript function for x^4
function fourthPower(x) {
    const two = (x) => {
         return x * x; //return x^2
    }
    return two(x) * two(x); //returns x^4
}

//Lisp parallel to the above
(define (fourth-power x) //this defines the procedure which is called by, fourth-power x, which returns x^4
    (* (lambda (x) (* x x)) (lambda (x) (* x x)))) //given input x, two lambda procedures of x * x are multiplied together
```

While having a power function is achievable with Math.pow() in Javascript, it is meant to showcase the arrow function nesting, and serve as a platform to understand the LISP parallel. For the LISP code, having a defined square function is necessary, but showcases how the Lambda procedure works.

Another aspect in Javascript which is difficult to fluently incorporate into my formalizations is creating arrays and objects to utilize multiple types, rather than restricted to only one defined type. In the same sense as the above problem, arrays in Javascript are not defined as:
  
```
const[] arr; //as Java would be int[] total;
```

but rather,

```
const arr = []; //or {} to create an object
```

This also allows dynamic arrays which I understood from C and C++. However, unlike C and C++, we can input any type of data into the indices of the array. Also, with objects, they have an indication parameter followed by the value associated with the title.

```
const obj = {name: Scott}
```

We would access the contents of name with,

```
obj.name; //this takes the variable arr, and we find Scott by going to the section labeled name
```

This is reminiscent of objects constructed from classes in Java and C, but we do not need to directly create individual classes to create data structures. Also, we can easily create arrays of objects, which we would not be able to do in Java and C unless we created an overloaded operation to work with a specific object.

## Conclusion

Overall, my understanding of Javascript is minimal, but the usefulness is clear. This programing language has helped me expand my mind in new ways, and make connections between knowledge I already have. Javascript should not be a programmers first language, but is essential to learn, as it brings many unique aspects to a coder’s toolkit. It also enhances abstract thinking when solving problems in ways that languages like Java and C cannot offer. Furthermore, learning Javascript from the athletic software engineering pedagogy has been intense, but also quite fun. While the first week was a bit difficult, I have found that my ability to hear a problem and think through possible solutions in real time, then transpose that to code has gotten increasingly better. The structure of doing practice workouts of the day without any knowledge of a correct solution, then going through the example, even if I completed it within the alotted time the first attempt, is the most crucial part to see success. The Brandon led WODs are also very valuable as his problems get me to start thinking about how I structure my code, and utilize Javascript in a more efficient way.
