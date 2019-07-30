>微信公众号：**[志文工作室(lzw-me)]**
关注计算机基础应用技术、前端开发等，公众号内同步发布志文工作室博客最新文章。问题或建议，请公众号留言。

![志文工作室公众号](https://lzw.me/images/wechat/lzwme-qrcode_430.jpg)

## Markdown-Weixin 简介

Markdown 转微信公众帐号内容神器，能让`Markdown`内容，无需作任何调整就能**一键复制**到微信公众号使用，特别针对代码展示做了优化。

> 使用微信公众号编辑器有一个十分头疼的问题——粘贴出来的代码，格式错乱，而且特别丑。

## 代码块显示效果

注：markdown对代码块的语法是开始和结束行都要添加：\`\`\`,其中 \` 为windows键盘左上角`esc` 下面的那个键。示例如下：
```css
ul, ol {
  margin: 0;
  padding: 0;
  padding-left: 40px;
}

.task-list-list {
  margin: 0;
  padding: 0;
}

table {
  display: table;
  width: 100%;
}
```

要精确指定语言（如：`java,cpp,css,xml,javascript,python,php,go,kotlin,lua,objectivec`等）时，在头部直接指定，如：\`\`\`javascript，如下：

```javascript
let timer;
function showSnackbar() {
  const $snackbar = $('#snackbar');
  $snackbar.addClass('show');
  clearTimeout(timer);
  timer = setTimeout(() => {
    $snackbar.removeClass('show');
  }, 3000);
}
```

在页面头部提供了很多中**代码主题**风格，可以根据需要选择合适的即可。

### Markdown基本语法

#### 标题
支持6种大小的标题，分别对应`#`,`##`,`###`,`####`,`#####`,`######`，和样式文件中的`h1,...,h6`如：
##### H5
###### H6

####行内代码
如：`AppCompatActivity`类,markdown对行内代码的语法是前后用：\`,其中 \` 为windows键盘左上角那个,

#### 强调
**我是强调**

#### 斜体
试试*斜体*

#### 强调的斜体
试试***强调的斜体***

#### 删除
试试 ~~删除~~

#### 外链的超链接
试试外链的超链接：[我是外链的超链接](http://blog.qikqiak.com),markdown对链接的语法为：`[]()`,如：`[我是外链的超链接](http://blog.qikqiak.com)`

#### 页内的超链接
试试页内的超链接：[我是页内的超链接](#jump_1)，注：你先要在要跳转的到地方放置一个类似：`<a id="jump_1">任意内容</a>`的锚点。由`id="jump_1" `来匹配。

#### 有序列表
1. 有序列表 1
2. 有序列表 2
3. 有序列表 3

#### 无序列表
- 无序列表 1
- 无序列表 2
- 无序列表 3

#### 引用块
只需要在前面加 `>`,如下:
>我是引用块
微信公众号：k8s技术圈
欢迎关注我，一起学习，一起进步，All in Kubernetes!

#### 分隔线
***

### Markdown扩展语法

#### 表格
| 班级 | 男生 | 女生 |
|-----|-----|------|
| 一(7)班 | 30   | 25 |
| 一(8)班 | 25   | 30 |

注：表格在公众号预览时，可能在PC端显示的不是正确的全屏，但在手机上预览时就会正常显示为全屏的了。

### 直接支持html,css
如果你懂html和css，那下面这些效果就不在话下了：

<a href="#jump_1">来个页内跳转</a>，跳转到文未的：`<a id="jump_1">我是页内跳转到的位置</a>` ,对应：`id="jump_1"`
<span  style="color: #5bdaed; ">先给点颜色你看看</span>
<span  style="color: #AE87FA; ">再给点颜色你看看</span>
<span  style="font-size:1.3em;">试试改变字体大小</span>
<span  style="font-size:1.3em;font-weight: bold;">改变字体大小，再来个粗体又如何？</span>

<p style="text-align:center">
试试内容居中

</p>

<p style="text-align:right">
那内容居右呢？
</p>

<p style="text-align:center;color:#1e819e;font-size:1.3em;font-weight: bold;">
来个综合的试试
<br/>
第二行
</p>

***
<a id="jump_1">我是页内跳转到的位置</a>

### LICENSE
MIT. Thanks for @barretlee.
