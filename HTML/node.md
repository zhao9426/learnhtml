# 文本
1. `h1 ~ h6` 标题
1. `p`  段落 
1. `b` 粗体 `i`斜体
1. `sup` 上标
1. `sub`下标
1. `br` 换行符
1. `hr`水平线
## 语义化标记
1. `strong` 加粗
1. `em` 强调
1. `blockquote` 较长引用
1. `q` 段引用
1. `abbr` 缩略词
1. `acronym` 首字母
1. `cite` 引文
1. `dfn` 定义
1. `address` 地址信息
1. `ins` 插入内容
1. `del` 删除文本
1. `s`不应当予以删除的内容
## 空白
当浏览器遇到两个或两个以上的空格时，只将看成一个

# 列表
1. `ul` 无序列表 
1. `ol` 有序列表
    +  `li` 列表项
1. `dl` 定义列表
    + `dt` 被定义项
    + `dd` 定义内容      

注：所有列表都可以嵌套


# 链接
1.  指向其他网站的链接
    ```
    <a href="http://www.empireonline.com">Empire</a>
    ```
1. 指向同一网站中其他网页的链接
    ```
    <a href="index.html">Home</a>
    ```
## 相对路径
### 相对连接类型
1. 相同的文件夹：
    ```
    <a href="reviews.html">Reviews</a> 
    ```
1. 子文件夹：
    ```
    <a href="music/listings.html">Listings</a>
    ```
1. 孙子文件夹：
    ```
    <a href="movies/div/reviews.html">Reviews</a>
    ```
1. 父文件夹：
    ```
    <a href="../index.html">Home</a>
    ```
1. 祖父文件夹：
    ```
    <a href="../../index.html">Home</a>
    ```
1. EMAIL 链接-mailto       
    ```
    <a href="mailto:join@example.org">Email Join</a>
    ```

1. 在新窗口中打开链接-target
    ```
    <a href="http://www.imdb.com" target="_blank">
    ```
1. 链接到当前页面的某个特定位置
    ```
    <a href="#top">top</a>:链接到页面顶部id特性值为top的某个元素
    ```
1. 链接到其他页面的某个特定位置
    ```
    <a href="http://www.htmlandcssbook.com/#bottom">aaa</a>:链接到其他页面底部id特性值为bottom的某个元素
    ```
# 图像
## 添加图像
1. `img` 标签添加图像，他没有结束标签，必须包含两个属性
1. `figure` 标签添加多个图片说明
1. `figcaption` 标签给图片添加说明
1. `src` 属性告知浏览器图片所在的地址，该特性值指向某个图片的相对路径
1. `alt`属性对图像进行文本说明
1. `title`属性提供有关图像的附加信息，光标悬停显示
1. `height` 高
1. `width` 宽
## 在代码中插入图片的位置
1. 在段落之前：段落会在图像之后另起一行开始显示
1. 在段落的起始处：段落文本的第一行将与图像的底部对齐
1. 在段落之中：图像将位于他所在段落文字之中

注： 图像插入块级元素中重视另起一行显示，内联元素位于块级元素中，并且不会另起一行显示
## 图像的水平对齐
1. `align:left` 左对齐,同时图像会被置于左侧
1. `align:right` 右对齐，同时图像会被置于右侧
## 图像垂直对齐方式
1. `align:top` 顶端对齐，相对于第一行
1. `align:middle` 居中对齐，相对于第一行
1. `align:bottom` 底端对齐，相对于第一行
## 图像格式
1. JPEG格式：图片中包含多种不同的颜色时用JPEG格式
1. Gif格式：动图、某个区域填充了完全相同的颜色时用，如果图像透明度部分有直边且这部分100%透明
1. PNG格式：当图像中包含少量的颜色或者大面积的相同区域时，应该保存为GIF或PNG，图像透明度部分有斜边或圆边，或般透明度或投影

# 表格
## 基本表格结构
1. `table` 表格
    +  `cellpadding="10"` 内边距
    +  `cellspacing="5"` 间隔
1. `thead` 表头
1. `thbody` 表中
1. `tfoot` 表尾
1. `tr` 每行
1. `td` 每个单元格
    +  `colspan="2"` 跨行
    +  `rowspan="2"` 跨列
1. `th` 标题
    +  `scope="col"` 列标题
    +  `scope="row"` 行标题
1. `width` 宽度
1. `bgcolor` 背景色

# 表单
## 表单结构
1. `form` 表单
    + `action`属性链接地址
    + `method`属性请求方式
        +   使用get请求的情况有：短表单、只从服务器检索数据的情形
        +   使用post请求的情况有：允许用户上传文件、非常长、包含敏感信息、向数据库中添加信息，或删 除信息  

