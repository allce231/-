# 常用的一些总结（可以出面试题哦）

一、javascript获取当前时间戳的4种方式
    1, var t = Date.parse(new Date()); //时间戳是把毫秒改成000显示
    2, var t = new Date().getTime();
    3, var t = new Date().valueOf();
    4, var t = +new Date();
