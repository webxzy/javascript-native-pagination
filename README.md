# javascript native pagination 
一款用原生javascript写的分组插件，简单易用

## 使用 Usage
- 首先在你的页面里引入。也可以使用require，这里不做演示了
```
<script type="text/javascript" src="pagination.js"></script>
```

- 在你的页面里提供一个带ID的元素
```
<ul id="pageLsit"></ul>
```

- 调用
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

## 参数 Options
- id 页面元素的id
- total 总页数
- showButtons 需要显示的按钮数量 default: 6
- callback 点击分页后触发的回调，pageIndex就是当前选择的页面的索引，从0开始

## 其他说明 Other
- 当showButtons的数量大于total的数量时，就会按照total的数量来渲染分页的按钮数量。只有当total的数量大于showButtons的数量时，设置的展示按钮数量才会有效。
- 样式可以自己定义。
Email: webxzy@qq.com