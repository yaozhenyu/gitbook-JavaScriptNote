# Object

所有对象继承自Object类

## Object内置方法

* Object.defineProperty
* Object.getOwnPropertyDescriptor

```JavaScript
var a = {
    x: 1,
    y:2,

    set z(o){
        this.x = o.x;
        this.y = o.y;
    },
    // get z(){
    //     return this.x+this.y
    // }
};

Object.defineProperty(a,"z",{
    value: 6,
});
// console.log(a.z);
console.log(Object.getOwnPropertyDescriptor(a,"z"));
```



