用T(v)表达式来将变量v转换成类型T

!!! warning "必须指定类型才能转换"
	var a int = 5，那么：

	var b string = string(a) 是OK的，而var b string = a是会报错的

另外，var b = string(a)，或者b := string(a)也可以