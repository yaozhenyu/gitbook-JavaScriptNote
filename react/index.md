# React

---

* [命令行工具](#命令行工具)
* [JSX语法](#jsx语法)
* [组件 - Component](#组件)

## 命令行工具

```bash
# 创建一个叫myapp的单页面应用
npx create-react-app myapp
```

## JSX语法

```JavaScript
ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);

// 把html代码当作一个对象，并作为结果返回


// 将HelloMessage函数返回的html代码挂载到id=root的dom对象下
ReactDOM.render(
  <HelloMessage name="Taylor" />,
  document.getElementById("root")
);
```

## 组件

props是指组件的所有属性

```JavaScript
// ES6写法
class HelloMessage extends React.Component {
  render() {
    return (
      <div>
        Hello {this.props.name}
      </div>
    );
  }
}

// ES5写法
var HelloMessage = React.createClass({
    rende:function(){
        return (
            <div>
                Hello {this.props.name}
            </div>
        );
    }
});

ReactDOM.render(
  <HelloMessage name="Taylor" />,
  document.getElementById("root")
);
```



