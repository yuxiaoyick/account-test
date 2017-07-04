##用Mac做一个可以动的web页面

用到了node.js、vue、html等方式，主要是node.js

是从[这里](https://github.com/jirengu-inc/animating-resume)看到的做法，模仿着做出来的，因为以上语言，我都不会😆

然后做出来的效果是[这样的](https://yuxiaoyick.github.io/account-test/dist/)（听说用搜狗浏览器是打不开的），下面我就说一下怎么搞出来的：

1：首先去GitHub上面新建一个项目（没有注册的要去注册一下），这样：

![这个图片一会再换](http://images2015.cnblogs.com/blog/903320/201603/903320-20160305134947346-1921005167.png)

然后给项目起个名字：
![项目名字](http://images2015.cnblogs.com/blog/903320/201603/903320-20160305135528627-97762586.png)

2：打开settings，有一个Github Pages 的设置，点击 source 中的本来的 None ，使其变成 master 分支，也就是作为部署github pages 的分支，然后点击 save。
![设置](http://images2015.cnblogs.com/blog/903320/201603/903320-20160305140204096-424861698.png)

![开个外网分支](http://images2015.cnblogs.com/blog/903320/201701/903320-20170115212404385-1979000093.png)

3：页面刷新之后，再看 github pages 设置框处，多了一行网址，就是你的 github pages 的网址了。（点进去你就会发现外网网址有了）
![网址出现](http://images2015.cnblogs.com/blog/903320/201701/903320-20170115213630338-44375750.png)

4：把你的新项目clone下来，进行修改。

我一般会用GitHub自带的工具，你也可以用git工作之类的代码管理工具。

##（这里的过程是如何在Github Pages生成自己的外网网址，有了这个网址就可以做很多事情了，比如：把自己写的网页放上去等等）

#然后下一阶段：
1：到这个[地方](https://github.com/yuxiaoyick/account-test)，把资源拷下来；

2:下载[node.js](http://nodejs.cn/)中文网

## 使用方法

``` bash
cd account-test
npm install
npm run dev
```

## 部署方法


1. 编辑 config/index.js，修改第 10 行的 assetsPublicPath，值为 `项目名/dist`。如果你没有修改项目名 account-test，则可跳过此步骤。（是你在GitHub上新建的那个项目名）

2. 编译、上传
    ``` bash
    npm run build
    git add .
    git commit -m "update"
    git push
    ```
    
记得npm run build编译成功之后，再上传。

然后你一定会问，怎么改这里的东西？大胡子是什么鬼？？？？？？
哈哈哈哈。。。。
我来说下怎么改里面的东西。

在src/App.vue里面改，用什么编译器呢？我用Xcode和WebStorm都可以。

装biu神功已经传授给你了，去成为biu界大佬吧！！！
