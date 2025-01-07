this - reference to the object where THIS is used (the object depends on the immediate context)
person.name = this.name

note: when you use arrow function in an object, when you call a property (ie. ${this.xxx}) with this. it is referring to the window object of the page. 
