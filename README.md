# JavaScript


## Exception Handling

```
try{
        // Test statements for any JavaScript Exceptions or manually throw the exceptions
}catch(e){ // Catch the JavaScript Exception or manually throwned Exceptions
		if(e instanceof InvalidError){// Process the exception
				// e.name
				// e.message
				// e.status
		}else if(e instanceof OutOfRangeError){// Process the exception
		}else{// re-throw the exception
				throw e;
		}
}finally{
		// What to do incase of Success/Failure
}
```
-------------------

## Inheritance
```
- No Classical Inheritance, Only Prototypal Inheritance
- An Object inherits from another Object
----
Prototype

1. __proto__ 
- Non-standard way from firefox/chrome
2. There are 2 standard methods: - IE9+, Chrome and firefox.
-Object.create(prototype, [propObjs])
-Object.getPrototypeOf(obj) 


var animal = {eats: true};
var rabbit = {jumps: true};

// "rabbit" inherits "animal" OR "animal" is prototype of "rabbit"
rabbit.__proto__ = animal; 

__proto__ is equal to [[Prototype]] from the Specification.
----
for..in loop - Enumerating the Object Properties(all enumerable properties of an Object and from its prototype chain)

// get all the Enumerable properties from "rabbit" and its prototype "animal"
for(var prop in rabbit){
   console.log(prop +" -- "+ rabbit[prop]);
}
----

hasOwnProperty()

// get all the Enumerable owned properties from "rabbit"
for(var prop in rabbit){
if(rabbit.hasOwnProperty(prop))
   console.log(prop +" -- "+ rabbit[prop]);
}
```


