# Object



```JavaScript
var a = {
	x: 1,
	y:2,

	set z(o){
		this.x = o.x;
		this.y = o.y;
	},
	// get z(){
	// 	return this.x+this.y
	// }
};

Object.defineProperty(a,"z",{
	value: 6,
});
// console.log(a.z);
console.log(Object.getOwnPropertyDescriptor(a,"z"));
```



