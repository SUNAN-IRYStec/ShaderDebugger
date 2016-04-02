# ShaderDebugger A tool for shader debugging

##  Intro


##  Usage:

##  Other Info

---

# ShaderDebugger 着色器调试工具

##  介绍

[`Codea`](codea.io) 支持在 `iPad` 上直接编写 `OpenGL ES` 的 `shader` 程序, 对于设计 `3D` 程序而已非常方便, 但是 `shader` 内部的变量无法直接观察, 使得调试起来比较困难. 鉴于此, 试着写了一个可以把 `shader` 内部变量值输出到屏幕的工具, 类似原型的东西, 比较粗糙, 性能很差, 不过刚好能用, 利用它可以轻松地观察 `shader` 内变量的值.

##  工具函数说明

实际上就是几个函数, 包括:

* 用于记录屏幕坐标的两个全局变量 `float x` 和 `float y`
* 用于最终显示变量值的 `showFloat()`
* 用于生成所需字型的 `ledRectChar()`
* 用于判断矩形区域范围的 `inRect()`

##  使用方法

把全局变量和该函数的声明和实现拷贝到 `fragment shader` 的代码中, 直接在 `main` 函数中调用即可, 如下所示:

### 显示整数

正整数

```
shoufloat(float(2345));
```

负整数
```
shoufloat(float(2345));
```

浮点数

```
shoufloat(.2345));
```

```
shoufloat(1234.345);
```

```
shoufloat(-1234.345);
```

##  其他

记录完成这个原型工具的整个开发调试过程的思路

[]()
[]()