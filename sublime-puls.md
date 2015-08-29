#sublime 常用插件

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
