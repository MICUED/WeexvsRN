# weex vs RN

文档版本0.0.1<br>
说明: Weex 和 React Native 是使用js开发移动端的两大热门框架，Weex 是阿里巴巴旗下的，React Native 是facebook旗下的。二者现在均开源，以下内容主要介绍了二者的优劣，各位可从官网中了解两大技术。[Weex](http://weex.apache.org/cn/guide/)， [React Native](https://facebook.github.io/react-native/docs/getting-started.html)
## 对比
### 1、跨平台
Weex：Weex官网宣称是跨三端，确实绝大部分组件做到了跨三端，应该封装绝大部分易于抽象的，能够三端实现的组件，但是各个平台在这些组件上还是会略有差异，有些平台特定的组件或者样式Weex并没有进行[封装](http://weex.apache.org/cn/references/web-standards.html)

React Native: 跨两端，也是封装了native组件，对于特定平台有特定的组件，但是并不能运行在Web端，社区中有人尝试过做一层封装跑到web上，但反馈并不好。

总结：二者皆对于平台绝大部分组件进行了封装，例如image/text等，但是RN在ios和android端自带组件多一些，二者开发过程中还是可能需要对特定平台的进行判断，或者编写特定平台的代码用以封装，Weex的优势在于天生集成web端。

```
Weex: 4
React Native: 3.5

```
### 2、版本要求
Weex: 支持安卓4.0+，ios7.0+
React Native: 支持安卓4.1+, ios7.0+

总结: 版本要求Weex略胜一筹，大巴但是安卓4.0以下用户，ios7.0以下用户的数量级已经很小，对整体的用户体验不大，当然多一个版本就是多一些赚钱的机会！

```
Weex: 5
React Native: 4.5

```
### 3、学习成本
Weex: 使用Vue作为上层框架，语法简单，易于上手
React Native: 使用jsx语法，相对于Vue语法（当然Vue也支持jsx）复杂一些

总结: 排除对组件的使用，只谈语法，Vue语法明显更符合当今前端开发方式，jsx超前一些，适用于重逻辑的业务，当然，jsx熟悉之后，也非常方便。

```
Weex: 5
React Native: 4

```

### 4、社区贡献

Weex: 官方平台上，目前来看只有十个可用组件[market](https://market.dotwe.org/ext/list.htm#15),电商常用的支付模块也没有相应的社区贡献，如果没有这类组件，前端需要自己编写原生代码（OC，java）

React Native: 社区贡献度非常活跃，这一点RN完胜Weex，[module](https://js.coach/react-native)，这点节约了业务开发很多时间和精力。

总结: React Native社区基本上做到了覆盖了所有的业务组件，这一点Weex社区需要做的还有很多

```
Weex: 1
React Native: 5

```
