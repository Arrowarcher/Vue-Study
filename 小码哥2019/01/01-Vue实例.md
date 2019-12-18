新建Vue实例时传入了options对象
```js
var vm = new Vue({		//options
			})
```

- el
	- string|HTMLElement
	- 决定Vue实例管理哪个DOM
- data
	- Object|Function（组件当中data必须是函数）
	- 实例对应得数据对象
- methods
	- {key:Function}
	- 方法