1. `input` 输入框  
    + `type="text"` 单行文本框
    + `type="password"` 密码框
    + `type="radio"` 单选按钮
    + `type="checkbox"` 复选框
    + `type="file"` 文件上传域
    + `type="submit"` 提交按钮
    + `type="image"` 图像按钮
    + `type="hidden"` 隐藏控件
    + `type="data"` 日期控件
    + `type="email"` 电子邮件
    + `type="url"` url输入
    + `type="search"` 搜索输入控件
        + `placeholder="placeholder"` 在用户输入之前显示的文本
1. `textarea` 文本域
    + `cols="20` 文本域宽度
    + `rows="4"` 行数
1. `select` 下拉列表框
    + `option` 列表项
    + `multiple="multiple"` 多选框
1. `button` 按钮
1. `label` 标签
1. `fieldset` 组合表单
    + `legend` 标题

注：
input中的id属性值跟label中for属性值相同
name这个特性对表单控件进行标识并与输入的信息一同传到服务器
maxlength限制用户在文本区域输入字符的数量
size不能再新表单中用来指定文本宽度

## 表单验证
    <form action="http://www.example.com/subscribe.php" method="post">
    <label for="username">Username</label>
    <input type="text" name="username" required="required" />
    <input type="submit" value="submit"/>
    </form>


# 其他标记
## DOCTYPE(文档类型)
DOCTYPE 用来告知浏览器此页使用了HTML的哪个版本，可以帮助浏览器正确的渲染页面
## id特性
id="pullquote"表示这个字段通过css设置为大写字母
## class特性
class特性指向他所属的类，关键段落含有一个值为important
## 块级元素
在浏览器窗口中显示时总是另起一行
块级元素有：
```
<h1><p><ul><li>
```
## 内联元素
总是与它相邻近元素出现在同一行
内联元素有：
```
<a><b><em>
```
## 内联框架
```
    <iframe 
    width="450"
    height="300"
    src="http://maps.google.co.uk/maps?
    q=moma+new+york
    &amp;output=embed"
    frameboder="0"
    scrolling="no">
    </iframe>
    scrolling表示是否在内嵌框架上显示滚动条
    frameborder表示是否显示框架的边框
    seamless表示不需要滚动条
```
## 页面信息
1. `meta` 空元素没有结束标签
1. `description` 描述信息
1. `keywords` 关键字
1. `author` 用于定义网页设计者
1. `pragma` 防止浏览器对页面的缓存
1. `expires` 用来指定页面的过期时间
1. `robots` 搜索是否将这个页面加入到他们的搜索结果中，如果不希望加就用noindex，如果希望加但不要收录页面上连接到其他页面用nofollow
  ## 转义字符
  小于号：&lt;
  大于号：&gt;
  and符号:&amp;
  双引号：&quot;
  美分符号：&cent;
  英镑符号：&pound;
  日元符号：&yen;
  欧元符号：&euro;
  版权符号：&copy;
  注册商标：&reg;
  商标：&trade;
  左单引号：&lsquo;
  右单引号：&rsquo;
  左双引号：&ldquo;
  右双引号：&rdquo;
  乘号：&times;
  除号：&divide;

`div`元素可以将块级元素聚合起
`span`可以将内联元素 聚合起来
# Flash、视频和音频

## 向网页中添加Flash影片
```
    <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/
    swfobject/2.2/swfoject.js"></script>
    <script type="text/javascript">
    swfobject.embedSWF("flash/bird.swf","bird","400","300","8.0.0");</script>
```
## 向网页中添加视频
```
<video src="video/puppy.mp4"
poster="images/puppy.jpg"
width="400" height="300"
peload
controls
loop>
```
1. `src` 指定视频路径
1. `poster` 在视频加载或播放前，指定播放器中显示一个图片
1. `width、height` 指定播放器的大小
1. `controls` 表示浏览器需要提供默认的播放控件
1. `autoplay` 视频文件自动播放
1. `loop` 视频结束后重新播放
1. `preload` 高数浏览器在页面加载时需要做什么
1. `none` 表示在用户按下播放按钮之前，浏览器不必加在视频
1. `auto` 表示浏览器应该在页面加载时载入视频
1. `metadata` 表示浏览器只需要收集少量视频信息，比如大小，首正图片，播放列表和持续时间
## 多个视频资源
```
    <source src="video/puupy.webm" type="video/webm";
    codecs="vp8, vorbis"/>
    <source>:可以在<video>后使用，<source>可以代替起始标签<video>中的src特性
    src：用于指定视频路径
    type：视频格式
    codecs：对视频进行编码
```
## 向视频中添加HTML5音频
```
<audio src="audio/test-audio.ogg"
controls autoplay>
<audio>为页面添加音频文件
src:指定音频文件路径
controls：表明播放器是否播放
autoplay:自动开始播放
preload：没有设置autoplay时告诉浏览器应该做什么
loop：表示音频结束后进行重新播放
## 多个音频资源
<source src="audio/test-audio.ogg"/>
```







