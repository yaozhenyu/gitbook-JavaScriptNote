# Object

所有对象继承自Object类



##  创建对象的三种方法

## Object内置方法

* Object.defineProperty
* Object.getOwnPropertyDescriptor

```JavaScript
var a = {
    x: 1,
    y:2,
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
*/
console.log(Object.getOwnPropertyDescriptor(a,"z"));
```

**setter/getter**

```JavaScript
// 对象a定义了一个属性z
var a = {
    x: 1,
    y:2,

    set z(o){
    },
    get z(){
        return this.x+this.y
    }
};

a.z = 8; // 不能赋值了
console.log(a.z) // 调用get方法获取值，结果为3
/* 结果：
{ get: [Function: get z],
  set: [Function: set z],
  enumerable: true,
  configurable: true 
}
*/
console.log(Object.getOwnPropertyDescriptor(a,"z"));
```



