# JavaCodeThreadSafetyTree
Java代码的线程安全性研究技术

<pre>
如何写线程安全的代码：

      在Java中，有许多方式去编写线程安全的代码：
           1）使用synchronized关键字,某个时刻，只有一个线程可以执行它，也就实现了线程安全。
           2）使用原子的Integer，原子的Integer可以保证++操作的原子性。

      在Java编程中，记住这些关键点可以帮你避免一些严重的并发问题，比如条件竞争或者死锁。

           1）不可变对象默认是线程安全的。
           2）只读，final类型的变量也是线程安全的。
           3）锁也是一种线程安全的方式。
           5）使用线程安全的类：vector, hashtable, cocurrenthashmap, String等
           6）原子操作是线程安全的，如32位的内存数据。
           7）本地变量是线程安全的。 ThreadLocal,因为每个线程都有自己的变量copy。
           8）多线程之间的共享对象尽可能的少，也就尽可能避免线程安全的问题。
           9）Volatile关键字。
</pre>