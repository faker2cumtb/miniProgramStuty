小程序中this指向的是当前对象，在方法的回调函数中，this已经改变了，并不指向之前的对象
### 解决方法
- 使用that保存this的状态

var that = this

- 使用es6中的箭头函数

   () => {
  }
  es6中的箭头函数没有自己的this，它的this是继承外层代码块的this
