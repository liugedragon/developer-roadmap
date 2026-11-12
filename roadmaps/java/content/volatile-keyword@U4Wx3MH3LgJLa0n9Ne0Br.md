# Volatile Keyword

The `volatile` keyword in Java can be applied to instance and static fields. A write to a volatile field happens-before every subsequent read of that field, providing visibility and ordering guarantees between threads. These are Java Memory Model guarantees, not a requirement to bypass processor caches or access physical main memory directly. Individual reads and writes of a volatile field are atomic, but compound operations such as `count++` are not made atomic by declaring `count` volatile; use synchronization or an atomic class such as `AtomicInteger` when updates must be atomic.

Visit the following resources to learn more:

- [@official@Java Language Specification: volatile Fields](https://docs.oracle.com/javase/specs/jls/se21/html/jls-8.html#jls-8.3.1.4)
- [@official@Java Language Specification: Happens-before Order](https://docs.oracle.com/javase/specs/jls/se21/html/jls-17.html#jls-17.4.5)
- [@article@Java Volatile Keyword](https://jenkov.com/tutorials/java-concurrency/volatile.html)
- [@article@Guide to the Volatile Keyword in Java](https://www.baeldung.com/java-volatile)
