## JAVA字符串

常量创建的字符串存储在公共池上，而new出来的字符串位于堆上

```java
String s1 = "Runoob";              // String 直接创建
String s2 = "Runoob";              // String 直接创建
String s3 = s1;                    // 相同引用
String s4 = new String("Runoob");   // String 对象创建
String s5 = new String("Runoob");   // String 对象创建
```

### StringBuilder和StringBuffer

- **StringBuffer 和 StringBuilder 类的对象能够被多次的修改，并且不产生新的未使用对象。**

- 在使用 StringBuffer 类时，每次都会对 StringBuffer 对象本身进行操作，而不是生成新的对象，所以如果需要对字符串进行修改推荐使用 StringBuffer。

- StringBuilder 类和 StringBuffer 之间的最大不同在于 StringBuilder 的方法不是线程安全的（不能同步访问）。

- 由于 StringBuilder 相较于 StringBuffer 有速度优势，所以多数情况下建议使用 StringBuilder 类。

------



## Java集合学习

### 1.HashSet

- HashSet 基于 HashMap 来实现的，是一个不允许有重复元素的集合。

- HashSet 允许有 null 值。

- HashSet 是无序的，即不会记录插入的顺序。

- HashSet 不是线程安全的， 如果多个线程尝试同时修改 HashSet，则最终结果是不确定的。 您必须在多线程访问时显式同步对 HashSet 的并发访问。

### 2.HashMap

- HashMap 是一个散列表，它存储的内容是键值对(key-value)映射。

- HashMap 实现了 Map 接口，根据键的 HashCode 值存储数据，具有很快的访问速度，最多允许一条记录的键为 null，不支持线程同步。

- HashMap是无序的，即不会记录插入的顺序。

### 3.ArrayList

- 底层数据结构是数组，创建时无需指定大小，方便扩容
- 动态扩容，第一次add数据时会初始化一个默认大小10，然后每次添加的时候判断是否足够大，不够的话会扩容，每一次通grow()方法扩容为原来大小的1.5倍。





