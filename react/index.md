# React

---

* [命令行工具](#命令行工具)
* [JSX语法](#jsx语法)

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

## render\(\)函数



