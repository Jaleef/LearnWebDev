## node和npm的学习

## node

nodejs是像python一样的解释器, 可以解释运行javascript代码

### 下载

[Node.js — 在任何地方运行 JavaScript](https://nodejs.org/zh-cn)

最好安装22.12.0LTS, 

**(PS: LTS是长期支持的意思, 这个词可能经常遇到; 一般, 偶数版本是稳定版, 奇数版本是开发版, 所以目前最好选择22.12.0)**

安装好后使用`node -v`检查版本, 没有问题即可



### 运行

运行方式也非常简单

```bash
node xxx.js
```

即可

**PS: 在项目中一般不用这样运行, 但是记住可以这样运行js即可**



## npm

当安装上面的node时, 会自动安装npm, `npm -v`检查版本

npm是nodejs的包管理工具, 类似于python的pip, 可以一键安装js的包

[点我查看npm有什么包](https://www.npmjs.com/)



### 配置代理

npm安装的包一般都很大, 下载很耗费时间, 推荐使用代理或者换源的方法, 我这里介绍如何配置代理

1. 首先确定代理服务器, 我的代理软件运行在本地的7890端口, 所以我的代理地址就是

```
127.0.0.1:7890
```

所以设置http和https代理

```bash
# http代理
npm config set proxy http://127.0.0.1:7890
# https代理
npm config set https-proxy http://127.0.0.1:7890 
```

查看npm是否成功配置代理

```bash
npm config get proxy
npm config get https-proxy
```



### 基本使用

