redis源码：
https://blog.huangz.me/diary/2014/how-to-read-redis-source-code.html

ziplist entry:<br>
从前往后一次是：<br>
1、前一个entry长度,用于从后往前遍历：小于254是一个字节，大于254是5个字节（0xFE + len(int32)）<br>
2、根据entry的类型决定：<br>
参考文件头的注释<br>
整数都是小端序<br>

redis对象<br>
https://www.cnblogs.com/wind-snow/p/11172832.html
