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



### 必要的操作方法

当创建一个新的html文件时什么都没有, 随便输入ht

![image-20241219112851458](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219112851458.png)

vscode会跳出来补全项, 选择**html:5**并回车就出现了

![image-20241219113004757](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219113004757.png)

(PS: 可以格式化一下, 输入ctrl + shift + p, 然后输入for就能看到format选项)

![image-20241219113136477](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219113136477.png)

**这样就很漂亮**

![image-20241219113216052](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219113216052.png)

**能出现自动补全一个html模板的原因在于vscode有一个内置的功能叫Snippets, 这个能配置不同语言的代码模板, 用好这个, 可以稍微减低开发难度**

#### 让我们来探究一下, 

1. 仍然输入ctrl + shift + p

![image-20241219113530186](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219113530186.png)

2. 选择Snippets: Configure Snippets后, 需要选择语言, 我们输入html后选择它![image-20241219113716124](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219113716124.png)

3. 里面空空如也, 我们可以写一个自己的html模板

![image-20241219114307613](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219114307613.png)

> **"prefix"**: !html	 当我们输入!html时, 触发这个模板的补全
>
> **"body"**: ...			 是补全的内容
>
> **"description"**: ... 是描述

**手写一个snippet有一点其他的考虑, 具体请查询gpt**

4. 使用这个模板, 输入!html

![image-20241219114702844](C:\Users\jeffp\AppData\Roaming\Typora\typora-user-images\image-20241219114702844.png)

就成功的使用了这个Snippet

**对于html:5这个补全, 我觉得应该是vscode内置的补全, 我们应该无法修改, 因此就没找到**

##### 以上, 如果学会写Snippets, 就可以给很多语言配上这样的模板, 而vscode也会像ide一样初始化工程了

#### PS: 我会在这个教程的后面教vscode的使用技巧



## 本次教程作业

1. 配置让自己写的舒适的Snippets给html, 还有其它的语言
2. 使用Snippets创建一个html的模板, 并尝试用Live Server打开

(你可能会想: **我在vscode外, 选择用浏览器打开这个html文件也可以啊, 为什么要一个插件来运行?** 哦我的朋友, 当你在服务器上远程开发时, 你如何去用浏览器打开呢? 也许能, 但肯定没有这个插件简单)
