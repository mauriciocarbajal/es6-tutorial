## ES6 Tutorial

Start the tutorial [here](http://ccoenraets.github.io/es6-tutorial).


My notes:

I forked this repo in order to commit my changes on each stage of the above tutorial. Move between commits to see each change.

PD: On the first commit, with title "babel, let (block scoped), destructing" of course it should say "babel, let (block scoped), destructuring" ;)


Some features not included in the tutorial:
# Template strings
```javascript
var name = "John";
var greet = `hi, my name is ${name}`;
```

# Const
```javascript
const name = "John";
name = "Doe"; //throws error, can't mutate name (though I could change attributes on the "name" object)
```


# Static methods in classes
```javascript
class Parent{
	age = 20;
	constructor(){

	}

	static foo(){

	}
}

class Child extends Parent{
	constructor(){
		super();
	}
}

var p = new Parent();

Parent.foo();	//static method
```

# async functions
```javascript
async function(){
	var f = await $.get("http:// ... ");
	console.log(f);
}

// that function returns a promise object
// further: generator functions

function* idMaker() {
  var index = 0;
  while (index < 3)
    yield index++;
}

var gen = idMaker();

console.log(gen.next().value); // 0
console.log(gen.next().value); // 1
console.log(gen.next().value); // 2
console.log(gen.next().value); // undefined
```


