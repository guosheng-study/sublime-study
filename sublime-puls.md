#sublime 常用插件

```html
<script>alert(1);</script>
```

###1.emmet
概括地说，Emmet（译者注：前身就是以前大名鼎鼎的Zen Coding，这个如果你没听说和使用过，就悲哀了）是一个可以让你更快更高效地编写HTML和CSS，节省你大量时间的插件。怎么使用？你只需按约定的缩写形式书写而不用写整个代码，然后按“扩展”键，这些缩写就会自动扩展为对应的代码内容。 比如，你只需要输入
```html
((h4>a[rel=external])+p>img[width=500 height=320])*12
```
然后它会被扩展转换成12个列表项和紧随其后的图像。然后你就可以在此基础上再填写内容，就这么简单。   
官网：http://emmet.io/   
语法：http://docs.emmet.io/abbreviations/syntax/  
GitHub : https://github.com/sergeche/emmet-sublime  

注意：sublime text 3可能提示让你下载pyv8这样的东西   
下载地址：https://github.com/emmetio/pyv8-binaries#readme   
下载之后解压到Sublime Text 3的安装目录

###2.DocBlockr
DocBlockr 可以使你很方便地对代码建立文档。它会解析函数，变量，和参数，根据它们自动生成文档范式，你的工作就是去填充对应的说明。在js里面输入/**然后按一下Tab键就好。
```js
/**
 * @param  {[type]}
 * @param  {[type]}
 * @return {[type]}
 */
function foo(n, m) {
    return n + m;
}
```


###3.cssFormat
CSS格式化，必备插件之一,安装完毕之后设定快捷键，然后就在快捷键了。
```
[
	// Convert to Expanded Format
	{
		"keys": ["ctrl+alt+["],
		"command": "css_format",
		"args": {
			"action": "expand"
		}
	},

	// Convert to expanded format (break selectors)
	{
		"keys": ["ctrl+alt+b"],
		"command": "css_format",
		"args": {
			"action": "expand-bs"
		}
	},

	// Convert to Expanded Format (Break Selectors)
	{
		"keys": ["ctrl+alt+v"],
		"command": "css_format",
		"args": {
			"action": "expand-bs"
		}
	},

	// Convert to Compact Format
	{
		"keys": ["ctrl+alt+]"],
		"command": "css_format",
		"args": {
			"action": "compact"
		}
	},

	// Convert to Compact Format (No Spaces)
	{
		"keys": ["ctrl+alt+n"],
		"command": "css_format",
		"args": {
			"action": "compact-ns"
		}
	},

	// Convert to Compact Format (Break Selectors)
	{
		"keys": ["ctrl+alt+b"],
		"command": "css_format",
		"args": {
			"action": "compact-bs"
		}
	},

	// Convert to Compact Format (Break Selectors and No Spaces)
	{
		"keys": ["ctrl+alt+m"],
		"command": "css_format",
		"args": {
			"action": "compact-bs-ns"
		}
	},

	// Convert to Compressed Format
	{
		"keys": ["ctrl+alt+\\"],
		"command": "css_format",
		"args": {
			"action": "compress"
		}
	}
]
```

###4.jsFormat
有了这个插件，可以写出看上去比较整齐的代码了。安装之后的快捷键是ctrl+alt+f
不过我习惯把他设置保存的时候，自动格式化。
更多介绍：https://packagecontrol.io/packages/JsFormat
```
{
    // exposed jsbeautifier options
    "indent_with_tabs": false,
    "preserve_newlines": true,
    "max_preserve_newlines": 4,
    "space_in_paren": false,
    "jslint_happy": false,
    "brace_style": "collapse",
    "keep_array_indentation": false,
    "keep_function_indentation": false,
    "eval_code": false,
    "unescape_strings": false,
    "break_chained_methods": false,
    "e4x": false,
    "wrap_line_length": 0,

    // jsformat options
    "format_on_save": true, //保存的时候自动格式化
    "format_selection": true,
    "jsbeautifyrc_files": false,
    "ignore_sublime_settings": true
}

```


###5.jQuery语法提示
安装此插件后，输入$.each然后按几下Tab可以体验一下。
更多介绍：https://packagecontrol.io/packages/jQuery
```js
$.each(function(index, el) {
	
});
```

###6.underscorejs snippets
安装此插件后，输入_each然后按几下Tab可以体验一下。
```js
_.each(list, function(value, key, list){

	// body

});
```
###7.TortoiseSVN
公司用这个，那就装一下这个插件。
需要配置TortoiseSVN安装地址，不然会用不了
```js
//"Preferences->Package Settings->TortoiseSVN->Settings - User" in the menu.
{
  // Auto close update dialog when no errors, conflicts and merges
  "autoCloseUpdateDialog": false,
  "tortoiseproc_path": "C:\\Program Files\\TortoiseSVN\\bin\\TortoiseProc.exe"
}
```

方便很多。这个插件装好之后有个快捷键
```
 - [alt+c] : commit current file.   
 - [alt+u] : update current file.  
 - [alt+r] : revert current file.  
