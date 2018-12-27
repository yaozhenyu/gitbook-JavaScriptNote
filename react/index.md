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

把HTML代码当作对象

```JavaScript
const element = <h1>Hello, world!</h1>;
```

## 组件

props是指组件的所有属性

```HTML
<div id="root"></div>
```

```JavaScript
// ES5写法
function HelloMessage (props) {
  return <h1>Hello, {props.name}</h1>;
}

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

// 把<div>里的内容挂载到id="root"的dom中
ReactDOM.render(
  <HelloMessage name="Taylor" />,
  document.getElementById("root")
);
```

## Props



