# ArrayList

##  类图

 ![类图](http://static.iocoder.cn/images/JDK/2019_12_01/01.png) 

实现了 4 个接口，分别是：

java.util.List 接口，提供数组的添加、删除、修改、迭代遍历等操作。
java.util.RandomAccess 接口，表示 ArrayList 支持快速的随机访问。

java.io.Serializable 接口，表示 ArrayList 支持序列化的功能。

java.lang.Cloneable 接口，表示 ArrayList 支持克隆。

继承了 java.util.AbstractList 抽象类，而 AbstractList 提供了 List 接口的骨架实现，大幅度的减少了实现迭代遍历相关操作的代码。可能这样表述有点抽象，胖友点到 java.util.AbstractList 抽象类中看看，例如说 #iterator()、#indexOf(Object o) 等方法。

不过实际上，在下面中我们会看到，ArrayList 大量重写了 AbstractList 提供的方法实现。所以，AbstractList 对于 ArrayList 意义不大，更多的是 AbstractList 其它子类享受了这个福利



java.lang.Cloneable 接口和ava.util.RandomAccess 接口说明见本目录下其他文章

