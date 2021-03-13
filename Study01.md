1. ## 字符串常量创建的字符串存储在公共池上，而new出来的字符串位于堆上

   ```java
   String s1 = "Runoob";              // String 直接创建
   String s2 = "Runoob";              // String 直接创建
   String s3 = s1;                    // 相同引用
   String s4 = new String("Runoob");   // String 对象创建
   String s5 = new String("Runoob");   // String 对象创建
   ```

   

   ## Java集合学习

   HashSet 基于 HashMap 来实现的，是一个不允许有重复元素的集合。

   HashSet 允许有 null 值。

   HashSet 是无序的，即不会记录插入的顺序。

   HashSet 不是线程安全的， 如果多个线程尝试同时修改 HashSet，则最终结果是不确定的。 您必须在多线程访问时显式同步对 HashSet 的并发访问。

   

