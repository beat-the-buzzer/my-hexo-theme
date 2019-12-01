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