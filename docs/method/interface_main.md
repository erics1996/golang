- 接口类型是由一组方法定义的集合。

- 接口类型的值可以存放实现这些方法的任何值。

- 接口不是被调用者来写，而是调用者来写

go语言的设计哲学认为：功能实现者的责任只要提供具体功能，用哪些interface来对功能做抽象是使用者的自由。功能实现者没有办法确定使用者会对自己提供的功能做哪些抽象，所以功能实现者不应该也没有能力设定接口。

例如：自己的代码要调用模块A，那么接口是自己来写，而不是模块A来写，即模块A里只有一堆的struct和其方法，自己写接口来封装这些struct方法是为了让自己的代码写起来更灵活（解耦）。
