## OS模块
格式：`os.函数`

|函数名|使用方法|
|--|--|
|`.getcwd()`|返回当前工作目录|
|`.chdir(path)`|改变目录至|
|`.listdir(path='.')`|列举制定目录中的文件 `'.'`代表当前目录 `'..'`上一次层目录|
|`.mkdir(path)`|创建目录|
-----------
## 文件模块

|打开模式|执行操作|
|:--:|--|
|`r`|只读方式打开（默认）|
|`w`|写入方式打开文件，会覆盖已存在文件|
|`a`|追加模式 继续写|
|`b`|以二进制打开|
|`t`|以文本模式打开（默认）|
|`+`|可读写模式  添加到其他模式中使用|
|`U`|通用换行符支持|

------

## 爬虫
+ 导入urllib包
+ 有些网址需要修改证书添加以下代码
` import ssl
ssl._create_default_https_context = ssl_create_unverified_context
`
--------

## pygame模块

#### display 使用方法
|函数|作用|
|---|---|
|`.set_mode`|设置窗口大小|
|`.set_caption`|窗口标题的名字|

###### `set_mode`显示模式

+ **第一个参数**
设置surface窗口大小
+ **第二个参数**
窗口属性

|选项|含义|
|----|---|
|`FULLSCREEN`|全屏|
|`DOUBLEBUF`|双缓冲模式|
|`HWSURFACE`|硬件加速（仅全屏可实现）|
|`OPENGL`|使用OpenGL渲染|
|`RESIZABLE`|窗口可以调节大小|
|`NOFRAME`|无边框|
+ **第三个参数**
  窗口颜色，一般不设置，由系统自动给出
#### font 使用方法
|函数|作用|
|---|---|
|`.Font`|设置文本格式，第一个参数字体，第二个尺寸|
|`.get_linesize()`|获取每行文本高度|

#### screen 使用方法

|函数|方法|
|---|---|
|`.fill`|填充屏幕|
|`.bilt`|二次覆盖|

#### transform 使用方法

|函数|方法|
|---|---|
|`.flip`|上下左右的翻转|
|`.scale`|缩放（快速）|
|`.rotate`|旋转|
|`.rotozoom`|缩放并旋转|
|`.scale2x`|快速放大一倍图像|
|`.smoothscale`|平滑的缩放图像（精准）|
|`.chop`|裁剪图像|


#### draw 绘制基本图形

|函数|作用|
|---|---|
|`.rect(Surface, color, Rect, width = 0)`|`rect`指定范围`(left, top, width, whight)`|
|`.polygon(Surface, color, pointlist, width = 0)`|`pointlist`一个个点的元组|