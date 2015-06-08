# iOS Best Practices
这里总结一下iOS最佳实践，主要参考Futurice developers的文章[iOS Good Practices](https://github.com/futurice/ios-good-practices)，同时加上了一些自己的理解

##目录
* 初始化项目


##初始化项目
###UI采用Interface Builder还是手写代码
当开始一个iOS项目时，一个常见的问题就是编写所有的views是采用手写代码的方式还是使用Interface Builder的Storyboard或XIB文件。两种方式都可以实现相同UI效果，但几点需要考虑：

####为什么使用代码？
* 当多人协作开发时，由于Storyboard复杂的XML结构，它更容易发生版本冲突，这比手写代码的方式更难合并代码。
* 手写代码更容易地结构化和重用views，因此使你的代码库保持[DRY](http://en.wikipedia.org/wiki/Don%27t_repeat_yourself)。
* 所有的信息都在同一个地方。在Interface Builder中，你必须通过点击所有inspectors才能找到你想要的东西。

####为什么使用Storyboard？
* 为了更少的技术要求，Storyboard通过微调颜色或布局约束等方式来直接对项目做出贡献是一种很好的方式。但它需要设置工程并且需要时间来学习基础。
* 由于你无需构建项目就可以预览一些变化，迭代速度就变得更快了
* 在Xcode 6，自定义字体和UI元素最后都以可视化的方式在Storyboard上显示，当你设计最终外观时，给你更加好的灵感。
* 从iOS 8开始，[Size Class](http://blog.futurice.com/adaptive-view-ios8)允许你为不同的类型的设备和屏幕来设计并且没有重复


###Git版本控制与.gitignore

###项目设置

###使用Cocoapods管理库

###项目目录结构