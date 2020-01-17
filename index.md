<head>
<meta charset="UTF-8">
<title>网页时钟</title>
<script type="text/javascript">
    //判断时间是否为个位数，如果时间为个位数就在时间之前补上一个“0”
	function check(val) {
		if (val < 10) {
			return ("0" + val);
		} 
		else {
			return (val);
		}
	}
	function displayTime() {
		//获取div元素
		var timeDiv=document.getElementById("timeDiv");
		//获取系统当前的年、月、日、小时、分钟、毫秒
		var date = new Date();
		var year = date.getFullYear();
		var month = date.getMonth() + 1;
		var day = date.getDate();
		var hour = date.getHours();
		var minutes = date.getMinutes();
		var second = date.getSeconds();
		var timestr = year + "年" + month + "月" + day + "日  " + check(hour)
				+ ":" + check(minutes) + ":" + check(second);
		//将系统时间设置到div元素中
		timeDiv.innerHTML = timestr;
	}
	//每隔1秒调用一次displayTime函数
	function start(){
        window.setInterval("displayTime()",1000)//单位是毫秒
}
</script>
</head>
<!--  body onload:当整个html页面加载完成后执行此函数  -->
<body οnlοad="start();">

<font color="red">jhfjfjhf</font>
## since we met

LY WP


### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/liyanbit/SWM/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
