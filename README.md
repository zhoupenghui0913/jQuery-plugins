##jQuery Plugins

这是一个jQuery插件集合, 包括 回到顶部插件、懒加载插件、轮播插件、stickUp插件、瀑布流布局插件、tab切换插件。

所有的插件都采用面向对象的方式编写，使用方便，有一定的扩展性。


###1、回到顶部
预览：[回到顶部效果](https://zhoupenghui0913.github.io/jQuery-plugins/gotop/index.html)

#### Usage

在要包含回到顶部元素的容器上调用`gotop`方法即可，该插件会自动添加目标元素，可以自己定制样式。
```
$('body').gotop();
```

### 2、图片懒加载

预览：[懒加载效果](https://zhoupenghui0913.github.io/jQuery-plugins/lazyload/index.html)

#### Usage

在需要`lazyload`的`img`元素中，`src`使用占位图片的`url`，`data-src`使用真实图片的`url`， 然后选中需要懒加载的图片元素, 调用`lazyLoad`方法。

```
$(".container").find('img').lazyLoad();
```

### 3、轮播

预览：[轮播效果](https://zhoupenghui0913.github.io/jQuery-plugins/slide/index.html)

#### 简介

无限滚动的轮播插件，支持点击跳转，自动滚动。需要使用和Demo同样的HTML结构以及一些必要的CSS。

##### Useage

在轮播容器上调用`slide`方法即可。

```
$(".carousel").slide();
```

###4、stickup

预览：[stickUp效果](https://zhoupenghui0913.github.io/jQuery-plugins/stickup/index.html)

#### Usage

当页面滚动时, 不同栏目的导航栏可以始终显示在浏览器窗口顶端位置。

必要的CSS：
```
.stick-up {
    position: fixed;
    top: 0;
    z-index: 99;
}
```

对需要`stickUp`的导航栏使用`stickUp`方法即可。

```
$('.ct').find(".nav").stickup();
```

###5、瀑布流布局

预览：[瀑布流效果](https://zhoupenghui0913.github.io/jQuery-plugins/waterfall/index.html)

#### Usage

在容器上获取需要瀑布流的元素，调用`waterFall`方法即可，支持自适应。
```
$('.ct').find('.item').waterFall( $('.ct') );
```

###6、tab切换

预览：[tab切换效果](https://zhoupenghui0913.github.io/jQuery-plugins/tabchange/index.html)

#### Usage

在指定容器上调用`switchTab`方法即可。
```
// 全部启动
$(".wrap").switchTab();

// 单个启动
$(".wrap1").switchTab();
$(".wrap2").switchTab();
```