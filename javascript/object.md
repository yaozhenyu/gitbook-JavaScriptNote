# Object

所有对象继承自Object类

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
var a = {
    x: 1,
    y:2,

    set z(o){
    },
    get z(){
        return this.x+this.y
    }
};

a.z = 8;
console.log(a.z) // 结果为3，调用get方法获取值
// 对象a定义了一个属性z
```