```
更多介绍：https://packagecontrol.io/packages/TortoiseSVN

###8.BracketHighlighter
括号匹配功能很不错，还可以配置颜色。
安装完成后，打开Preferences -> package settings -> Bracket Highlighter -> Bracket Settings – User (注意是user)，然后添加如下代码
```
{
    "bracket_styles": {
        "default": {
            "icon": "dot",
            // "color": "entity.name.class",
            "color": "brackethighlighter.default",
            "style": "highlight"
        },
 
        "unmatched": {
            "icon": "question",
            "color": "brackethighlighter.unmatched",
            "style": "highlight"
        },
        "curly": {
            "icon": "curly_bracket",
            "color": "brackethighlighter.curly",
            "style": "highlight"
        },
        "round": {
            "icon": "round_bracket",
            "color": "brackethighlighter.round",
            "style": "highlight"
        },
        "square": {
            "icon": "square_bracket",
            "color": "brackethighlighter.square",
            "style": "highlight"
        },
        "angle": {
            "icon": "angle_bracket",
            "color": "brackethighlighter.angle",
            "style": "highlight"
        },
        "tag": {
            "icon": "tag",
            "color": "brackethighlighter.tag",
            "style": "highlight"
        },
        "single_quote": {
            "icon": "single_quote",
            "color": "brackethighlighter.quote",
            "style": "highlight"
        },
        "double_quote": {
            "icon": "double_quote",
            "color": "brackethighlighter.quote",
            "style": "highlight"
        },
        "regex": {
            "icon": "regex",
            "color": "brackethighlighter.quote",
            "style": "outline"
        }
    }
}
```
更多介绍：http://facelessuser.github.io/BracketHighlighter/

###9.SublimeTmpl
一直都很奇怪为什么sublime text 3没有新建文件模板的功能，像html头部的DTD声明每次都要复制粘贴。用SublimeTmpl这款插件终于可以解脱了，SublimeTmpl能新建html、css、javascript、php、python、ruby六种类型的文件模板，所有的文件模板都在插件目录的templates文件夹里，可以自定义编辑文件模板。
```
ctrl+alt+h html
ctrl+alt+j javascript
ctrl+alt+c css
ctrl+alt+p php
ctrl+alt+r ruby
ctrl+alt+shift+p python
```
如果想要新建其他类型的文件模板的话，先自定义文件模板方在templates文件夹里，再分别打开Default (Windows).sublime-keymap、Default.sublime-commands、Main.sublime-menu、SublimeTmpl.sublime-settings这四个文件照着里面的格式自定义想要新建的类型


###10.Case Conversion
是不是有人忽略了大小写转化？这个插件帮助你节约宝贵时间。
```
To snake_case: "ctrl+alt+c", "ctrl+alt+s"
To camelCase: "ctrl+alt+c", "ctrl+alt+c"
To PascalCase: "ctrl+alt+c", "ctrl+alt+p"
To dot.case: "ctrl+alt+c", "ctrl+alt+d"
To dash-case: "ctrl+alt+c", "ctrl+alt+h"
To separate words: "ctrl+alt+c", "ctrl+alt+w"
to separate with slashes: "ctrl+alt+c", "ctrl+alt+/"
To toggle between snake_case, camelCase and PascalCase: "ctrl-shift-_"
```
不过上面上面的快捷有冲突我自己定义了一下
```
{
        "keys": ["ctrl+k", "ctrl+u"],
        "command": "convert_to_snake"
    }, {
        "keys": ["ctrl+k", "ctrl+k"],
        "command": "convert_to_camel"
    }, {
        "keys": ["ctrl+k", "ctrl+j"],
        "command": "convert_to_pascal"
    }, {
        "keys": ["ctrl+k", "ctrl+n"],
        "command": "convert_to_dot"
    }
```


###11.LiveStyle
解决两个问题：
1、每次修改样式，查看修改结果的时候都需要刷新一下页面才能看到。  
2、调试页面再chrome下修改的样式不能同步到原始文件中，要照着chrome中调试好的，再去原始文件再去敲一遍。  

当然光是装了sublime text的插件还不行，另外还得装chrome对应的插件
插件地址：http://www.crx4chrome.com/crx/993/


###12. SideBarEnhancements
SideBarEnhancements本是增强侧边栏的插件，里面有一个将图片直接转成base64也很不错。




