jsx方便创建虚拟DOM，需要经过babel转译
jsx可以理解为原始创建虚拟DOM的语法糖
虚拟DOM本质是Object类型的对象
虚拟DOM是React内部在用，无需真实DOM那么多属性
虚拟DOM会被转化为真实DOM呈现在页面上
jsx语法规则：
1.定义虚拟DOM不要写引号
2.标签中混入JS要使用{}
3.样式的类名需要用className
4.内联样式要使用style={{key: value}}
5.虚拟DOM必须只有一个根标签
6.标签必须闭合
7.标签首字母为小写元素，转化为HTML元素
8.无小写字母元素，会报错
9.自定义标签必须大写字母开头

jsx中只能够使用{}引入一个JS语句，而不是引入代码部分
ReactDOM.render()之后，React会解析标签，发现组件是函数定义的，随后会调用该函数，组件首字母必须大写

类式组件必须继承React.Component，而且必须实现render方法,而且render必须有返回值
类式组件使用标签之后，React解析器会自动new一个该类的实例并通过该实例调用到原型的render方法
props, refs, state三大重要属性