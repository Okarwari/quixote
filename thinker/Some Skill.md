####一些技巧


####切片是python十分好用的工具：
就我理解来说：
	切片是在原数组的基础上标记上被选中位置，然后对此位置（元素）进行读写。
	若是对他人进行赋值的话，他将被选中的元素里存储的值（所绑定对象的地址）重新生成一个序列或者元组赋值给他人。同样，切片本身可以进行写入。通过其他切片可以对原始切片进行修改写入


####巧用进制有时候也可以很好的解决一些问题，比如对于一些用特定的数值去表示一些数