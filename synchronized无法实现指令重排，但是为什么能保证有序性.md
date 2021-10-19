## synchronized无法实现指令重排，但是为什么能保证有序性

### 关键点：

1. as-if-serial保证单线程下的程序执行结果的准确性
2. synchronized保证程序段执行之前获得锁，只允许本线程获得这个锁

### 答题步骤：

1. 解释什么叫指令重排，它的实现原理
2. 通过指令重排导出会出现有序性问题
3. 引出as-if-serial语义，说出它的作用
4. 解释一下synchronized，原理，还有它的作用（重入锁，<u>排他锁</u>）
5. 联系as-if-serial和synchronized