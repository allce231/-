## 前端常用的一些方法总结（可以出面试题哦）-- by Hanson.liu

###javascript 篇

####一、javascript获取当前时间戳的4种方式
    1, var t = Date.parse(new Date()); //时间戳是把毫秒改成000显示
    2, var t = new Date().getTime();
    3, var t = new Date().valueOf();
    4, var t = +new Date();

####二、javascript判断是否为数组
    var toString = Object.prototype.toString;
        toString.call("") // [object String];
        toString.call([]) // [object Array];
        toString.call(function(){}) // [object Function];
        toString.call(undefined) // [object Undefined];
        toString.call(null) // [object Null];

####三、jQuery 插件常用写法

    (function($){
        var defaults = {
            //...
        };

        $.fn.test = function(options){
            var opt = $.extend(defaults,options);
            //支持JQuery选择器 链式调用
            return this.each(function(){
                //...
            });
        };
    })(jQuery);

####四、


### css 篇
