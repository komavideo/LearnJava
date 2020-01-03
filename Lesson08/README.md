异常处理
========

在Java程序执行过程中会遇到各种运行时的错误，我们应该在编码过程中预见到这些错误，并进行捕捉和进行适当的错误处理。

## 知识点

* try/catch
* try/catch/finally

## 实战演习

~~~java
public class Main {
    public static void main(String[] args) {
        try {
            System.out.println("===处理开始===");
            //业务处理逻辑
            int a = 40;
            int b = 10;
            System.out.println(a / b);
        } catch (Exception e) {
            //错误捕捉并处理
            System.out.println("XXX错误处理XXX");
            System.out.println(e.toString());
        } finally {
            //收尾处理：无论错误发生与否，都会这行这段逻辑
            System.out.println(">>>收尾处理<<<");
        }
    }
}
~~~

## 课程文件

https://github.com/komavideo/LearnJava

## 小马视频频道

http://komavideo.com
