## 个人博客的theme文件

下载后放在theme文件夹，然后在hexo根目录下修改主题文件

### 注意事项：

1、 Menu中使用绝对路径的地址

需要在地址前面加上两个斜线

```yml
github:
  url: //https://github.com/beat-the-buzzer/
  target: _blank
```

2、去除javascript:;

源码里面有很多地方渲染的时候都加上了`javascript:;`，导致一些点击跳转失效

3、发布到github.io的问题

有时候在本地运行可以正常，但是在远程访问的时候，找不到文件。

原因：修改了文件夹的大小写，在提交Git的时候，远程不会修改；

例如：远程的文件夹是css，本地改成CSS，push到远程，最终的文件名还是小写的css；

解决方案：发布之前清除`github.io`的`master`分支里面的文件；

发布注意：尽量不要修改文件的大小写。