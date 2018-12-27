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
// 把html代码当作一个对象，并作为结果返回
class HelloMessage extends React.Component {
  render() {
    return (
      <div>
        Hello {this.props.name}
      </div>
    );
  }
}

// 将HelloMessage函数返回的html代码挂载到id=root的dom对象下
ReactDOM.render(
  <HelloMessage name="Taylor" />,
  document.getElementById("root")
);
```

## 组件

```JavaScript
// 继承React.Component，上面的例子是ES6写法

```

## render\(\)函数



