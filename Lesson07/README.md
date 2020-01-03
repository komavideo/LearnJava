变量的类型
=========

## 知识点

* 变量定义
* 变量类型

参考网页：

https://docs.oracle.com/javase/tutorial/java/nutsandbolts/datatypes.html

## 实战演习

~~~java
public class Main {
    /**
     * 类变量（静态）
     */
    private static String VERSION = "1.0.0";
    /**
     * 实例变量
     */
    String mStr = "helo";

    public static void main(String[] args) {

        /**
         * 方法级局部变量
         */
        // 声明三个int型整数：a、 b、c
        int a, b, c;
        // 声明三个整数并赋予初值
        int d = 10, e = 20, f = 30;
        // 声明并初始化g
        byte g = 99;
        // 声明并初始化字符串str
        String str = "komavideo";
        // 声明了双精度浮点型变量PI
        double PI = 3.141592654;
        // 声明变量c的值是字符'z'
        char chr = 'z';

        System.out.println("Version:" + VERSION);
        System.out.println("mStr:" + new Main().mStr);
        System.out.println("PI:" + PI);
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
