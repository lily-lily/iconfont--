# iconfont--
把图标做成iconfont字体，在线制作iconfont，省去占用图片空间缩小图标大小
1）首先登陆阿里巴巴矢量图标库http://www.iconfont.cn/，将你需要的图标点击加入购物车；
2）打开右上角的购物车，将选择的图标添加在项目中，如果没有项目可以新建项目，确定加入即可；
3）点击项目后，然后在“图标管理”-“图标应用项目”中找到这个项目，查看在线链接，把里面的代码复制到CSS中。
@font-face {
  font-family: 'iconfont';  /* project id 309142 */
  src: url('//at.alicdn.com/t/font_ci6pfokyd5vlhaor.eot');
  src: url('//at.alicdn.com/t/font_ci6pfokyd5vlhaor.eot?#iefix') format('embedded-opentype'),
  url('//at.alicdn.com/t/font_ci6pfokyd5vlhaor.woff') format('woff'),
  url('//at.alicdn.com/t/font_ci6pfokyd5vlhaor.ttf') format('truetype'),
  url('//at.alicdn.com/t/font_ci6pfokyd5vlhaor.svg#iconfont') format('svg');
}
.iconfont {
  font-family:"iconfont" !important;
  font-size:16px;
  font-style:normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
在html中可以直接使用
<i class="iconfont">&#xe640;</i>

或者下载至本地，解压文件夹可以看到生成的html、css、以及其他的svg、ttf等等，打开iconfont.css文件可以直接到css中
@font-face {font-family: "iconfont";
  src: url('iconfont.eot?t=1495509603231'); /* IE9*/
  src: url('iconfont.eot?t=1495509603231#iefix') format('embedded-opentype'), /* IE6-IE8 */
  url('iconfont.woff?t=1495509603231') format('woff'), /* chrome, firefox */
  url('iconfont.ttf?t=1495509603231') format('truetype'), /* chrome, firefox, opera, Safari, Android, iOS 4.2+*/
  url('iconfont.svg?t=1495509603231#iconfont') format('svg'); /* iOS 4.1- */
}

.iconfont {
  font-family:"iconfont";
  font-size:16px;
  font-style:normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-gouwuchetianjia:before { content: "\e640"; }

.icon-xiazai:before { content: "\e6dd"; }
在html中直接使用为<i class="iconfont icon-xiazai"></i>效果也是一样的。
4）如果你需要的图标不符合，也可以直接自己上传，不过需要验证通过才可以使用。
5）下载的图标可以根据.confont的样式来决定颜色或者大小等

注：雪碧图又称csssprite,可以将许多小图标放至在一张图上，不过占用内存大。目前需要推荐的iconfont字体支持小图标。大图片的需要压缩推荐https://tinypng.com/，不过有限制，只压缩png或者jpg
