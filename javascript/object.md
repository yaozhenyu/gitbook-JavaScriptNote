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

//为对象a定义一个属性 "z"
Object.defineProperty(a,"z",{
    value: 6,
});

// 获取对象a的属性"z" 结果为
/*
{ value: 6,
  writable: false,
  enumerable: true,
  configurable: true 
}
/*
console.log(Object.getOwnPropertyDescriptor(a,"z"));
```



