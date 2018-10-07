#DESIGN PATTERN In JavaScript

###Why Design Pattern?
* Design patterns are the basic building block for maintainable software applications.
* A guide for novice developers looking to improve their coding skills.
###Programming is like WAR
###You are the Warrior
![War](http://media.cleo.com.sg/2018/04/avengers-infinity-war-poster-768x597.jpg)

###To win the war you need Plan- Pattern
![War](http://2.bp.blogspot.com/-h-wKbGwEHO0/VaSoN-6SU3I/AAAAAAAABrQ/WcJQcWbUFjY/s1600/baahubali-battle-plan.jpg)

###What is Design Pattern
Design patterns are reusable solutions to commonly occurring problems in software design.  
* Patterns are proven solutions to software development problems
* Patterns are scalable as they usually are structured and have rules that you should follow
* Patterns are reusable for similar problems.

###Categories Of Design Pattern

* Creational - focus on handling object creation mechanisms
* Structural -concerned with object composition and typically identify simple ways to realize relationships between different objects.
* Behavioral - focus on improving or streamlining the communication between disparate objects in a system.

##Although there is a long list of design patterns , I will cover few

###Type of Pattern 
* Module
* Prototype
* Observer
* Singleton

###Module Design Pattern
 Help in keeping the units of code for a project both cleanly separated and organized. Github https://gist.github.com/acharyaks90/58ff6c9022359015414ea6c99f2697fd Gist-
 ```javascript
 
//  Module Pattern
var healthLifeStyle = (function() {
  var yoga = 'Pranayam'

  var doYoga = function() {
     console.log('Deep Breathing');
  }

  return {
    exercise: function() {
      doYoga();
      console.log(yoga);
    }
  };

})();

healthLifeStyle.exercise();       // Outputs: 'Deep Breathing'
console.log(healthLifeStyle.yoga);  // undefined
```
