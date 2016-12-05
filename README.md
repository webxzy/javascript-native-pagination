# javascript native pagination 
一款用原生javascript写的分组插件，简单易用

## 如何使用 start
1. 首先在你的页面里引入。也可以使用require，这里不做演示了
```
<script type="text/javascript" src="pagination.js"></script>
```

2. 在你的页面里提供一个带ID的元素
```
<ul id="pageLsit"></ul>
```

3. 调用
```
var page = new Pagination({
	id: 'pageList',
	total: 21,
	showButtons: 10,
	callback: function (pageIndex) {
		console.log(pageIndex);
	}
});
```

## 关于参数 Options
- id 页面元素的id
- total 总页数
- showButtons 需要显示的按钮数量
- callback 点击分页后触发的回调，pageIndex就是你的当前选择的页面的索引，从0开始

Email: webxzy@qq.com