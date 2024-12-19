# 学习html5

## 快速上手html5

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
		<title>Document</title>
	</head>
	<body>
    </body>
</html>

```

以上是一个最基本的html框架, 我们把上面的

- html, head, meta, title, body称为标签(label) 

- charset="UTF-8"称为属性(props)
- 在title标签里面的Document称为内容(content)
- 标签是分级的, head, body标签在html标签里面, meta, title在head标签里面, 相对而言, 把外层标签称为父标签(parent), 内层标签称为子标签(children), 而且这些标签的关系是分级的, 让我来画一个标签树

![image-20241219105155840](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219105155840.png)

(如果你想知道画这种流程图用的什么软件, 这个是draw.io, 最初我用它来画UML图, 实际上它能做的是远不止那些, 访问app.diagrams.net即可使用在线版draw.io, 如果你觉得有用, 给它github添上一星吧)

- 标签分 **开标签**\<body>,和**闭标签**\</body>, 它们之间包裹的是内容, 会被渲染到浏览器上



## 用vscode编辑html

### 必要的插件

![image-20241219105836648](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219105836648.png)

以上三个插件, 

- Auto Close Tag, 当你输入开标签, 会自动补全闭标签

- Auto Rename Tag, 当你修改开标签, 也会自动修改闭标签

![image-20241219110511582](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219110511582.png)

- live Server: 会将编写的html文件运行到浏览器上

**使用方法**

![image-20241219110648006](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219110648006.png)

按ctrl + shift + p, 进入vscode的命令行模式, 输入live会找到**Live Server: Open with Live Server**

往下选择它, 按enter就自动把html运行到浏览器上了

**(一个伟大的编辑器, 不会设计一个复杂的页面, 放着很多一辈子都用不到的功能, 应该是把功能放到命令框里, 当需要的时候搜索即可, 并且以插件的形式存在, 不需要即可删除)**

**在弹出的浏览器里查看html页面**

![image-20241219111448153](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219111448153.png)

干净的像一张白纸, 因为我们还没有写任何东西