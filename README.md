# HHuploadify
基于Huploadify（基于uploadify）的图片上传插件，自动上传，上传进度条，上传后预览

有一个著名的图片上传插件uploadify，在这个插件基础上，Huploadify被开发出来，是由国人开发的，使用起来也比较好用。但是，我希望对自己的项目进行定制，希望实现像淘宝添加图片那样，点击一个上传按钮，然后自己上传，上传的时候，有一个进度条，上传完之后，预览图片。

同时，在Huploadify基础上，还增加了单个图片上传，比如在上传头像的时候，不可能让你上传多张图片。

因此，我在Huploadify的基础上进行修改，得到了HHuploadify。

HHuploadify的用法和Huploadify的用法是一模一样的。不过增加了几个点：

1. 增加isSingle配置项，在初始化的时候，如果isSingle=true，那么这个上传只能上传一张图片。domo.html中有案例
2. 增加了上传图片结束后，将图片显示到该上传区域中预览，返回格式必须是json，有一个url字段。upload.php中有案例

修改样式：通过修改HHuploadify.css文件中的样式来控制表现。

上传后得到的图片预览是通过将图片作为该区域的背景图片实现的，因此，如果要调整该图片，必须通过css来进行控制。

http://www.tangshuang.net/2002.html
