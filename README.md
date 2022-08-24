redis源码：
https://blog.huangz.me/diary/2014/how-to-read-redis-source-code.html

ziplist entry:
从前往后一次是：
1、前一个entry长度,用于从后往前遍历：小于254是一个字节，大于254是5个字节（0xFE + len(int32)）
2、根据entry的类型决定：
参考文件头的注释
整数都是小端序

redis对象<br>
https://www.cnblogs.com/wind-snow/p/11172832.html
