# 项目预览

在这个项目中，你会得到一个基于 web 的用来读取 rss 源的应用。最开始的这个项目的开发者意识到了测试的价值，他们也已经把 [Jasmine](http://jasmine.github.io) 包含在了项目之中，而且甚至已经开始写他们第一个测试用例。但是不幸的是，他们决定去创建一个他们自己的公司，所以我们现在拿到的是一个缺乏完整测试用例的应用，这样是你会参与到这个项目的原因。

# 安装
克隆该项目打开index.html的本地路径即可

# 我如何完成这个项目
- 在浏览器里面查看一下应用的功能
- 查看项目的 HTMl (**./index.html**), CSS (**./css/style.css**) 和 JavaScript (**./js/app.js**) 文件来对项目的工作原理有一个基本的了解。
- 查看 Jasmine spec 文件 **./jasmine/spec/feedreader.js** 然后翻阅阅读 [Jasmine 文档](http://jasmine.github.io)。
- 编辑 **./js/app.js** 里面的 `allFeeds` 变量使给出的测试通不过，然后观察Jasmine是怎么展示你应用的错误信息的。
- 第一个测试用来保证 allFeeds 变量被定义了而且不是空的。
- 编写一个测试遍历 allFeeds 对象里面的所有的源来保证有链接字段而且链接不是空的。
- 编写一个测试遍历 allFeeds 对象里面的所有的源来保证有名字字段而且不是空的。
- 写一个叫做 `"The menu"` 的测试用例
- 写一个测试用例保证菜单元素默认是隐藏的。需要分析 html 和 css 来搞清楚是怎么实现隐藏/展示菜单元素的。
- 写一个测试用例保证当菜单图标被点击的时候菜单会切换可见状态。这个测试应该包含两个 expectation ： 党点击图标的时候菜单是否显示，再次点击的时候是否隐藏。
- 写一个叫做 `"Initial Entries"` 的测试用例
- 写一个测试保证 `loadFeed` 函数被调用而且工作正常，即在 `.feed` 容器元素里面至少有一个 `.entry` 的元素。
- 写一个叫做 `"New Feed Selection"` 的测试用例
- 写一个测试保证当用 `loadFeed` 函数加载一个新源的时候内容会真的改变。
